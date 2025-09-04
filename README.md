# O. Henry Short Stories Analysis

[Research Question and Background]

“Do O. Henry’s characters reflect stereotypes of early 20th-century America?” This
question is very important because it helps us understand how literary works reflect and
shape social perceptions. The early 20th century was a significant period of social change
and immigration in the United States, during which stereotypes played a key role in
shaping the public’s understanding of different groups. By analyzing O. Henry’s
characters, we can not only explore how literature reflects the social and cultural context
of the time but also gain deeper insight into how stereotypes are propagated through
literature, influencing people’s views on identity and social class. This has important
implications for literary studies, social history, and cultural research.

[Data Source]

I selected 25 of O. Henry’s more well-known short stories and converted them into txt
files, which I stored in a corpus for analysis.

[Method 1 - Named Entity Recognition]

In this method, I used SpaCy’s named entity recognition to find all characters in the O.
Henry stories. Then I collected adjectives that appear in the same sentence as each
character. I focused on a list of adjectives that are related to social stereotypes common in
early 20th-century America, such as “greedy,” “lazy,” “honest,” and “poor.” By counting
how often these stereotype-related adjectives describe each character, I was able to
measure how much O. Henry’s characters reflect these social stereotypes.
The results show that some characters are described using adjectives connected to
common stereotypes. For example, Andy is called “honest,” David is described as “lazy”
and “poor,” and Sudie is called “greedy.” This suggests that O. Henry’s characters do
reflect a little social stereotypes of his time. This method offers a clear way to connect the
language used in the stories with the social ideas about people in early 20th-century
America, helping us understand how literature can reflect cultural views.

[Method 2 - Word2Vec]

In this method, I used the Word2Vec model to train on the complete texts of O. Henry,
aiming to find words that were semantically closest to preset stereotype keywords. First,
SpaCy was used to split the texts into sentences and tokens, and then these data were
used to train the Word2Vec model to obtain vector representations of words. Next, by
calculating the similarity between the keywords and other words, the contextual
associations related to the stereotypes were identified.
The results showed that many words with high similarity to some keywords were not
clearly related to the stereotypes. For example, the words near "lazy" were mostly
unrelated nouns or adverbs; the words related to "kind" were mostly function words; and
"greedy" was sometimes associated with proper names. This indicated that the semantic
context of stereotype words in the texts was complex, and stereotypes were not expressed
by simply clustering certain words, but were implicitly conveyed through diverse
contexts.

[Method 3 - LDA Topic Modeling]

In the third method, I used the topic model to analyze the themes in the complete works
of O. Henry. First, SpaCy was applied to preprocess the text by splitting it into sentences,
performing lemmatization, and removing stop words, which produced a dictionary and
the corresponding corpus. Then, based on this corpus, an LDA model with five topics
was trained to automatically identify the underlying topic distributions and keywords in
the text. This approach allowed for grasping the overall thematic structure of the text,
rather than focusing only on individual words or sentences.
The results showed that the five extracted topics mainly consisted of high-frequency
everyday words and narrative-related terms such as “say,” “man,” “look,” and “go,”
lacking distinctive words that clearly reflect social stereotypes. This indicates that in O.
Henry’s works, stereotypes do not appear as concentrated, independent themes but are
dispersed and implicitly embedded within ordinary narratives. This method provided a
macro-level perspective for understanding the overall semantic environment of the text.
