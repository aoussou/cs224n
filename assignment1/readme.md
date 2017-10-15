**NOTE:**

1. Code acceleration

It seems like it is possible to make `q3_run.py` run about *twice as fast* by passing `gradOut` of `skipgram` to `negSamplingCostAndGradient` in `q3_word2vec.py` instead of creating a numpy zeros array at every iteration of the context words. This is implemented in `q3_word2vec_fast.py`.

2. Question 3 results

In question 3, the results using the code in this repository are different than [the official solution](http://web.stanford.edu/class/cs224n/assignment1/assignment1_soln.pdf "the official solution"). A number of githubers get the same results ([Twice22](https://github.com/Twice22/CS224n-solutions/blob/master/Assigment%201/assignment1/q3_word_vectors.png), [izarov](https://github.com/izarov/cs224n/blob/master/assignment1/q3_word_vectors.png) ), but others get different ones ([kvfrans](https://github.com/kvfrans/cs224-solutions/blob/master/a1/q3_word_vectors.png), [kingtaurus](https://github.com/kingtaurus/cs224d/blob/master/assignment1/q3_word_vectors.png)). The results obtained using the code in this repo are similar to those of [yasiemir](https://github.com/yasiemir/cs224n/blob/master/assignment1/q3_word_vectors.png).

  Since, at least for the spring 2017 version of the course, the same seeds are used, it is not clear why the results differ. In any case, the accuracies attained in question 4 with the coefficients obtained using this code are reasonable (~30% when the GloVe pretrained coefficient yield about 37%).

3. `get_datasets.sh` link broken

The link given to download the pretrained weights for question 4 in the original `get_datasets.sh` file is broken.

At this time, the following link works: https://github.com/nate-parrott/squad/raw/master/data/glove.6B.50d.txt.zip

The get <code>get_datasets.sh</code> file of this repository has been modified accordingly.
