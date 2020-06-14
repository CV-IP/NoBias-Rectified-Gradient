# Modifed Rectified Gradient

In 
[*Why are Saliency Maps Noisy? Cause of and Solution to Noisy Saliency Maps*](https://arxiv.org/abs/1902.04893) Rectified Gradient has been introduced, a method of making saliency maps less noisy by modifying the rule of backpropagating the gradients. Additionally, in a final step a multiplication with input features has been hardcoded into the method. 

Since this multiplication with input features is in many cases undesirable, we add a new method "name of the method" which is equivalent to Rectified Gradient in most regards but omits this final step.
