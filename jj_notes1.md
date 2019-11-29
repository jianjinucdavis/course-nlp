##### 2019-11-28 
1. setup git for the course
2. read [lesson 0] (https://github.com/jianjinucdavis/course-nlp/blob/master/0-course-logistics.ipynb)
	- todo:
	- browse lesson 1
	- write a technical blog
	- revisit blog resources at the end of the course
3. read [lesson 1 - what is NLP] (https://github.com/jianjinucdavis/course-nlp/blob/master/1-what-is-nlp.ipynb)
	- Note
	- Application: part of speech tagging, named entity recognition, question answering, speech recognition, text-speech conversion, topic modeling, sentiment classification, language modeling, translation
	- Norvig vs. Chomsky: Modeling outcome vs. mechanisms
	- Manning (incorporating linguistic structure) vs. LeCun (Powerful neural architectures)
	- Interesting projects. Think of a project to do.
	- Textbook: focus on [speech and language processing] (https://web.stanford.edu/~jurafsky/slp3/)
	- todo: revisit tools and python libs when necessary

4. read [lesson 2 - topic modeling with NMF and SVD] (https://github.com/jianjinucdavis/course-nlp/blob/master/2-svd-nmf-topic-modeling.ipynb)
	- Topic modeling using matrix decomposition
	- Singular Value Decomposition (SVD) and Non-negative Matrix Factorization (NMF)
	- Preprocessing: removing stop words `sklearn.feature_extraction.stop_words`, Stemming and Lemmatization, spacy - offers alternative to universal stop words
	- stop words / stemming are context dependent. they may contains useful info for the problem to solve
	- Sub-word units: SentencePiece library from Google
	- Data processing: word counts (`sklearn.feature_extraction.text.CountVectorizer`)
	- Q: what does to_dense() do? how does it help? `vectors = vectorizer.fit_transform(newsgroups_train.data).todense()`
	- SVD: orthogonal matrix decomposition
	- todo: learn the math behind SVD
	- NMF: non-negative matrix factorization: factoring matrix into one skinny positive matrix and one short positive matrix
	- TF-IDF
```
	TF = (# occurrences of term t in document) / (# of words in documents)
	IDF = log(# of documents / # documents with term t in it)
```
	- TFIDF: what is reconstruction error?

