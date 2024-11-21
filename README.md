#
<div align="center">
  <h1>Decoding Narratives</h1>
    <h2>Towards a Classification Analysis for Stereotypical Patterns in Italian News Headlines</h2>
</div>
<br/>

This repository contains the source code of the paper *Decoding Narratives: Towards a Classification Analysis for Stereotypical Patterns in Italian News Headlines* presented at the **DS4EIW Workshop, IEEE BigData 2024** (TODO)

This work analyzes how Italian newspapers with opposing political leanings differ in their headline composition, particularly regarding stereotypical or clickbait content. Using a deep learning classifier and Explainable AI, the study highlights tonal distinctions: Newspaper A is more balanced and detailed, while Newspaper B is punchier and more provocative, especially on sensitive topics like immigration and social justice.

The pipeline followed for this analysis is the following: 

<p align = "center">
<img width="849" alt="Pipeline" src="https://github.com/user-attachments/assets/2cb8f65f-bc0b-48a5-a672-9ea28e6294aa">
</p>

## Table of Contents
- [Data](#data)
- [Usage](#usage)
- [References](#references)
- [Authors](#authors)

## Data
The data collection started from [CHANGE-it](https://huggingface.co/datasets/gsarti/change_it), a dataset that contains 152k article-headline pairs, collected from two Italian newspapers situated at the opposite ends of the political spectrum, with the two newspapers equally represented. 


## Usage



## References
```bibtex
@inproceedings{Clickbait_more_click,
author = {D. Molina, Maria and Sundar, S. Shyam and Rony, Md Main Uddin and Hassan, Naeemul and Le, Thai and Lee, Dongwon},
title = {Does Clickbait Actually Attract More Clicks? Three Clickbait Studies You Must Read},
year = {2021},
isbn = {9781450380966},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3411764.3445753},
doi = {10.1145/3411764.3445753},
articleno = {234},
numpages = {19},
location = {Yokohama, Japan},
series = {CHI '21}
}

@article{Effect_Of_Clickbait_on_Users,
  title={Effects of Clickbait Headlines on User Responses: An Empirical Investigation},
  author={Supavich Pengnate and Jeffrey Chen and Alex R. Young},
  journal={Journal of International Technology and Information Management},
  year={2021},
  url={https://api.semanticscholar.org/CorpusID:256298481}
}

@article{Click_me,
  author    = {Jung, Alexander K. and Stieglitz, Stefan and Kissmer, Tobias and Mirbabaie, Milad and Kroll, Thomas},
  title     = {Click me…! The influence of clickbait on user engagement in social media and the role of digital nudging},
  journal   = {PLOS ONE},
  year      = {2022},
  volume    = {17},
  number    = {6},
  pages     = {e0266743},
  doi       = {10.1371/journal.pone.0266743},
  pmid      = {35767538},
  pmcid     = {PMC9242456},
  month     = jun
}

@article{how_news_shape_political_knowledge,
  author    = {Suk, Jaeho and Coppini, Davide and Muñiz, Carlos and Rojas, Hernando},
  title     = {The more you know, the less you like: A comparative study of how news and political conversation shape political knowledge and affective polarization},
  journal   = {Communication and the Public},
  year      = {2022},
  volume    = {7},
  number    = {1},
  pages     = {40-56},
  doi       = {10.1177/20570473211063237}
}

@article{clickbait,
title = {Click bait: Forward-reference as lure in online news headlines},
journal = {Journal of Pragmatics},
volume = {76},
pages = {87-100},
year = {2015},
issn = {0378-2166},
doi = {https://doi.org/10.1016/j.pragma.2014.11.010},
url = {https://www.sciencedirect.com/science/article/pii/S0378216614002410},
author = {Jonas Nygaard Blom and Kenneth Reinecke Hansen},
keywords = {Online news headlines, Forward-reference, Cataphora, Discourse deixis, Media commercialization, Tabloidization},
abstract = {This is why you should read this article. Although such an opening statement does not make much sense read in isolation, journalists often write headlines like this on news websites. They use the forward-referring technique as a stylistic and narrative luring device trying to induce anticipation and curiosity so the readers click (or tap on) the headline and read on. In this article, we map the use of forward-referring headlines in online news journalism by conducting an analysis of 100,000 headlines from 10 different Danish news websites. The results show that commercialization and tabloidization seem to lead to a recurrent use of forward-reference in Danish online news headlines. In addition, the article contributes to reference theory by expanding previous models on phoricity to include multimodal references on the web.}
}

@article{guilty_by_association,
  author    = {Kroon, Anne C. and Trilling, Damian and Raats, Tim},
  title     = {Guilty by Association: Using Word Embeddings to Measure Ethnic Stereotypes in News Coverage},
  journal   = {Journalism \& Mass Communication Quarterly},
  year      = {2021},
  volume    = {98},
  number    = {2},
  pages     = {451-477},
  doi       = {10.1177/1077699020932304}
}


@article{uninformed_or_misinformed,
author = {Atle Haugsgjerd, Rune Karlsen and Kari Steen-Johnsen},
title = {Uninformed or Misinformed in the Digital News Environment? How Social Media News Use Affects Two Dimensions of Political Knowledge},
journal = {Political Communication},
volume = {40},
number = {6},
pages = {700--718},
year = {2023},
publisher = {Routledge},
doi = {10.1080/10584609.2023.2222070},
URL = { 
        https://doi.org/10.1080/10584609.2023.2222070
},
eprint = { 
        https://doi.org/10.1080/10584609.2023.2222070
}
}


@inproceedings{diving_deep_into_clickbaits,
author = {Rony, Md Main Uddin and Hassan, Naeemul and Yousuf, Mohammad},
title = {Diving Deep into Clickbaits: Who Use Them to What Extents in Which Topics with What Effects?},
year = {2017},
isbn = {9781450349932},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3110025.3110054},
doi = {10.1145/3110025.3110054},
abstract = {The use of alluring headlines (clickbait) to tempt the readers has become a growing practice nowadays. For the sake of existence in the highly competitive media industry, most of the on-line media including the mainstream ones, have started following this practice. Although the wide-spread practice of clickbait makes the reader's reliability on media vulnerable, a large scale analysis to reveal this fact is still absent. In this paper, we analyze 1.67 million Facebook posts created by 153 media organizations to understand the extent of clickbait practice, its impact and user engagement by using our own developed clickbait detection model. The model uses distributed sub-word embeddings learned from a large corpus. The accuracy of the model is 98.3\%. Powered with this model, we further study the distribution of topics in clickbait and non-clickbait contents.},
booktitle = {Proceedings of the 2017 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining 2017},
pages = {232–239},
numpages = {8},
location = {Sydney, Australia},
series = {ASONAM '17}
}

@inproceedings{clickbait_viral_journalism,
  title={Clickbait as a strategy of viral journalism: conceptualisation and methods},
  author={A Bazaco and Marta Redondo and Pilar S{\'a}nchez-Garc{\'i}a},
  year={2019},
  url={https://api.semanticscholar.org/CorpusID:150129578}
}

@INPROCEEDINGS{detecting_and_preventing_clickbaits,
  author={Chakraborty, Abhijnan and Paranjape, Bhargavi and Kakarla, Sourya and Ganguly, Niloy},
  booktitle={2016 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM)}, 
  title={Stop Clickbait: Detecting and preventing clickbaits in online news media}, 
  year={2016},
  volume={},
  number={},
  pages={9-16},
  keywords={Media;Syntactics;Facebook;Internet;Browsers;Web pages},
  doi={10.1109/ASONAM.2016.7752207}}

@misc{wang2024adaptablereliabletextclassification,
      title={Adaptable and Reliable Text Classification using Large Language Models}, 
      author={Zhiqiang Wang and Yiran Pang and Yanbin Lin and Xingquan Zhu},
      year={2024},
      eprint={2405.10523},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2405.10523}, 
}

@misc{LLaMa,
      title={LLaMA: Open and Efficient Foundation Language Models}, 
      author={Hugo Touvron and Thibaut Lavril and Gautier Izacard and Xavier Martinet and Marie-Anne Lachaux and Timothée Lacroix and Baptiste Rozière and Naman Goyal and Eric Hambro and Faisal Azhar and Aurelien Rodriguez and Armand Joulin and Edouard Grave and Guillaume Lample},
      year={2023},
      eprint={2302.13971},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2302.13971}, 
}

@article{choosing_the_right_words,
author = {W. Timothy Coombs},
title ={Choosing the Right Words: The Development of Guidelines for the Selection of the “Appropriate” Crisis-Response Strategies},

journal = {Management Communication Quarterly},
volume = {8},
number = {4},
pages = {447-476},
year = {1995},
doi = {10.1177/0893318995008004003},
URL = { 
        https://doi.org/10.1177/0893318995008004003
},
eprint = { 
        https://doi.org/10.1177/0893318995008004003
}
,
    abstract = { Although crisis management has evolved rapidly over the past decade, the symbolic aspect of crisis management has been ignored. More specifically, little research has examined crisis-response strategies (public statements made after a crisis) to see how these messages can be used to shape public perceptions of the crisis and the organization in crisis. This article synthesizes existing literature to create a list of crisis-response strategies and develops a set of guidelines for appropriate use of a given strategy. The guidelines are based upon Attribution Theory and use the crisis situation and the publics as the factors that help to determine when a crisis-response strategy is appropriate. }
}

@book{barthes1970,
  title     = "S/Z",
  author    = "Barthes, Roland",
  year      = 1970,
  publisher = "Éditions du Seuil",
  address   = "Paris",
  note      = "Translated by Richard Miller in 1974",
}

@ARTICLE{trust_and_distrust,

AUTHOR={Gefen, David  and Fresneda, Jorge E.  and Larsen, Kai R. },

TITLE={Trust and Distrust as Artifacts of Language: A Latent Semantic Approach to Studying Their Linguistic Correlates},

JOURNAL={Frontiers in Psychology},

VOLUME={11},

YEAR={2020},

URL={https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2020.00561},

DOI={10.3389/fpsyg.2020.00561},

ISSN={1664-1078},
}

@article{choosing_words_wisely,
  author = {Janet Coats and Kendall Moe},
  title = {Choose Your Words Wisely: The Role of Language in Media Trust},
  journal = {University of Florida College of Journalism and Communications},
  year = {2023},
  url = {https://www.jou.ufl.edu/insights/choose-your-words-wisely-the-role-of-language-in-media-trust/},
  note = {Originally published in the November 16 issue of InContext, a publication by Digital Content Next}
}

@inproceedings{text_classification_llms,
    title = "Text Classification via Large Language Models",
    author = "Sun, Xiaofei  and
      Li, Xiaoya  and
      Li, Jiwei  and
      Wu, Fei  and
      Guo, Shangwei  and
      Zhang, Tianwei  and
      Wang, Guoyin",
    editor = "Bouamor, Houda  and
      Pino, Juan  and
      Bali, Kalika",
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2023",
    month = dec,
    year = "2023",
    address = "Singapore",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-emnlp.603",
    doi = "10.18653/v1/2023.findings-emnlp.603",
    pages = "8990--9005",
    abstract = "Despite the remarkable success of large-scale Language Models (LLMs) such as GPT-3, their performances still significantly underperform fine-tuned models in the task of text classification.This is due to (1) the lack of reasoning ability in addressing complex linguistic phenomena (e.g., intensification, contrast, irony etc); (2) limited number of tokens allowed in in-context learning. In this paper, we introduce \textbf{C}lue \textbf{A}nd \textbf{R}easoning \textbf{P}rompting (CARP). CARP adopts a progressive reasoning strategy tailored to addressing the complex linguistic phenomena involved in text classification: CARP first prompts LLMs to find superficial clues (e.g., keywords, tones, semantic relations, references, etc), based on which a diagnostic reasoning process is induced for final decisions. To further address the limited-token issue, CARP uses a fine-tuned model on the supervised dataset for $k$NN demonstration search in the in-context learning, allowing the model to take the advantage of both LLM{'}s generalization ability and the task-specific evidence provided by the full labeled dataset. Remarkably, CARP yields new SOTA performances on 4 out of 5 widely-used text-classification benchmarks, 97.39 (+1.24) on SST-2, 96.40 (+0.72) on AGNews, 98.78 (+0.25) on R8 and 96.95 (+0.6) on R52, and a performance comparable to SOTA on MR (92.39 v.s. 93.3). More importantly, we find that CARP delivers impressive abilities on low-resource and domain-adaptation setups. Specifically, using 16 examples per class, CARP achieves comparable performances to supervised models with 1,024 examples per class.",
}

@inproceedings{sorato-etal-2021-using,
    title = "Using Word Embeddings to Quantify Ethnic Stereotypes in 12 years of {S}panish News",
    author = "Sorato, Danielly  and
      Zavala-Rojas, Diana  and
      del Carme Colominas Ventura, Maria",
    editor = "Rahimi, Afshin  and
      Lane, William  and
      Zuccon, Guido",
    booktitle = "Proceedings of the 19th Annual Workshop of the Australasian Language Technology Association",
    month = dec,
    year = "2021",
    address = "Online",
    publisher = "Australasian Language Technology Association",
    url = "https://aclanthology.org/2021.alta-1.4",
    pages = "34--46",
    abstract = "The current study provides a diachronic analysis of the stereotypical portrayals concerning seven of the most prominent foreign nationalities living in Spain in a Spanish news outlet. We use 12 years (2007-2018) of news articles to train word embedding models to quantify the association of such outgroups with drug use, prostitution, crimes, and poverty concepts. Then, we investigate the effects of sociopolitical variables on the computed bias series, such as the outgroup size in the host country and the rate of the population receiving unemployment benefits. Our findings indicate that the texts exhibit bias against foreign-born people, especially in the case of outgroups for which the country of origin has a lower Gross Domestic Product per capita (PPP) than Spain.",
}

@inproceedings{contextualized_word_embeddings,
author = {Thijs, Guusje and Trilling, Damian and Kroon, Anne C.},
title = {Contextualized Word Embeddings Expose Ethnic Biases in News},
year = {2024},
isbn = {9798400703348},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3614419.3643994},
doi = {10.1145/3614419.3643994},
abstract = {The web is a major source for news and information. Yet, news can perpetuate and amplify biases and stereotypes. Prior work has shown that training static word embeddings can expose such biases. In this short paper, we apply both a conventional Word2Vec approach as well as a more modern BERT-based approach to a large corpus of Dutch news. We demonstrate that both methods expose ethnic biases in the news corpus. We also show that the biases in the news corpus are considerably stronger than the biases in the transformer model itself.},
booktitle = {Proceedings of the 16th ACM Web Science Conference},
pages = {290–295},
numpages = {6},
keywords = {bias, contextualized word embeddings, news, static word embeddings, stereotypes, transformer},
location = {Stuttgart, Germany},
series = {WEBSCI '24}
}

@article{guilty_by_association,
author = {Anne C. Kroon and Damian Trilling and Tamara Raats},
title ={Guilty by Association: Using Word Embeddings to Measure Ethnic Stereotypes in News Coverage},

journal = {Journalism \& Mass Communication Quarterly},
volume = {98},
number = {2},
pages = {451-477},
year = {2021},
doi = {10.1177/1077699020932304},

URL = { 
    
        https://doi.org/10.1177/1077699020932304
    
    

},
eprint = { 
    
        https://doi.org/10.1177/1077699020932304
    
    

}
,
    abstract = { The current study provides a new level of empirical evidence for the nature of ethnic stereotypes in news content by drawing on a sample of more than 3 million Dutch news items. The study’s findings demonstrate that universally accepted dimensions of stereotype content (i.e., low-status and high-threat attributes) can be replicated in news media content across a diverse set of ingroup and outgroup categories. Representations of minorities in newspapers have become progressively remote from factual integration outcomes, and are therefore rather an artifact of news production processes than a true reflection of what is actually happening in society. }
}

@article{muller2023differential,
  author = {Philipp Müller and Chung-Hong Chan and Katharina Ludwig and Rainer Freudenthaler and Hartmut Wessler},
  title = {Differential Racism in the News: Using Semi-Supervised Machine Learning to Distinguish Explicit and Implicit Stigmatization of Ethnic and Religious Groups in Journalistic Discourse},
  journal = {Political Communication},
  volume = {40},
  number = {4},
  pages = {396--414},
  year = {2023},
  publisher = {Routledge},
  doi = {10.1080/10584609.2023.2193146}
}

@misc{change_it,
  title = {Corpus 7373},
  author = {{European Language Grid}},
  year = {2023},
  url = {https://live.european-language-grid.eu/catalogue/corpus/7373},
  note = {Accessed: 2024-10-02}
}

@misc{italianBertElectra,
  author       = {Stefan Schweter},
  title        = {Italian BERT-Electra models},
  year         = {2020},
  url          = {https://github.com/stefan-it/italian-bertelectra},
  note         = {Accessed: 2024-11-03}
}

@article{SHAP,
  author       = {Scott M. Lundberg and
                  Su{-}In Lee},
  title        = {A unified approach to interpreting model predictions},
  journal      = {CoRR},
  volume       = {abs/1705.07874},
  year         = {2017},
  url          = {http://arxiv.org/abs/1705.07874},
  eprinttype    = {arXiv},
  eprint       = {1705.07874},
  timestamp    = {Fri, 26 Nov 2021 16:33:36 +0100},
  biburl       = {https://dblp.org/rec/journals/corr/LundbergL17.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}

@article{migrations_in_italy,
  author = {Nese, Annalisa},
  title = {Migrations in Italy and Perceptions of Ethnic Threat},
  journal = {International Migration \& Integration},
  year = {2023},
  volume = {24},
  pages = {939–968},
  doi = {10.1007/s12134-022-00985-8},
  url = {https://doi.org/10.1007/s12134-022-00985-8},
  accepted = {2022-08-20},
  published = {2022-09-16},
  note = {Issue Date: September 2023}
}

@techreport{Papademetriou2016,
  author = {Papademetriou, Demetrios G. and Banulescu-Bogdan, Natalia},
  title = {Understanding and Addressing Public Anxiety About Immigration},
  institution = {Migration Policy Institute},
  year = {2016},
  type = {Council Statement},
  address = {Washington, DC},
  note = {Transatlantic Council on Migration - Council Statement, Rome, 2015},
  pages = {1--23}
}

@misc{ISTATMigrationData,
  author = {{Italian National Institute of Statistics (ISTAT)}},
  title = {International Migration Data},
  year = {Accessed 2024},
  url = {http://dati.istat.it/Index.aspx?QueryId=19675&lang=en},
  note = {Available online at ISTAT Data Portal}
}

@misc{iom_about_migration,
  author       = {{International Organization for Migration}},
  title        = {About Migration},
  year         = {2024},
  url          = {https://www.iom.int/about-migration},
  note         = {Accessed: 2024-11-05}
}



@inproceedings{demattei-etal-2020-changeit,
    author = {De Mattei, Lorenzo and Cafagna, Michele and Dell'Orletta, Felice and Nissim, Malvina and Gatt, Albert},
    title = {{CHANGE-IT @ EVALITA 2020}: Change Headlines, Adapt News, GEnerate},
    booktitle = {Proceedings of Seventh Evaluation Campaign of Natural Language Processing and Speech Tools for Italian. Final Workshop (EVALITA 2020)},
    editor = {Basile, Valerio and Croce, Danilo and Di Maro, Maria, and Passaro, Lucia C.},
    publisher = {CEUR.org},
    year = {2020},
    address = {Online}
}


@inproceedings{devlin-etal-2019-bert,
    title = "{BERT}: Pre-training of Deep Bidirectional Transformers for Language Understanding",
    author = "Devlin, Jacob  and
      Chang, Ming-Wei  and
      Lee, Kenton  and
      Toutanova, Kristina",
    booktitle = "Proceedings of the 2019 Conference of the North {A}merican Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers)",
    month = jun,
    year = "2019",
    address = "Minneapolis, Minnesota",
    publisher = "Association for Computational Linguistics",
    doi = "10.18653/v1/N19-1423",
    pages = "4171--4186",
}

@article{polarization,
author = {Petter Törnberg },
title = {How digital media drive affective polarization through partisan sorting},
journal = {Proceedings of the National Academy of Sciences},
volume = {119},
number = {42},
pages = {e2207159119},
year = {2022},
doi = {10.1073/pnas.2207159119},
URL = {https://www.pnas.org/doi/abs/10.1073/pnas.2207159119},
eprint = {https://www.pnas.org/doi/pdf/10.1073/pnas.2207159119},
abstract = {Recent years have seen a rapid rise of affective polarization, characterized by intense negative feelings between partisan groups. This represents a severe societal risk, threatening democratic institutions and constituting a metacrisis, reducing our capacity to respond to pressing societal challenges such as climate change, pandemics, or rising inequality. This paper provides a causal mechanism to explain this rise in polarization, by identifying how digital media may drive a sorting of differences, which has been linked to a breakdown of social cohesion and rising affective polarization. By outlining a potential causal\&nbsp;link between digital media and affective polarization, the paper suggests ways of designing digital media so as to reduce their negative consequences. Politics has in recent decades entered an era of intense polarization. Explanations have implicated digital media, with the so-called echo chamber remaining a dominant causal hypothesis despite growing challenge by empirical evidence. This paper suggests that this mounting evidence provides not only reason to reject the echo chamber hypothesis but also the foundation for an alternative causal mechanism. To propose such a mechanism, the paper draws on the literatures on affective polarization, digital media, and opinion dynamics. From the affective polarization literature, we follow the move from seeing polarization as diverging issue positions to rooted in sorting: an alignment of differences which is effectively dividing the electorate into two increasingly homogeneous megaparties. To explain the rise in sorting, the paper draws on opinion dynamics and digital media research to present a model which essentially turns the echo chamber on its head: it is not isolation from opposing views that drives polarization but precisely the fact that digital media bring us to interact outside our local bubble. When individuals interact locally, the outcome is a stable plural patchwork of cross-cutting conflicts. By encouraging nonlocal interaction, digital media drive an alignment of conflicts along partisan lines, thus effacing the counterbalancing effects of local heterogeneity. The result is polarization, even if individual interaction leads to convergence. The model thus suggests that digital media polarize through partisan sorting, creating a maelstrom in which more and more identities, beliefs, and cultural preferences become drawn into an all-encompassing societal division.}}

@article{us_versus_them,
author = {Julia M. Wondolleck, Barbara Gray and Todd Bryan},
title = {Us versus Them: How Identities and Characterizations Influence Conflict},
journal = {Environmental Practice},
volume = {5},
number = {3},
pages = {207--213},
year = {2003},
publisher = {Taylor \& Francis},
doi = {10.1017/S1466046603035592},
URL = { 
        https://doi.org/10.1017/S1466046603035592
},
eprint = { 
        https://doi.org/10.1017/S1466046603035592
}

}

@inbook{us_versus_them2, place={Cambridge}, title={Us versus Them: Domestic Support and Foreign Opposition in Media Coverage of the Iraq War Debate}, booktitle={Influence from Abroad: Foreign Voices, the Media, and U.S. Public Opinion}, publisher={Cambridge University Press}, author={Hayes, Danny and Guardino, Matt}, year={2013}, pages={17–50}} <div></div>

@article{racism_and_the_press,
 title     = {Racism and The Press},
 ISSN = {09579265, 14603624},
 URL = {http://www.jstor.org/stable/42887807},
 author = {Kenneth L. Hacker},
 journal = {Discourse & Society},
 number = {3},
 pages = {378--383},
 publisher = {Sage Publications, Ltd.},
 reviewed-author = {TEUN A. VAN DIJK and ROGER FOWLER},
 urldate = {2024-11-06},
 volume = {3},
 year = {1992}
}

@article{principles_of_critical_discourse,
  author    = {Teun A. van Dijk},
  title     = {Principles of Critical Discourse Analysis},
  journal   = {Discourse \& Society},
  volume    = {4},
  number    = {2},
  pages     = {249--283},
  year      = {1993},
  doi       = {10.1177/0957926593004002006},
}

@book{elite_discourse_and_racism,
  author    = {Teun A. van Dijk},
  title     = {Elite Discourse and Racism},
  publisher = {Sage Publications},
  address   = {London},
  year      = {1993},
}

@misc{treccani_immigrato,
  author       = {Treccani},
  title        = {Immigrato},
  year         = {n.d.},
  url          = {https://www.treccani.it/vocabolario/immigrato/},
  note         = {Accessed: 2024-11-06}
}



@article{tebano,
author = {Ventura, Francesco and Greco, Salvatore and Apiletti, Daniele and Cerquitelli, Tania},
title = {Trusting deep learning natural-language models via local and global explanations},
year = {2022},
issue_date = {Jul 2022},
publisher = {Springer-Verlag},
address = {Berlin, Heidelberg},
volume = {64},
number = {7},
issn = {0219-1377},
url = {https://doi.org/10.1007/s10115-022-01690-9},
doi = {10.1007/s10115-022-01690-9},
journal = {Knowl. Inf. Syst.},
month = jul,
pages = {1863–1907},
numpages = {45},
}


@article{nlpguard,
author = {Greco, Salvatore and Zhou, Ke and Capra, Licia and Cerquitelli, Tania and Quercia, Daniele},
title = {NLPGuard: A Framework for Mitigating the Use of Protected Attributes by NLP Classifiers},
year = {2024},
issue_date = {November 2024},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
volume = {8},
number = {CSCW2},
url = {https://doi.org/10.1145/3686924},
doi = {10.1145/3686924},
journal = {Proc. ACM Hum.-Comput. Interact.},
month = nov,
articleno = {385},
numpages = {25},
}

@INPROCEEDINGS{E-mimic,
  author={Attanasio, Giuseppe and Greco, Salvatore and La Quatra, Moreno and Cagliero, Luca and Tonti, Michela and Cerquitelli, Tania and Raus, Rachele},
  booktitle={2021 IEEE International Conference on Big Data (Big Data)}, 
  title={E-MIMIC: Empowering Multilingual Inclusive Communication}, 
  year={2021},
  volume={},
  number={},
  pages={4227-4234},
  doi={10.1109/BigData52589.2021.9671868}}


@InProceedings{inclusivelypaper,
author="La Quatra, Moreno
and Greco, Salvatore
and Cagliero, Luca
and Cerquitelli, Tania",
title="Inclusively: An AI-Based Assistant for Inclusive Writing",
booktitle="Machine Learning and Knowledge Discovery in Databases: Applied Data Science and Demo Track",
year="2023",
publisher="Springer Nature Switzerland",
address="Cham",
pages="361--365",
isbn="978-3-031-43430-3"
}


@inproceedings{10.1145/3397482.3450728,
author = {Qian, Kun and Danilevsky, Marina and Katsis, Yannis and Kawas, Ban and Oduor, Erick and Popa, Lucian and Li, Yunyao},
title = {XNLP: A Living Survey for XAI Research in Natural Language Processing},
year = {2021},
isbn = {9781450380188},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3397482.3450728},
doi = {10.1145/3397482.3450728},
booktitle = {26th International Conference on Intelligent User Interfaces - Companion},
pages = {78–80},
numpages = {3},
keywords = {natural language processing, interactive survey, Explainable AI},
location = {College Station, TX, USA},
series = {IUI '21 Companion}
}


@article{Guidotti:2018:SME:3271482.3236009,
 author = {Guidotti, Riccardo and Monreale, Anna and Ruggieri, Salvatore and Turini, Franco and Giannotti, Fosca and Pedreschi, Dino},
 title = {A Survey of Methods for Explaining Black Box Models},
 journal = {ACM Comput. Surv.},
 issue_date = {January 2019},
 volume = {51},
 number = {5},
 month = aug,
 year = {2018},
 issn = {0360-0300},
 pages = {93:1--93:42},
 articleno = {93},
 numpages = {42},
 doi = {10.1145/3236009},
 acmid = {3236009},
 publisher = {ACM},
 address = {New York, NY, USA},
} 


@inproceedings{danilevsky-etal-2020-survey,
    title = "A Survey of the State of Explainable {AI} for Natural Language Processing",
    author = "Danilevsky, Marina  and
      Qian, Kun  and
      Aharonov, Ranit  and
      Katsis, Yannis  and
      Kawas, Ban  and
      Sen, Prithviraj",
    month = dec,
    year = "2020",
    address = "Suzhou, China",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2020.aacl-main.46",
    pages = "447--459",
}


@article{shapley1953value,
  title={A value for n-person games},
  author={Shapley, Lloyd S},
  journal={Contributions to the Theory of Games},
  volume={2},
  number={28},
  pages={307--317},
  year={1953}
}


@article{Mor_Belinkov_Kimelfeld_2024, 
title={Accelerating the Global Aggregation of Local Explanations}, 
volume={38}, 
url={https://ojs.aaai.org/index.php/AAAI/article/view/29845}, 
DOI={10.1609/aaai.v38i17.29845}, 
year={2024}, 
month={Mar.}, 
pages={18807-18814} }

@article{ventura2023explaining,
  title={Explaining deep convolutional models by measuring the influence of interpretable features in image classification},
  author={Ventura, Francesco and Greco, Salvatore and Apiletti, Daniele and Cerquitelli, Tania},
  journal={Data Mining and Knowledge Discovery},
  pages={1--58},
  year={2023},
  publisher={Springer}
}
```

## Authors


- **Matteo Berta**, *Politecnico di Torino* 
- **Salvatore Greco**, *Politecnico di Torino*
- **Giuseppe Tipaldo**, *Politecnico di Torino* 
- **Tania Cerquitelli**, *Politecnico di Torino* 
