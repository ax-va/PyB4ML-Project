# PyB4ML
PyB4ML is a collection of algorithms and models written in Python 3.8 for probabilistic programming. The main focus of the package is on Bayesian reasoning by using Bayesian and/or Markov networks. 

The collection contains the following algorithms and models.

Factored-inference-related algorithms for probabilistic graphical models:
- Belief Propagation (BP) [B12] for efficient inference in trees (pb4ml/inference/factored/belief_propagation.py);
- Bucket Elimination (BE) [B12] for inference in loopy graphs or computing the joint probability distribution of several query variables (pb4ml/inference/factored/bucket_elimination.py);
- Greedy Bucket Elimination (GBE) combining Bucket Elimination with an elimination ordering pre-calculated by Greedy Ordering (pb4ml/inference/factored/greedy_elimination.py);
- Greedy Ordering (GO) [KF09] for greedy search for a near-optimal variable elimination ordering (pb4ml/inference/factored/greedy_ordering.py).

Academic probabilistic models in the factor graph representation:
- Bayesian network "Extended Student" [KF09] (pb4ml/models/academic/extended_student.py);
- Bayesian network "Student" [KF09] (pb4ml/models/academic/student.py);
- Markov network "Misconception" [KF09] (pb4ml/models/academic/misconception.py).

See in a tests folder how to use the algorithms. In a models folder, you can find how to create factor graph models.

© 2021-2022 Alexander Vasiliev

References:
[B12] David Barber, "Bayesian Reasoning and Machine Learning", Cambridge University Press, 2012;
[KF09] Daphne Koller and Nir Friedman, "Probabilistic Graphical Models: Principles and Techniques", The MIT Press, 2009
