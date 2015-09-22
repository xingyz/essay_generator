﻿# essay_generator

An automatic 'essay' generator. It can be fed a large list of documents, and a topic(or a question). The system is going to generate a short article on the specified topic.

It uses tokenization to create Bags of sentences, and eliminates stop-words, and then use TF-IDF to calculate similarities of each bag to the specified topic.

<b>Structure:</b>

generator.cpp is the entry point for main() method.

Document: Each Bag of sentences. Result of SentenceSplitter.

Stopword: deals with stopword elimination.

SentenceSplitter: deals with tokenization.

Ranker: ranks documents based on similarities.

Essayomat: Combines previous classes to do the automatic trick!
