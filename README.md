# Understanding-word2Vec
This repository discusses about TF-IDF,keras Tokensier,Gensim package.
                                                
                                                
                                                
                                                
                                                NATURAL LANGAUGE PROCESSING

                                                        CSE-4022
                                                        Slot:G2+TG2

 



                                                      PROJECT REPORT
                                               UNDERSTANDING WORD-TO-VECTORS

                                                        
                                                        Submitted by
                                                        Abishek k(16BCE0613)
                                                       Akash Ram(16BCE0554)



                                                        Submitted to
                                                     Prof.Sharmila banu k



TF-IDF[Term Frequency and Inverse Document Frequency]:          
                   
 

Tf-idf stands for Term frequency-inverse document frequency. The tf-idf weight is a weight often used in information retrieval and text mining. Variations of the tf-idf weighting scheme are often used by search engines in scoring and ranking a document’s relevance given a query. This weight is a statistical measure used to evaluate how important a word is to a document in a collection or corpus. The importance increases proportionally to the number of times a word appears in the document but is offset by the frequency of the word in the corpus (data-set).
tf-idf is a weighting scheme that assigns each term in a document a weight based on its term frequency (tf) and inverse document frequency (idf). The terms with higher weight scores are considered to be more important.
But TF-IDF does not see the context of the words or how the words in th sentences are formed. To solve this problem Word embeddings came into the picture.



Word embeddings:

A word embedding is an approach to provide a dense vector representation of words that capture something about their meaning. Word embedding are an improvement over simpler bag-of-word model word encoding schemes like word counts and frequencies that result in large and sparse vectors (mostly 0 values) that describe documents but not the meaning of the words. Word embedding work by using an algorithm to train a set of fixed-length dense and continuous-valued vectors based on a large corpus of text. Each word is represented by a point in the embedding space and these points are learned and moved around based on the words that surround the target word. It is defining a word by the company that it keeps that allows the word embedding to learn something about the meaning of words. The vector space representation of the words provides a projection where words with similar meanings are locally clustered within the space. The use of word embedding over other text representations is one of the key methods that has led to breakthrough performance with deep neural networks on problems like machine translation.



Gensim:

Gensim is package in python for natural language processing whic provideto build the word embedding for corpus,Gensim uses neural network to build the word embedding.Gensim uses to approach
Continous Bag of words(CBOW) and Skip-Gram. Both the methods are explained below.
The word embedding are the vetorised form of the vectors,which are actually the updated wieghts of all the input nodes in the deeo neural network.

How to set up gensim:
Type the following command in your anaconda prompt/Terminal

pip install --upgrade gensim

Word2vec is a group of related models that are used to produce word embeddings. These models are shallow, two-layer neural networks that are trained to reconstruct linguistic contexts of words. Word2vec takes as its input a large corpus of text and produces a vector space, typically of several hundred dimensions, with each unique word in the corpus being assigned a corresponding vector in the space. Word vectors are positioned in the vector space such that words that share common contexts in the corpus are located in close proximity to one another in the space.
Word2vec can utilize either of two model architectures to produce a distributed representation of words: continuous bag-of-words (CBOW) or continuous skip-gram. In the continuous bag-of-words architecture, the model predicts the current word from a window of surrounding context words. The order of context words does not influence prediction (bag-of-words assumption). In the continuous skip-gram architecture, the model uses the current word to predict the surrounding window of context words. The skip-gram architecture weighs nearby context words more heavily than more distant context words.CBOW is faster while skip-gram is slower but does a better job for infrequent words.


                                                                                                                             
                                                                                                                        

