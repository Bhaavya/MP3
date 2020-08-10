# MP3: Implementing the PLSA Algorithm
## DUE: Friday April 5 11:59pm

In this MP, you will implement the PLSA algorithm discussed in lectures [3.7](https://www.coursera.org/learn/text-mining/lecture/HKe8K/3-7-probabilistic-latent-semantic-analysis-plsa-part-1) and [3.8](https://www.coursera.org/learn/text-mining/lecture/GJyGG/3-8-probabilistic-latent-semantic-analysis-plsa-part-2) of the Text Mining Coursera course.
You are not required to implement the PLSA algorithm with a background model (we will run tests assuming the background model has not been implemented). You are provided with two data sets in the `data` folder: `test.txt` and `dblp.txt`. You can assume that each line is a separate document.

The `test.txt` data set contains 1000 lines. Each line is a document. The first 100 documents are labeled with the topic the document belongs to, either 0 (“Seattle”) or 1 (“Chicago”).  Each of the first 100 document is generated by sampling completely from the topic that is labelled (i.e., generated from one topic only). The rest 900 documents are generated from a mixture model of the topic “Seattle” and “Chicago”. Run your code to test if your EM algorithm returns reasonable results.

The `DBLP.txt` data set is made up of research paper abstracts from DBLP. Each line is a document. Make sure to test your code on the simpler data set `test.txt` before running it on `DBLP.txt`.

You are provided with a code skeleton `plsa.py`. Do not change anything in the `def __init__()` function. But feel free to change anything in the `main()` function to test your code.

Some suggested tips:
1.	Using matrices is strongly encouraged (writing nested `for-loops` for calculation is painful)
2.	Python libraries `numpy` and `scipy` are useful in matrix based calculations

You may find the following resources helpful:
1.	[Cheng’s note](http://sifaka.cs.uiuc.edu/czhai/pub/em-note.pdf) on the EM algorithm
2.	[Chase Geigle’s note](http://times.cs.uiuc.edu/course/598f16/notes/em-algorithm.pdf) on the EM algorithm, which includes a derivation of the EM algorithm (see section 4), and
3.	[Qiaozhu Mei’s note](http://times.cs.uiuc.edu/course/598f16/plsa-note.pdf) on the EM algorithm for PLSA, which includes a different derivation of the EM algorithm.


THIS MP IS CODING AND DEBUGGING HEAVY! PLEASE DON'T LEAVE IT TILL THE LAST MINUTE!