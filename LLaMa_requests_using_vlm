from vllm import LLM, SamplingParams
import os
import pandas as pd
from tqdm import tqdm
import requests
import json
from math import ceil
from tqdm import tqdm
import torch 

# vLLM model details
model_name = "meta-llama/Llama-3.1-8B-Instruct"

# Load the model using vLLM
llm = LLM(model_name)

categories = ['Sports', 'Economy', 'Other', 'Environment', 'Entertainment', 'Health', 
              'Justice', 'Religion', 'Politics', 'Culture', 'Terrorism', 'Technology', 
              'Immigration', 'Crime', 'Society', 'Education', 'Tragedy/Disaster', 'Journalism', 
              'Food', 'Animal', 'Human Interest', 'Science', 'Conflict', 'Travel', 'Relations']

# Define base prompt to classify topics
base_prompt = """You are an expert news editor. Your job is to classify each Italian news headlines into one of these topics: ['Sports', 'Economy', 'Other', 'Environment', 'Entertainment', 'Health', 'Justice', 'Religion', 'Politics', 'Culture', 'Terrorism', 'Technology', 'Immigration', 'Crime', 'Society', 'Education', 'Tragedy/Disaster', 'Journalism', 'Food', 'Animal', 'Human Interest', 'Science', 'Conflict', 'Travel', 'Relations'].

Instructions:
You must provide only one topic as an answer and nothing more.
Please use the "Other" topic only when all the others are inappropriate and limit its usage.

Examples:
Headline: "Juve al Mondiale per Club, ufficiale l’ultima novità: tutte le avversarie"
Topic: "Sports"

Headline: "Manovra, il governo accelera: testo oggi in Cdm insieme a decreto fiscale."
Topic: "Politics"

Now, is your turn:
Headline: "{}"
Topic: """

# Function to process a batch of sentences and classify the topics
def process_batch(headlines, batch_number, output_folder):
    results = []

    for headline in tqdm(headlines):
        print(f"Processing headline: {headline}")  # Debugging output
        dynamic_prompt = base_prompt.format(headline)  # Insert the headline into the prompt

        error_occurred = 0  # Initialize error flag
        try:
            # Define sampling parameters for generation
            sampling_params = SamplingParams(temperature=0.2, max_tokens=4)

            # Generate response from the model
            print("Generating response...")  # Debugging output
            output = llm.generate(dynamic_prompt, sampling_params)
            # Extract the first response from the output
            resp = output[0].outputs[0].text.strip()

            response_data = {"topic": resp}
            
        except Exception as e:
            print(f"Error processing headline '{headline}': {e}")
            error_occurred = 1  # Set error flag if an exception occurred
            response_data = {"topic": "unknown"}  # Assign a default 'unknown' topic if error occurs

        # Append the headline and response to results
        results.append({
            "headline": headline,
            "topic": response_data.get("topic", "unknown"),  # Ensure a default 'unknown' topic if missing
            "error": error_occurred  # Add error status
        })

    # Create a pandas DataFrame from the results
    df = pd.DataFrame(results)

    # Ensure the output folder exists
    os.makedirs(output_folder, exist_ok=True)

    # Save the batch to a CSV file
    batch_file = os.path.join(output_folder, f"batch_{batch_number}.csv")
    df.to_csv(batch_file, index=False)
    print(f"Batch {batch_number} saved to {batch_file}")

# Main processing function to handle multiple batches
def process_in_batches(sentences, batch_size, output_folder, start_batch=1):
    total_sentences = len(sentences)
    num_batches = (total_sentences + batch_size - 1) // batch_size  # Calculate the number of batches

    for i in range(start_batch - 1, num_batches):
        start_idx = i * batch_size
        end_idx = min(start_idx + batch_size, total_sentences)
        batch_sentences = sentences[start_idx:end_idx]
        print(f"Processing batch {i + 1}/{num_batches} with sentences {start_idx + 1} to {end_idx}")
        process_batch(batch_sentences, i + 1, output_folder)

# Example usage
df_headlines = pd.read_csv(r"/home/mberta/miniconda3/envs/lama_env/lama/data/headlines.csv")
sentences = df_headlines['headline'].tolist()  # Load all sentences from the "headline" column

batch_size = 16  # Specify a batch size
output_folder = r"/home/mberta/miniconda3/envs/lama_env/lama/data/output_vllm"  # Specify the output folder
start_batch = 1  # Specify the starting batch (1-indexed)

# Process the sentences in batches and save to CSV files
process_in_batches(sentences, batch_size, output_folder, start_batch)
