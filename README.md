# 2019 Deep geometric learning workshop @ IPAM, UCLA
_emphasized parts_ are Chan's comments.

## Links
* http://www.ipam.ucla.edu/programs/workshops/workshop-iv-deep-geometric-learning-of-big-data-and-applications
* [schedule & video](http://www.ipam.ucla.edu/programs/workshops/workshop-iv-deep-geometric-learning-of-big-data-and-applications/?tab=schedule)

## Szlam
* script + ML -> pure ML for Mincraft bots
* ML _components_
* neural _semantic parser_
  * ![2019-05-20 09.49.07](photos/2019-05-20%2009.49.07.jpg)
  * natural language -> programmning language
  * SentenceRec by Dong & Lapata, 2016

## Chintala
* forward autodiff: time O(n) <- time-space tradeoff -> backworkd autodiff: space O(n)
* PyTorch Geometric
  * includes over 60 graph kernel benchmark datasets
  * point clouds to a graph by generating a nearest neighbor graph
    * _any better way than using nearest neighbors to construct a graph from a point cloud?_
    
## Sulam
* ```x = D \cdot y```
  * ```x```: data
  * ```D```: pre-built dictionary of reps
  * ```y```: sparse representation
  
## Pollefeys
* Energy-based 3d semantic segmantation

## Jalali
* high-throughput, low-latency opto-electric system to classify cells in blood (cytometry) and detect surface proteins of cancer cells by scattering laser
* time-strech microscopy

## Goldstein
* data poisoining
* in a high-dimensional space, \epsilon-enighborhood can be very large
* instead of using ImageNet for a high-dim input, use enlarged MNIST.
* _how an adversarial training changes a classifier?_
  * _enforce disentanglement?_
* https://arxiv.org/abs/1809.02104
* build "I don't know" class to avoid this problem.

## Zhang
* cross-entropy decision boundary has poor margin, compared to SVM.

## Lederman
* reconstruct a molecule from various 2d projections (or crosssections)
* has a good forward model.

## Bresson
* graph auto-encoder
  * encoding is easy; decoding is more challenging.
  * graph to vector to graph
    * _using a vector to represent a graph is a step forward from a single scalar statistic, but maybe a concatenation of scalars are of the same or better capacity?_
* Information, Computation, Optimization: Connecting the Dots in the Traveling Salesman Problem
  * https://www.youtube.com/watch?v=q8nQTNvCrjE
* Operational research

## Pirsiavash
* Self-supervised
  * _generate_ annotations
  * pretrain using pseudotask, which is a self-supervied part, then do transfer learning with actual labeled dataset.
* distillation from one network to another with a different architecture.
  * _if we can transfer from human-engineered features, treating them as a black box, to a neural network, can we do the oppoisite to "extract knowledge" from a neural network?_
