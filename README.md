##LSA Lab

Your assignment for this week is to do LSA on a group of newsgroup posts from the newsgroup 'rec.sport.baseball.'  (Feel free to pick another newsgroup if you like, the list is here.  http://scikit-learn.org/stable/datasets/twenty_newsgroups.html) <br>  

1.  To get the newsgroup data, use this code: <br>

from sklearn.datasets import fetch_20newsgroups<br>
categories = ['rec.sport.baseball']<br>
dataset = fetch_20newsgroups(subset='all',shuffle=True, random_state=42, categories=categories)<br>
corpus = dataset.data<br>

2.  Next, you'll be adapting my LSA code for your problem.  This shouldn't be too hard, but please spend some time understanding what my code is doing.  <br>

3.  When you print the discovered concepts you'll probably find they don't make sense.  Consider adjusting the words in the stop word list to remove things like nntp, and people's names...<br>

4.  Once youre satisfied with your work, submit the link to your work