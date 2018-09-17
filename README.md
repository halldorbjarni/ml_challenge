# ML Challenge

Overall this was a very fun challenge. My approach was based on a blog post ([link](https://medium.com/@ageitgey/machine-learning-is-fun-part-8-how-to-intentionally-trick-neural-networks-b55da32b7196)) which was basically to find the gradient to maximize the probability of the image being a six **with respect to the input image** but not the weights in the neural net. I think this is somewhat analogous to a neural net where the gradient is only based on the first layer but not the last two layers of the neural net. I think the key learning here is that sometimes it's good to think outside of the box, like taking the gradient with respect to something other than the weights. 

I ran into a few problems with training taking very long for some input images. I tried using momentum gradient descent to speed things up and that helped (after playing around with the learning rate). It however only became fast once the momentum was bigger than 1 which is not how it should be used since you just snowball in one direction, oblivious to any change. I'm actually quite curious why some input examples behave like that.

The link to the 10 adversarial images can be found [here](https://github.com/halldorbjarni/ml_challenge/blob/master/adversarial_examples.png).

To reproduce my results spin up a jupyter notebook and execute the cells in the IPython notebook.



![here](https://github.com/halldorbjarni/ml_challenge/blob/master/adversarial_examples.png).

