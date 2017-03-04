Architecture: how neurons are connected together.

1. Feed-forward neural networks (common)
* first layer is the input units, the last layer is the output, and one or more layers of hidden units.
* for networks with more than one hidden layer, we call them "deep" neural networks (deep learning).
* they compute a series of transformations that change the similarities between cases, so that in each layer, there is a new layer of input.

2. Recurrent networks
* have directed cycles in connected graphs, have complicated dynamics, and hard to train.
* natural way to model `sequential data` (e.g., stock price over past 5 years)
* have the ability to remember info in hidden state for a long time (very hard to train)

Example: predict the next character in a sequence.

3. Symmetrically connected networks
Similar to recurrent networks, but connection between units are symmetrical (same weight in both directions)
* much easier to analyze than recurrent networks
* cannot model cycles.
