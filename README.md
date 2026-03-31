# DS 4320 Project 1 - TITLE!!!
### Executive Summary
This README now documents a GFM-focused DS 4320 project and includes completed project metadata (name, NetID, DOI, links, and license) plus a summary table for quick reference. It also contains a defined problem statement, rationale, references with footnotes, a terminology table, callout examples, and code highlighting examples to demonstrate practical GitHub Flavored Markdown usage.

<br>

<br>

---

### Name - Claire Bassett
### NetID - qxm6fm
### DOI - [https://doi.org/10.1000/182](https://doi.org/10.1000/182)
### Press Release
[**Data Science Project uses GFM to meet spec**](https://github.com/UVADS/DS-4320/tree/main)
### Data - [link to data](https://myuva-my.sharepoint.com/:f:/g/personal/qxm6fm_virginia_edu/IgCDzA5Osn1hRqLfM9T5a0zqAWiED4j0_D5ALxiBqLDtB84?e=ChlPrh)
### Pipeline - [analysis code](https://doi.org/10.1000/182)
### License - [MIT](LICENSE.md)
---
| Spec | Value |
|---|---|
| Name | Claire Bassett |
| NetID | qxm6fm |
| DOI | [https://doi.org/10.1000/182](https://doi.org/10.1000/182) |
| Press Release | [Data Science Project uses GFM to meet spec](https://github.com/UVADS/DS-4320/tree/main) |
| Data | [link to data](https://myuva-my.sharepoint.com/:f:/g/personal/qxm6fm_virginia_edu/IgCDzA5Osn1hRqLfM9T5a0zqAWiED4j0_D5ALxiBqLDtB84?e=ChlPrh) |
| Pipeline | [analysis code](https://doi.org/10.1000/182) |
| License | [MIT](LICENSE.md) |

---
<br>

<br>

## Problem Definition
### General and Specific Problem

* **General Problem:** Bot Detection
* **Specific Problem:** How can we predict the presence of bots by analyzing patterns in how misinformation is created and spread? Specifically, can features such as misleading content labels, text patterns, and engagement behavior from the Truth Seeker dataset be used as signals to improve bot detection?
  
### Rationale

This refinement goes beyond detecting bots but rather analyzing their role in spreading misinformation. By understanding how bots disseminate false information and the signals that may point to an automated account, researchers are able to identify key aspects of these bots. enables researchers to understand patterns in fake news creation. Thus allowing for effective migtifation strategies to protect users.

This approach goes beyond simply detecting bots, focusing instead on understanding their role in spreading misinformation. By analyzing how bots disseminate false or misleading content and identifying signals indicative of automated behavior, researchers can uncover patterns in fake news creation. These insights enable the development of targeted mitigation strategies to protect users and improve the integrity of news and information. 


### Motivation

The spread of misinformation on social media has become a growing concern, especially as automated accounts, or bots, can amplify false information quickly and at scale. These bots can influence public opinion, distort online discourse, and make it harder for users to distinguish between reliable and misleading content. Given the high level of polarization in the United States today, there is an increasing need for research on how fake accounts disseminate information and contribute to widening political divides.


### Press Release Headline and Link
[**INSERT **](https://github.com/UVADS/DS-4320/tree/main)

## Domain Exposition
### Terminology
| Term            | Meaning                                                                               |
|--------------------------|-------------------------------------------------------------------------------------------------------------|
| TruthSeeker2023          | Ground‑truth fake news analysis dataset of tweets linked to real/fake news statements from PolitiFact.     |
| statement                | Headline/claim of a news article or fact‑checked statement.                                                 |
| author                   | Person or entity who made the statement (PolitiFact subject).                                               |
| target                   | Ground‑truth truthfulness category for the statement (PolitiFact‑derived).                                  |                                          |
| Manual keywords          | Manually crafted keywords used to query Twitter for related tweets.                                         |
| tweet                    | Tweet text retrieved using the manual keywords and linked to a statement.                                   |
| 5 Label Majority Answer  | MTurk majority label for tweet–statement relation: Agree, Mostly Agree, Disagree, Mostly Disagree, Unrelated, or NO MAJORITY. |
| 3 Label Majority Answer  | MTurk majority label: Agree, Disagree, Unrelated, or NO MAJORITY.      
| Bots  | An automated account that can interact with other users  |
| Credibility | The perceived trustworthiness or reliability of an account or its content  |
| Influence | How a user affects engagement and the spread of content within a network  |

### Domain
This project lies at the intersection of politics and technology. It focuses on how bots, influence political discourse through the spread of misinformation. By analyzing patterns in fake news and online behavior, the project explores how technological systems can impact public opinion and political dynamics.
### Background Reading
### Summary of Readings

| Title | Brief Description | Link to File |
|------|------------------|--------------|
| AI and Misinformation | Explores how artificial intelligence has made it easy to mass-produce realistic fake images and news, leading to an increase in AI-enabled fake news sites in 2023 and amplifying the impact of misinformation on elections and conflicts. | [View Article](https://drive.google.com/file/d/1GnF-vaL7ZVtajucNA3lw22He_96Jzg30/view?usp=sharing) |
| Bots and Misinformation Spread on Social Media: Implications for COVID-19 | The article explores the prevalence of bots in spreading misinformation related to COVID-19. Additionally, it examines how this can influence public behavior and contribute to harmful outcomes such as reduced adherence to public safety measures. | [View Article](https://drive.google.com/file/d/1MVuG_PYsb5qzGVKq4v045qVN4ZX4GU4s/view?usp=sharing) |
| Towards Accurate Fake News Detection: Evaluating Machine Learning Approaches and Feature Selection Strategies | The research paper explores machine learning techniques for detecting fake news. It finds that Random Forest and Logistic Regression demonstrate stable, high performance across multiple feature selection methods. Recursive feature elimination and SelectKBest improve classification performance, while PCA reduces interpretability and overall performance. | [View Article](https://drive.google.com/file/d/1sIUP3ldJqsAghQcBOkgI2QxtwuJJyZVr/view?usp=sharing) |
| CIC TruthSeeker Dataset 2023 (TruthSeeker2023) | The article describes the TruthSeeker dataset, highlighting its contributions to current fake news datasets, including provenance and features. | [View Article](https://drive.google.com/file/d/1QKskKM6B6u6orWnFooaRA1Tvdb6Lw1JM/view?usp=sharing) |
| World-first social media wargame reveals how AI bots can swing elections | This article describes "Capture the Narrative," a social media wargame where students influence AI bots to affect election results. It demonstrates how easily fake news can be generated and how it impacts decision-making, underscoring the need for increased digital literacy. | [View Article](https://drive.google.com/file/d/1yN3S1a59QLGsjyaktTXaCxERb1EhChc7/view?usp=sharing) |

## Data Creation 

### Provenance
The TruthSeeker dataset was found by querying large datasets related to bot detection and the factor of fake news. It was selected due to its size and complexity. The physical compositon of the dataset was sourced by crawling Twitter for tweets related to real and fake news stories drawn from PolitiFact, using manually generated keywords fed into the Twitter API to collect over tweets linked to 700 real and 700 fake news items. Ground truth labels were then established through Amazon Mechanical Turk crowdsourcing, where workers rated how closely each tweet aligned with its associated news statement, with a majority agreement algorithm assigning final validity classifications.

To access the data this link was used: https://www.unb.ca//cic/datasets/truthseeker-2023.html . Then scroll down to download the dataset on the bottom of the page, entering information, downloading the zip file, and then downloading the "Features_For_Traditional_ML_Techniques" dataset.

### Code

| Code Title | Description | Link |
|-------|-------------|------|
| Loading | Code cleaning data, creating unique identifiers, and generating seperate parquet files from CSV. | [INSERT LINK](https://myuva-my.sharepoint.com/:u:/g/personal/qxm6fm_virginia_edu/IQC4h9mPQ0XPQLXMnoB4yJBgAZQjTFWv8w55AuXFZ4ZpXf4?e=cZqAc6) |
| Pipeline  | A table containing 134,198 tweet records from the TruthSeeker dataset, including the linguistic characteristics of each tweet such as punctuation and word classification.  | [lexical.parquet](https://myuva-my.sharepoint.com/:u:/g/personal/qxm6fm_virginia_edu/IQD-UPFOSB5OTaKMdoFk-BqCAQVtBeNMIQkpup2Z8Ty4UHM?e=mr8h1Q) |



### Bias Identification
Bias was likely introduced to this dataset, as the tweets were collected using manually generated keywords, meaning keywords not anticipated by the researchers were excluded entirely. Additionally, only targeting twitter could limit certain content as the demographic of twitter skews towards younger users, therefore, fake news/bot accounts would be targeted at this population. Furthermore, the dataset lacks unique user identifiers meaning the same user's bot and credibility scores may appear across several rows if they posted more than one tweet in the dataset, thus, distorting the true distribution of user-level signals. 

### Bias Mitigation
By using MTurk annotations, bias is partially mitigated by requiring consensus across multiple independent raters rather than relying on a single judgment. Additionally, the large sample size of 134,198 tweets helps dilute the impact of uneven keyword coverage and repeated user records, reducing the influence of any single skewed observation on the overall dataset.

### Rationale
The manual keyword generation directly shaped the corpus of the dataset, introducing uncertainty about the coverage of tweet collection. However, this approach made data generation feasible and ensured tweets were relevant to common real and fake news topics. The exclusion of unique user identifiers, while limiting user-level analysis, was likely an ethical decision used to protect user privacy in accordance with the platforms terms of service and data protection standards. Additionally, restricting the collection to Twitter, while a limitation in terms of generalizability, provided a consistent structure with standardized metadata fields, making the data more usable. 

## Metadata
### Schema 

### Tables 
| Table | Description | Link |
|-------|-------------|------|
| Text | A table containing 134,198 tweet records from the TruthSeeker dataset, describing the text features of tweets including information on word make-up and the percentage of tags in the text. | [text.parquet](https://myuva-my.sharepoint.com/:u:/g/personal/qxm6fm_virginia_edu/IQC4h9mPQ0XPQLXMnoB4yJBgAZQjTFWv8w55AuXFZ4ZpXf4?e=cZqAc6) |
| Lexical | A table containing 134,198 tweet records from the TruthSeeker dataset, including the linguistic characteristics of each tweet such as punctuation and word classification.  | [lexical.parquet](https://myuva-my.sharepoint.com/:u:/g/personal/qxm6fm_virginia_edu/IQD-UPFOSB5OTaKMdoFk-BqCAQVtBeNMIQkpup2Z8Ty4UHM?e=mr8h1Q) |
| Meta-data | A table containing 134,198 tweet records made from the TruthSeeker dataset, including information on the user who posted the tweet, including the size of following and interaction totals on posts. | [metadata.parquet](https://myuva-my.sharepoint.com/:u:/g/personal/qxm6fm_virginia_edu/IQBvurMzcYT6Qa8fpABqehkxASOv1qsr1GLJADMs3oPsg_U?e=J2r12y) |
| Scores |A table containing 134,198 tweet records derived from the TruthSeeker dataset, capturing credibility, influence, and bot activity scores alongside fake news labels. | [scores.parquet](https://myuva-my.sharepoint.com/:u:/g/personal/qxm6fm_virginia_edu/IQDatITsN_HlQ5DUvow7xuI0AS76HvPFEMi-wZ_fZ30KiL4?e=mGfknG) |

### Data Dictionary 


| name                     | data type | description                                                                 | example |
|--------------------------|----------|-----------------------------------------------------------------------------|---------|
| unique_count             | int64    | number of unique, complex words                                            | 5 |
| total_count              | int64    | total number of words                                                      | 6 |
| ORG_percent              | float64  | Percent of text including spaCy ORG tags                                   | 0.333333 |
| NORP_percent             | float64  | Percent of text including spaCy NORP tags                                  | 0.166667 |
| GPE_percent              | float64  | Percent of text including spaCy GPE tags                                   | 0.166667 |
| PERSON_percent           | float64  | Percent of text including spaCy PERSON tags                                | 0.166667 |
| MONEY_percent            | float64  | Percent of text including spaCy MONEY tags                                 | 0.166667 |
| DATA_percent             | float64  | Percent of text including spaCy DATA tags                                  | 0.0 |
| CARDINAL_percent         | float64  | Percent of text including spaCy CARDINAL tags                              | 0.0 |
| PERCENT_percent          | float64  | Percent of text including spaCy PERCENT tags                               | 0.0 |
| ORDINAL_percent          | float64  | Percent of text including spaCy ORDINAL tags                               | 0.0 |
| FAC_percent              | float64  | Percent of text including spaCy FAC tags                                   | 0.0 |
| LAW_percent              | float64  | Percent of text including spaCy LAW tags                                   | 0.0 |
| PRODUCT_percent          | float64  | Percent of text including spaCy PRODUCT tags                               | 0.0 |
| EVENT_percent            | float64  | Percent of text including spaCy EVENT tags                                 | 0.0 |
| TIME_percent             | float64  | Percent of text including spaCy TIME tags                                  | 0.0 |
| LOC_percent              | float64  | Percent of text including spaCy LOC tags                                   | 0.0 |
| WORK_OF_ART_percent      | float64  | Percent of text including spaCy WOA tags                                   | 0.0 |
| QUANTITY_percent         | float64  | Percent of text including spaCy QUANTITY tags                              | 0.0 |
| LANGUAGE_percent         | float64  | Percent of text including spaCy LANGUAGE tags                              | 0.0 |
| Max Word                 | int64    | Length of the longest word in the sentence                                 | 14 |
| Min Word                 | int64    | Length of the shortest word in the sentence                                | 1 |
| Avg Word Length          | float64  | Average length of words in the sentence                                    | 5.47619 |
| present_verb             | int64    | Number of present tense verbs                                              | 1 |
| past_verb                | int64    | Number of past tense verbs                                                 | 1 |
| adjectives               | int64    | Number of adjectives                                                       | 1 |
| pronouns                 | int64    | Number of pronouns                                                         | 1 |
| TO’s                     | int64    | Number of to usages                                                        | 0 |
| determiners              | int64    | Number of determiners                                                      | 0 |
| conjunctions             | int64    | Number of conjunctions                                                     | 0 |
| dots                     | int64    | Number of (.) used                                                         | 5 |
| exclamations             | int64    | Number of (!) used                                                         | 0 |
| question                 | int64    | Number of (?) used                                                         | 1 |
| ampersand                | int64    | Number of (&) used                                                         | 0 |
| capitals                 | int64    | Number of capitalized letters                                              | 33 |
| digits                   | int64    | Number of digits (0-9) used                                                | 3 |
| long_word_freq           | int64    | Number of long words                                                       | 5 |
| short_word_freq          | int64    | Number of short words                                                      | 19 |
| followers_count          | float64  | Number of followers                                                       | 4262.0 |
| friends_count            | float64  | Number of friends                                                         | 3619.0 |
| favourites_count         | float64  | Number of favourites across all tweets                                    | 34945.0 |
| statuses_count           | float64  | Number of tweets                                                          | 16423.0 |
| listed_count             | float64  | Number of tweets the user has in lists                                    | 44.0 |
| mentions                 | float64  | Number of times the user was mentioned                                    | 1.0 |
| replies                  | float64  | Number of replies the user has                                            | 1.0 |
| retweets                 | float64  | Number of retweets the user has                                           | 3.0 |
| favourites               | float64  | Number of favourites the user has                                         | 10.0 |
| hashtags                 | float64  | Number of hashtags (#) the user has used                                  | 0.0 |
| URLs                     | float64  | whether the user has a provided a url in relation to their profile        | 1.0 |
| quotes                   | float64  | Number of times the user has been quote tweeted                           | 1.0 |
| BotScoreBinary           | float64  | Binary score whether the user is considered a bot or not                  | 0.0 |
| cred                     | float64  | Credibility score                                                         | 0.540794 |
| normalized_influence     | float64  | Influence score the user has, normalized                                  | 0.104602 |
| majority_target          | bool     | Truth value of the tweet                                                  | True |
| statement                | object   | Headline of a news article                                                | End of eviction moratorium means millions could lose housing |
| BinaryNumTarget          | float64  | Binary representation of truth value (1 = True / 0 = False)               | 1.0 |
| tweet                    | object   | Twitter post text                                                         | @POTUS Biden Blunders...what did I miss? |


### Data Dictionary - Quantification of Uncertainty

| Field Name | Data Type | Min | Max | Mean | Std Dev | Null/Missing |
|-----------|-----------|-----|-----|------|---------|--------------|
| Unnamed: 0 | int64 | 0.0 | 1.341970e+05 | 67098.500000 | 38739.770050 | 0 |
| BinaryNumTarget | float64 | 0.0 | 1.000000e+00 | 0.513644 | 0.499816 | 0 |
| followers_count | float64 | 0.0 | 1.306019e+08 | 11293.082103 | 437497.073676 | 0 |
| friends_count | float64 | 0.0 | 5.869010e+05 | 1893.454455 | 6997.695671 | 0 |
| favourites_count | float64 | 0.0 | 1.765080e+06 | 32981.233878 | 68780.210325 | 0 |
| statuses_count | float64 | 1.0 | 2.958918e+06 | 34195.761449 | 75101.195265 | 0 |
| listed_count | float64 | 0.0 | 2.221930e+05 | 73.300198 | 1083.274277 | 0 |
| following | float64 | 0.0 | 0.0 | 0.0 | 0.0 | 0 |
| BotScore | float64 | 0.0 | 1.0 | 0.059106 | 0.167819 | 0 |
| BotScoreBinary | float64 | 0.0 | 1.0 | 0.032355 | 0.176942 | 0 |
| cred | float64 | 0.0 | 1.0 | 0.405852 | 0.239223 | 0 |
| normalize_influence | float64 | 0.0 | 2.086063e-01 | 0.077665 | 0.026184 | 0 |
| mentions | float64 | 0.0 | 12.0 | 1.388918 | 1.471604 | 0 |
| quotes | float64 | 0.0 | 5913.0 | 0.573406 | 28.436726 | 0 |
| replies | float64 | 0.0 | 42068.0 | 1.914201 | 122.041183 | 0 |
| retweets | float64 | 0.0 | 126062.0 | 6.674354 | 406.542579 | 0 |
| favourites | float64 | 0.0 | 460320.0 | 27.572386 | 1831.425703 | 0 |
| hashtags | float64 | 0.0 | 12.0 | 0.104726 | 0.458687 | 0 |
| URLs | float64 | 0.0 | 1.0 | 0.737701 | 0.439886 | 0 |
| unique_count | int64 | 0.0 | 9.0 | 2.365624 | 1.351617 | 0 |
| total_count | int64 | 0.0 | 32.0 | 3.441229 | 2.479373 | 0 |
| ORG_percentage | float64 | 0.0 | 1.0 | 0.199964 | 0.276376 | 0 |
| NORP_percentage | float64 | 0.0 | 1.0 | 0.067412 | 0.165502 | 0 |
| GPE_percentage | float64 | 0.0 | 1.0 | 0.136151 | 0.242561 | 0 |
| PERSON_percentage | float64 | 0.0 | 1.0 | 0.221930 | 0.298133 | 0 |
| MONEY_percentage | float64 | 0.0 | 1.0 | 0.029525 | 0.106880 | 0 |
| DATE_percentage | float64 | 0.0 | 1.0 | 0.102339 | 0.206059 | 0 |
| CARDINAL_percentage | float64 | 0.0 | 1.0 | 0.091104 | 0.190366 | 0 |
| PERCENT_percentage | float64 | 0.0 | 1.0 | 0.030638 | 0.116949 | 0 |
| ORDINAL_percentage | float64 | 0.0 | 1.0 | 0.012432 | 0.070884 | 0 |
| FAC_percentage | float64 | 0.0 | 1.0 | 0.003352 | 0.037525 | 0 |
| LAW_percentage | float64 | 0.0 | 1.0 | 0.005265 | 0.048690 | 0 |
| PRODUCT_percentage | float64 | 0.0 | 1.0 | 0.006839 | 0.053513 | 0 |
| EVENT_percentage | float64 | 0.0 | 1.0 | 0.002607 | 0.032400 | 0 |
| TIME_percentage | float64 | 0.0 | 1.0 | 0.005662 | 0.046830 | 0 |
| LOC_percentage | float64 | 0.0 | 1.0 | 0.009771 | 0.070224 | 0 |
| WORK_OF_ART_percentage | float64 | 0.0 | 1.0 | 0.008517 | 0.062580 | 0 |
| QUANTITY_percentage | float64 | 0.0 | 1.0 | 0.002396 | 0.030757 | 0 |
| LANGUAGE_percentage | float64 | 0.0 | 1.0 | 0.001011 | 0.019590 | 0 |
| Word count | int64 | 0.0 | 110.0 | 35.077691 | 13.604442 | 0 |
| Max word length | int64 | 0.0 | 145.0 | 13.062043 | 3.044782 | 0 |
| Min word length | int64 | 1.0 | 1000.0 | 1.399857 | 2.795407 | 0 |
| Average word length | float64 | -1.0 | 88.0 | 5.056648 | 0.825737 | 0 |
| present_verbs | int64 | 0.0 | 16.0 | 2.452354 | 2.049247 | 0 |
| past_verbs | int64 | 0.0 | 15.0 | 1.812210 | 1.736990 | 0 |
| adjectives | int64 | 0.0 | 17.0 | 3.034308 | 2.012125 | 0 |
| adverbs | int64 | 0.0 | 12.0 | 1.575873 | 1.546382 | 0 |
| adpositions | int64 | 0.0 | 14.0 | 3.619644 | 2.195625 | 0 |
| pronouns | int64 | 0.0 | 14.0 | 1.495820 | 1.639470 | 0 |
| TOs | int64 | 0.0 | 8.0 | 0.788626 | 0.961242 | 0 |
| determiners | int64 | 0.0 | 5.0 | 0.135583 | 0.379235 | 0 |
| conjunctions | int64 | 0.0 | 13.0 | 1.003495 | 1.086844 | 0 |
| dots | int64 | 0.0 | 50.0 | 2.366116 | 2.140459 | 0 |
| exclamation | int64 | 0.0 | 66.0 | 0.259408 | 0.903957 | 0 |
| questions | int64 | 0.0 | 43.0 | 0.307151 | 0.774367 | 0 |
| ampersand | int64 | 0.0 | 13.0 | 0.121537 | 0.453865 | 0 |
| capitals | int64 | 0.0 | 250.0 | 12.831905 | 15.557524 | 0 |
| digits | int64 | 0.0 | 138.0 | 3.559494 | 6.674458 | 0 |
| long_word_freq | int64 | 0.0 | 47.0 | 2.249557 | 2.912136 | 0 |
| short_word_freq | int64 | 0.0 | 164.0 | 21.438658 | 9.625147 | 0 |


