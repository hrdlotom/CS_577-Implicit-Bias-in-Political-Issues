CS 577 Project - Political Bias With One-Sided Nouns

CONTENTS OF THIS FILE
---------------------

* Introduction
* Content
* Installation
* FAQ


INTRODUCTION
---------------------
In this project, we focus on finding pairs of nouns that are synonymous and by themselves objective, but in certaincontexts convey opposing views on topics. We use different methods to capture context of the textand improve the selection of the noun pairs.


CONTENT
---------------------
- dataset dictionary
    raw export of ConvinceMe posts from https://nlds.soe.ucsc.edu/iac2 that weatures specific topics (abortion, ..) using SQL queries
- dataset processed
    processed datasets that are ready to be loaded and further processed based on specific needs of a given model
- models.ipynb
    this file consist of various models and combinations of these models that do binary classifiaction of posts - whether they belong to pro or against group. These models are for instance Neural Net featuring simmilar words or Linear Regression with sentiment analysis. More about our models is featured in our project report.
- ELMo_Model.ipynb
    this file is all about ELMo. It does both classification using ELMo embedding and 1-NN Consine simmilarity between pairs, and calculation of distances between nouns on demand.
- data_pre-processing.ipynb
    preprocessing of extracted data from dataset dictionary folder
- noun_significance_extraction.ipynb
    experimental file identifing related nouns using WordNet
- readme.txt
    file that you are reading just now :)
    
    
INSTALATION
---------------------
Some requirements - 
Anacoda
tenserflow in version 2.0.0 (pip install tensorflow==2.0.0)
other dependencies that can be installed using pip


FAQ
---------------------
How long does it take to run the code
- depends on your device. But be prepared to wait for hours. Especially ELMo model is relatively slow.