# Language_detector

In this project I use [European Parliament Proceedings Parallel Corpus](http://www.statmt.org/europarl/) which is a text dataset used for evaluating language detection engines. The 1.5GB corpus includes 21 languages spoken in EU. 

I test two different approaches, [bag of words](http://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.htm) and a [TfidfVectorizer](http://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) - Equivalent to CountVectorizer followed by TfidfTransformer. The last approach uses [n_gram](https://en.wikipedia.org/wiki/N-gram) which gives better results when tested on a different test set. 

The Europarl parallel corpus is extracted from the proceedings of the European Parliament. It includes versions in 21 European languages: Romanic (French, Italian, Spanish, Portuguese, Romanian), Germanic (English, Dutch, German, Danish, Swedish), Slavik (Bulgarian, Czech, Polish, Slovak, Slovene), Finni-Ugric (Finnish, Hungarian, Estonian), Baltic (Latvian, Lithuanian), and Greek.

All formats contain document $(<$CHAPTER id$>)$, speaker $(<$SPEAKER id name language$>)$, and paragraph $(<$P$>)$ mark-up on a separate line. The data is stored in one file per day, and in smaller units for newer data.
