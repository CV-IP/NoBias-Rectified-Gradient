# No Bias Rectified Gradient

In 
[*Why are Saliency Maps Noisy? Cause of and Solution to Noisy Saliency Maps*](https://arxiv.org/abs/1902.04893) Rectified Gradient has been introduced, a method of making saliency maps less noisy by modifying the rule of backpropagating the gradients. Additionally, in a final step a multiplication with input features has been hardcoded into the method. 

Due to the bias introduced by this multiplication with input features it is in many cases undesirable. We therefore add a new method "nobias_rectgrad" which is equivalent to Rectified Gradient but omits this final step.
