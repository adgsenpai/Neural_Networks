# Neural_Networks
Understanding Neural Networking with basics of Keras.

<img src="https://github.com/ADGVLOGS/Neural_Networks/blob/main/resources/nth-network.png?raw=true">
<p>Diagram of a Nth Neural Network</p>

| Topics                     | Links                                                             |
|----------------------------|-------------------------------------------------------------------|
|Keras Activation Functions: | https://keras.io/activations/                                     |
|Keras Models:               | https://keras.io/models/about-keras-models/#about-keras-models    |
|Keras Optimizers:           | https://keras.io/optimizers/                                      |
|Keras Metrics:              | https://keras.io/metrics/                                         |
|Keras - Functions           | https://keras.io/api/models/sequential/                           |


## Important Partial Derivatives for Backpropagation 
#### (experimenting with LaTeX for GitHub for full equations sheet check out) 

https://raw.githubusercontent.com/adgsenpai/Neural_Networks/main/Partial_Derivatives_Backpropagation.pdf

`Equation 1`

$$ z_{1} =  x_{1}*w_{1}+b_{1} $$

`Equation 2`

$$ a_{1} = f(z_{1}) = {1 \over 1+e^{-z_{1}}} $$

`Equation 3`

$$ z_{2} = a_{1} * w_{2} + b_{2} $$

`Equation 4`

$$ a_{2} = f(z_{2}) = {1 \over 1+e^{-z_{2}}}$$

`Equation 5`

$$ E = {1 \over 2}{(T-a_{2})^2} $$

#### Doing one partial differential equation

`using Equation 5` $$ E = {1 \over 2}{(T-a_{2})^2} $$



1. for $ {\partial{E} \over \partial{w_2}} $

$ {\partial{E} \over \partial{w_2}} = {\partial{E} \over \partial{a_2}}{\partial{a_{2}} \over \partial{z_{2}}} {\partial{z_{2}} \over \partial{w_{2}}} $

$ {\partial{E} \over \partial{w_2}} = 2{1 \over 2}{(T-a_{2})}{(-1)} $
$ = -{(T-a_{2})}$

 
