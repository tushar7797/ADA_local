# ADA_local
Title : Analysis of the people's popularity and reason for its change during the time

Abstract:  With this dataset, we can get the popularity of a person by watching his number of quotations and the number of occurrences. After having identified the popularity of the people, we can determine why certain person loses or increases his populary during the time. For instance, discovering what event makes a person famous according to the quotations he made last year, and what event made lose popularity. We could analyze the impact on the popularity when a president finish his term or when he begins his term. Or for example to infer when something append (for example: Donald Trump became president) just looking at his popularity variation. So watching the poplarity can give us a lot of informations.

Research Questions: (A list of research questions you would like to address during the project)
Discribing the data with the popular speaker and the urls(news vendor) that provided his statesment. To find the connection with the person to the news vendor with the purpose to investigate the people's popularity related to the vendors.

Proposed additional datasets (if any): (List the additional dataset(s) you want to use (if any), and some ideas on how you expect to get, manage, process, and enrich it/them. Show us that you’ve read the docs and some examples, and that you have a clear idea on what to expect. Discuss data size and format if relevant. It is your responsibility to check that what you propose is feasible.)

## Datasets
- Quotebank data from 2015 to 2020
- Wikidata with speaker informations
- Wikidata QIDs with labels and description

### How we manage the data
For the Quotebank data, we load directly with the help of pandas without unpack the files. We load with chunksize because the data is too big to fit in memory. So we need to handle the data by batch and merge the results (by adding in a list and concatenate this list of results to get the results dataframe). For the Wikidata with speaker information and the wikidata QIDs with labels and description datasets, we directly load all the data because there are much smaller than the first one. We merge these two datasets to get the speaker informations directly (without to look the QIDs in the wikidata QIDs dataset). The merge is done in `parse_speaker_attributes.ipynb`.

## Methods : 
data analysis with python and NLP


## Proposed timeline :
- Milestone P2, 12 Nov 2021
- Week 9
- Week 10
- Week 11
- Week 12
- Week 13
- Milestone P3, 17 Dec 2021

## Organization within the team: 

Questions for TAs (optional): 
