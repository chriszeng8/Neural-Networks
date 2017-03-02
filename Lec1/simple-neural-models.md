Idealized Neurons

1. *Linear Neurons*

Simple but computationally limited

```
y = b + sum (x_i * w_i)
```
output y =  bias of the neuron b + sum of all incoming connections (where w_i is weighting on input line i, x_i is activity on input line i)

2. Binary threshold Neurons

McCulloch-Pitts
* First compute a weighted sum of the inputs.
* then send out a fixed size spike of activity if the weighted sum exceeds a threshold.
* each neuron combines truth values of proposition to compute the truth values of another proposition (no exactly sure what it means yet)

Two equivalent ways to write binary threshold neuron:

z = sum_i (x_i*w_i),
y = 1 (if z>=threshold), or 0 otherwise

Alternatively,
z = b + sum (x_i * w_i)
y = 1 if z>=0, or 0 otherwise. (in which b = - threshold);

3. Rectified Linear Neurons

Compute a `linear` weighted sum of inputs, the output is a `non-linear` function of the total input.

z = b + sum (x_i*w_i)
y = z if z>=0, or y = 0 otherwise.


4. Sigmoid Neurons (most commonly used in artificial neuron nets)

gives real value output that is smooth and bounded function of their of input.
value bounded between 0 and 1.
`typically they use the logistic function`
The total input z is computed:
  ```z = b + sum (x_i* w_i)```
The output is:
```y=1/(1+e^-z)```

when z= 0, y is 0.5.
Nice thing about sigmoid is that is has smooth derivative.

5. Stochastic binary Neurons.
```z = b + sum (x_i* w_i)```
```P(s=1)=1/(1+e^-z)``` (not too sure what this means???)
