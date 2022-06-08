# dataset-for-system-acquiring-content-differences

This is a dataset consisting of 48 articles referring to 9 different news, with at least three articles for each news. All the articles regarding the same event and published on the same date (or similar) are comparable. For each news, we consider one article as the Reference Article, and the others as Target Articles.
For each article, we record the news it is sharing, the main topic of that news (e.g., politics, health etc.), the newspaper source, their publication date and their link. To simplify the collection process, we exploited CrowdTangle. We collected a list of events happened between 2020 and 2021 and obtained social media posts from Facebook pages of international newspapers (e.g., CNN, The Guardian, Al Jazeera English) with links to articles about the news. We then collected the news content directly from the newspaper website. In order to obtain ground-truth labels for sentences in the target articles, we performed a crowdsourcing experiment using Prolific. The annotators were presented with a list of ⟨target sentence - reference sentence⟩ pairs.
Annotators were asked to decide whether the target sentence was similar, different or very different from the reference sentence. Each pair was labelled by 7 different annotators. We considered the majority vote across annotations to obtain the gold label.
