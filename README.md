multiclass_tagger
=================
This algorithim ingests a set of documents and splits it into a training and test set. 
Using associated metadata--right now in the form of a .csv--the algorithm learns to apply multiple tags to a body of text.
Also, this can extract relevant entities from the text including people, places, organizations, etc.

This requires Python 2.7, Sci-Kit learn, NLTK, and NumPy. The tagging algorithm is a linear support vector classifier against a
tfidf of n-grams (3) set up as a one vs. rest classifier.


How this works
===============
First, e-mail me and I'll send you the small set of documents as a .zip to run this. The algorithm doesn't work well with the test set for a variety of reasons including poor human tagging and over-tagging. However, I plan to test this on a much larger corpus to see if this can get better results. The entity extraction works ok though. documentagger.py & documentagger.ipynb are the same except the .pynb file will run with (http://ipython.org/notebook.html "iPython Notebook"). 
