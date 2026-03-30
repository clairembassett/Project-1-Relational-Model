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
### Data - [link to data](https://doi.org/10.1000/182)
### Pipeline - [analysis code](https://doi.org/10.1000/182)
### License - [MIT](LICENSE.md)
---
| Spec | Value |
|---|---|
| Name | Claire Bassett |
| NetID | qxm6fm |
| DOI | [https://doi.org/10.1000/182](https://doi.org/10.1000/182) |
| Press Release | [Data Science Project uses GFM to meet spec](https://github.com/UVADS/DS-4320/tree/main) |
| Data | [link to data](https://doi.org/10.1000/182) |
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

### Code

### Bias Identification

### Bias Mitigation

### Rationale

## Metadata
### Schema 

### Data

### Data Dictionary 

### Data Dictionary - Quantification of Uncertainty

##

### References
* GitHub Docs - Basic writing and formatting syntax [^1]
* GitHub Flavored Markdown Spec [^2]
* Markdown Creator's Blog [^3]


[^1]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
[^2]: https://github.github.com/gfm/
[^3]: https://daringfireball.net/projects/markdown/

### Terminology
| Term | appearance | code |
|:------|:------------:|---:|
|Superscript | 2<sup>nd</sup>| `<sup>nd</sup>`|
|Subscript | 2<sub>nd</sub>| `<sub>nd</sub>`|
|Inline code| `import numpy as np`| \` \` |
|Table justification | use colons in table header row | `:---` or `:---:` or `---:`|

### Background Summary
> [!TIP]
> Did you know you can make these call outs



### Code Highlighting

#### Formatting plain
```
import numpy as np

x = 137

for fruit in fruits:
    print fruit
```


#### Formatting with python
```python
import numpy as np

x = 137

for fruit in fruits:
    print fruit
```



