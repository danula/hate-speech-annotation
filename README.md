# How Crowd Worker Factors Influence Subjective Annotations: A Study of Tagging Misogynistic Hate Speech in Tweets

This repository contains the expert-annotated hate speech dataset used for our study on annotating misogynistic hate speech. If you use our work in your research, please cite the following paper published at HCOMP 2023.

Hettiachchi, D., Holcombe-James, I., Livingstone, S., de Silva, A., Lease, M., Salim, F.D. and Sanderson, M. 2023. How Crowd Worker Factors Influence Subjective Annotations: A Study of Tagging Misogynistic Hate Speech in Tweets. Proceedings of the AAAI Conference on Human Computation and Crowdsourcing. 11, 1 (2023), 38-50. https://doi.org/10.1609/hcomp.v11i1.27546.

[BibTeX](hettiachchi2023.bib) | [PDF](https://www.danulahettiachchi.com/papers/hcomp23.pdf)


### Data Sampling and Annotation Process for Expert Labels

Hate speech is a broad term that refers to content targeting a person or group of people on the basis of their protected characteristics (e.g., race, ethnicity, national origin, disability, religious affiliation, sexual orientation, sex, gender identity). In this work, we consider annotation of sexist/misogynistic hate speech or hate speech directed at women on X (Twitter), a specific target group which has received far less attention than the study of hate speech annotation at large. A subject expert on anti-discrimination, and free speech and media law curated a list of 16 Twitter profiles (public figures) susceptible to sexist and misogynistic hate speech. We also contacted these individuals to obtain their consent to include their Twitter handle and relevant tweets in our research. We received positive responses from seven individuals, and collected the 5,000 most recent tweets for each profile. The selected individuals included authors, journalists, and activists from White, African-American, and Asian racial groups located in the US, UK, and Australia. Their profiles had 194,308 followers and 26,098 tweets on average. To avoid ambiguity on whether a tweet is directed at the specific person, we excluded any tweet that included more than one mentions (i.e., twitter handles in the tweet). Finally, we ordered by the tweet date and selected 2000 recent tweets for each profile.

#### Annotation Guidelines

Prior work has examined the utility of categories/factors, rating scales and comparative judgements when collecting hate speech annotations (Poletto et al. 2019). While rating scales are reported to be easy to use for annotators, they produce results which are difficult to understand and lead to poor overall performance in automated models. Comparative judgements such as best-worst-scale lead to better model outcomes. However, such ranking input scales are not suitable for our study design. Therefore, we collect categorical responses in our study. As we are interested in examining a specific type of hate speech, we use a tailored hate speech taxonomy instead of using generic and broader hate speech taxonomies (Salminen et al. 2018a) that have limited and incomplete label categories for misogynistic hate speech. Specifically, De Silva (2020) presents a functional theory of sex-based vilification, and Guest et al. (2021) propose a taxonomy, from which we adapt the following categories of hate speech:

- _Threats and Violent Abuse (TVA)_ are particularly serious examples of sex-based hate speech. It includes death and rape threats, as well as violent 'correctives' which tell the participant that they ‘deserve/need [to be violated]’
- _Sexualised Abuse (SA)_ reduces women to tools or objects for men’s sexual use or pleasure. It exposes women's sexuality in public, irrelevant, humiliating, and/or distressing ways.
- _Other Objectifying Speech (OOS)_ is speech that is less severe than threats and violent abuse or sexualised abuse, but that still treats women as for use by others (typically by men). It is speech that treats women as valuable only if they are attractive or useful to others.
- _Other Contemptuous Speech (OCS)_ communicates hatred, dislike, or disrespect for women that does not fit the categories described above. Other contemptuous speech typically treats women as inferior to men.
- _Other Hate Speech (OHS)_ is content that you think ought to be tagged as hate speech, but that does not fit into any of the above categories of sex-based hate speech. 

#### Annotation Process

Two authors (one woman, and one man) independently annotated the selected collection containing 14,000 tweets according to the annotator instructions and examples generated for the study. Afterwards, a third author, the expert mentioned earlier, reviewed the annotations, discussed any conflicts with the other two authors, and determined the final gold annotations. For the final dataset, we selected all the tweets tagged as hateful, and randomly selected a subset of tweets tagged as not hateful. 

While we treat these expert annotations as gold data to evaluate the agreement between annotators and experts, we acknowledge that expert annotations are not equivalent to ground truth due nuanced nature of defining hate speech (Fortuna, Soler, and Wanner 2020).

### Dataset

Our final [dataset](expert-annotations.csv) includes 140 tweets with the following expert-annotated labels. 

- Not Hate Speech - 90  
- Hate Speech - 50
  - Threats and Violent Abuse (TVA) - 4
  - Sexualised Abuse (SA) - 9
  - Other Objectifying Speech (OOS) - 7 
  - Other Contemptuous Speech (OCS) - 10
  - Other Hate Speech (OHS) - 20

Dataset fields
- [tweet_id](https://developer.x.com/en/docs/x-ids): You can use this ID to retrieve the original post from X (Twitter).
- annotation: Final hate speech label from the aforementioned annotation process.  
- tweet_mention: Username handle of the public figure mentioned in the post.

Please refer to the full [research paper](https://doi.org/10.1609/hcomp.v11i1.27546) for more details.

### Contact

For any questions and requests, please contact [Danula Hettiachchi](https://www.danulahettiachchi.com/).

- Danula Hettiachchi, RMIT University
- Indigo Holcombe-James, RMIT University
- Stephanie Livingstone, RMIT University
- Anjalee de Silva, The University of Melbourne
- Matthew Lease, University of Texas at Austin
- Flora D. Salim, University of New South Wales
- Mark Sanderson, RMIT University

