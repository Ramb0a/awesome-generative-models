# Gans

Generative Adversarial networks are minimax games in which a generator (smooth criminal) tries to fool a discriminator (the cops) into believing the world is flat. 

<img src="flat_earth.gif"  height="400" /> 

> Because the Generator and Discriminator can tune only their own parameters and not each other’s, GAN training can be better described as a game, rather than optimization.

> GANs consist of two networks whose cost functions are dependent on both of the networks’ parameters. 

In this zero-sum game, eventually neither player can improve their position with any actions. This happens when both the generator discriminator can no further minimize the loss of the parameters under their control.

The [Nash equilibrium](https://www.investopedia.com/terms/n/nash-equilibrium.asp#:~:text=The%20Nash%20equilibrium%20is%20a%20decision%2Dmaking%20theorem%20within%20game,the%20decisions%20of%20other%20players.) brings training to completion when: 
  * the generator makes perfect fakes
  * the discriminator has a 50/50 chance of identifying real or fake

At that point the generator can only decrease the quality of its outputs by making changes to its routine. 

<img src="gan_equal.png" height="500" />

When the Disciminator acts as a Classifier and 1 is the label for Real and 0 the label for Fake, we get the confusion Matrix: 

| Input | Discrimintator Close to 1 | Discriminator Close to 0 |
| ---- | ---- | --- | 
|Real (x) | Positive Postive | False Negative |
| Fake (*x) | False Positive | Positive Negative |

It is the generators job to evoke all error that it can in the Discriminators judgement of its work product through the creation of artifacts that result in false positives, and false negatives. 

![Gans](gan.jpg)

The discriminative classifier and the generator train themselves after battle to be better the next time.

<img src="sf.gif" />


## [Vanilla GAN](https://youtu.be/HGYYEUSm-0Q)

Goodfellow and other put forth the GAN architecture in (2014) in [Generative Adversarial Nets](https://arxiv.org/pdf/1406.2661.pdf)

# References

(2017) [Towards Principled Methods For Training Generative Adversarial Network](https://arxiv.org/pdf/1701.04862.pdf)

(2017) [Stabilizing Training of Generative Adversarial Networks through Regularization](https://arxiv.org/pdf/1705.09367.pdf)

(2014 [Generative Adversarial Nets](https://arxiv.org/pdf/1406.2661.pdf)

