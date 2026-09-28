# Intelligent Question Answering System

An intelligent Question Answering platform combining Information Retrieval, Natural Language Processing and Deep Learning to extract answers from technical documents.

## 🎯 Project Overview

This project was developed as part of my Master's thesis in Computer Science, Big Data specialization.

The objective was to design an intelligent Question Answering system capable of helping operational users find answers to technical questions from a domain-specific knowledge corpus.

Instead of returning a list of documents like a traditional search engine, the system identifies the most relevant passage and extracts the answer directly from it.

## 🧠 Approach

The solution is organized into several main components:

1. Data collection and preparation
2. Text preprocessing and tokenization
3. Information Retrieval using BM25
4. Relevant passage selection
5. Answer extraction using BERT
6. Web application deployment
7. Communication between the user interface, backend services and database

### Pipeline

User Question
↓
Text Preprocessing
↓
BM25 Retrieval
↓
Most Relevant Passage
↓
BERT Question Answering Model
↓
Extracted Answer
↓
Web Application

## 🔎 Information Retrieval

The retrieval component uses **BM25Okapi** to rank documents/passages according to their relevance to the user's question.

The project also studied TF-IDF and compared it with BM25 during the information retrieval phase.

## 🤖 Question Answering Model

The answer extraction component is based on **BERT Base Uncased** using transfer learning.

The model receives:

* the user's question
* the selected passage

and predicts the beginning and the end positions of the answer within the passage.

The model was trained and evaluated using a combination of collected domain-specific question-answer pairs and the SQuAD dataset.

## 🧹 Data Processing

The preprocessing pipeline includes:

* Tokenization
* Stop-word removal
* Punctuation processing
* Text normalization
* Preparation of question/passage pairs

Approximately 1,500 domain-specific question-answer pairs were collected for the project, in addition to the SQuAD dataset.

The dataset was divided into training, validation and test subsets.

## 🏗️ Application Architecture

The deployed web application combines several technologies:

* **Python** for the NLP and Deep Learning components
* **BERT** for answer extraction
* **BM25Okapi** for information retrieval
* **TensorFlow / Keras**
* **Transformers**
* **Flask** for the Python backend
* **Node.js** for application/server communication
* **Socket.IO** for real-time communication
* **React.js** for the user interface
* **MongoDB** for application data storage

## 🖥️ Application

The application provides different functionalities including:

* User authentication
* Communication between users
* Intelligent Question Answering
* Expert intervention
* Modification/correction of generated answers

## 📊 Results and Limitations

The experiments showed that the system could correctly extract answers in several test cases.

The evaluation also highlighted limitations, particularly for:

* Long answers
* Questions with insufficient matching terms
* Cases where several terms appear repeatedly in a passage
* Limited domain-specific training data

One proposed improvement is to enrich the training dataset with more long-answer examples.

## 🚀 Future Improvements

Possible improvements identified during the project include:

* Increasing the amount of domain-specific training data
* Adding more long-answer examples
* Using Bi-Encoder and Cross-Encoder approaches for passage retrieval
* Adding speech recognition
* Developing a mobile version
* Improving answer extraction accuracy

## 🛠️ Technologies

`Python` `NLP` `Deep Learning` `BERT` `BM25` `TensorFlow` `Keras` `Transformers` `NLTK` `Flask` `Node.js` `Socket.IO` `React.js` `MongoDB`

## 🎓 Academic Project

**Master's Degree — Big Data**

Université des Sciences et de la Technologie Houari Boumediene (USTHB)

2022

Project developed as part of a Master's thesis.

## 👩‍💻 Author

**Mellissa Misraoui**

Business Intelligence Engineer | Data & Analytics

[LinkedIn](https://www.linkedin.com/)

[GitHub](https://github.com/MellissaZ)
