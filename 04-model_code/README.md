# tf-bpr

BPR implemetations in Tensorflow

Bayesian Personalized Ranking(BPR) is a learning algorithm for collaborative filtering first introduced in: BPR: Bayesian Personalized Ranking from Implicit Feedback. Steffen Rendle, Christoph Freudenthaler, Zeno Gantner and Lars Schmidt-Thieme, Proc. UAI 2009.  

All models are implemented in python using TensorFlow and best trained on a CPU*. s

## Files

Models are in the `models` folder an subclass the base `Model` class. We have various implementations:

* BPR: the baseline model from the Rendle paper
* VBPR: the visual baseline from the Runing, McAuley paper
* HBPR: our original work using heuristics from the data

There are various support files:

* corpus.py: manages the dataset
* sampling.py: implements the sampling strategy for BPR
* train.py: the main training routine

The main entry point of the training routine is managed by the `train.py` file w/ has a help document: `python train.py -h` . 



### Data

See notes about data in the project root README

## * Notes on GPU Applicability

https://github.com/hexiangnan/theano-BPR/issues/2

