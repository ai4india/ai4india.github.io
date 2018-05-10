# Multi-lingual Chatbot for an Indian Setting

## Aim

This project aims in building a chatbot capable of handling **multiple language inputs simutaneously** and respond with context. This is very essential in many sectors since the consumer base is very large when compared to the people available to serve them. This calls for automating certain part of monotonous work so that service people can cater to pressing essential activities.

Also considering that many people aren't comfortable in conversing in english, we need to integrate many indian languages (like Tamil, Hindi) so that poeple find it easy to communicate their problems.

## Possible Applications

* Banking
* Tourism
* Agriculture and Enviroment
* Any Other

## Datasets

No datasets available for specific for this project. We have identified prospective datasets.

* All India Radio - Agriculture related problems

## Pipe-line for the Project

This project can be divided into 3 main phases. They are mainly,

* Speech to Text Conversion

The input to this chabot is given via speech, as writting in multilingual sense is not straight forward. This phase also includes pre-processing   needed and gives word2vec embeddings that are used by the next phase.


* Embedding Mapping

This part of the project essentially maps different language embeddings in common domain so that it can be fed to the chatbot for further processing. An Encoder-Decoder Arcitecture or a simple linear transformation like *Ax* can be used. Even adversarial solutions are proposed in literature. 


* Training a Contextual Chatbot

This part of the project is the essential part where the chatbot is trained to respond to the user input. This can be done using a combinatorial algorithm (avoiding NLG altogether), using graph based search (depending on the application) or using NLG for some parts of the process and other algorithms for rest. This part essentially integrates all the previous part and comes out as a final product.
