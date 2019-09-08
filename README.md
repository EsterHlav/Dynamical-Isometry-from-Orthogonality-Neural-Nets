# Dynamical Isometry as A Consequence of Weight Orthogonality in Neural Networks
## Impact of Orthogonal Initialization in Deep Learning
#### Ester Hlav, 2019

How does orthogonal initialization of weight matrices help improve the training of neural networks? What happens, if we further impose orthogonality during training? In this project, we research the effect of dynamical isometry and its positive impact on the convergence during training.

**What is dynamical isometry?** <br/>
Dynamical Isometry happens when the singular values of the input-output Jacobian for weight matrixes equal one. When the Jacobian *J* is well-conditioned, *i.e.* its eigenvalues are equal to one, then *J* is a norm-preserving-mapping, the mean of the Spectral density of *J* becomes one and dynamical isometry is reached. When a neural network achieves dynamical isometry, the gradient avoids the chaotic (exploding gradient) as well as ordered (vanishing gradient) zone, which triggers better and faster convergence.

![](https://github.com/EsterHlav/Dynamical-Isometry-from-Orthogonality-Neural-Nets/ordered_chaotic.png)

**Research Questions** <br/>
Effect of *Orthogonal Initialization* on: <br/>
A) Vanishing and Exploding Gradient <br/>
B) Difference of Speed of Convergence between Deep and Shallow Neural Networks <br/>
C) Accuracy of Non-Linear Neural Networks with vs without Dynamic Isometry


Effect of *Orthogonal Regularization*:<br/>
D) Can excessive orthogonality constraint (*i.e.* hard regularization) hurt performance?<br/>
E) Can specific conditions (*e.g.* depth) enforce orthogonality in a more beneficial way than others?

While the first part of the project researched the mathematical consequences of dynamical isometry, in the second half we conduct experiments for recurrent neural networks (RNNs) and impose an orthogonal regularization constraint **with gain** on training. While we report for some datasets non-conclusive results of orthogonal regularization, our results on Sequential MNIST dataset report that a gain-adjusted regularizer outperforms a single-soft regularizer.

![](https://github.com/EsterHlav/Dynamical-Isometry-from-Orthogonality-Neural-Nets/singular_values.png)
