Simple way to recognize handwritten shapes:

A neural network with 2 layers of neurons:
* top layer represent known shapes
* bottom layer represent pixel intensities

Output: classes of shapes

each inked pixel can vote for several different shapes, and votes can have different intensities. the shape gets most votes wins

how to learn the weights?

show strength of the input image

initial weight of each background image is random noise (0-9). the goal is train, and get the images learn from the input image. the way to learn it:

`increment` the weight from active pixels to the correct class.
`decrement` the weights from active pixels to whatever class the network guesses.

If the pixel is correct, the increment will cancel out the decrement, so nothing will change.
(details will be explained in the future lectures).
