# dataset-for-system-acquiring-content-differences

This repository contains <nome dataset>, a new resource of newspaper articles and sentence-level similarity ratings among them.
The dataset has been collected in the context of a project aimed at identifying novel information in articles about an event with respect to a given reference (i.e., another news article about the same event).

The data have been manually collected and annotated via crowdsourcing.

The dataset contains 47 news articles, divided in 9 different news event, with each news event being represented by at least three articles. For each event, we record a *Reference Article* and at least two *Target Articles*.

We considered a list of events happened between 2020 and 2021 and reported by international newspapers (e.g., CNN, The Guardian, Al Jazeera English). For each article, we record the news it is sharing, the main topic of that news (e.g., politics, health etc.), the newspaper source, the date of publication and the URL.

In order to obtain sentence-level similarity ratings we performed a crowdsourcing experiment, in which raters where asked, given a pair of (*Target Sentence* - *Reference Setence*, to decide if the Target Sentence was *Similar* (SS), *Different* (DS), or *Very Different* (VDS) from the Reference Sentence. Each pair was labelled by 7 different annotators. In order to obtain a final label, we took the majority vote across annotations.

The repository includes three files:

- **articles.csv**: all the articles' texts and metadata about them
- **sentences.csv**: sentences extracted from each article and their metadata, including a sentence ID and the ID of the article they are originally from
- **sentence_pair_ratings**: the ratings and label obtained via crowdsourcing. Each row includes the ID of the Target Sentence, the ID of the Reference Sentence, the number of annotators that labelled them for a specific class, and the final label obtained via majority vote

Citation: TBD
