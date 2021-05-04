# programming-gans

Generative Adversarial networks are minimax games in which a generator (smooth criminal) tries to fool a discriminator (the cops) into believing the world is flat. 

<img src="flat_earth.gif"  height="500" /> 

![Gans](gan.jpg)

A GAN is a zero-sum game in which eventually neither player can improve their position with any actions. This Nash equilibrium, and thus training is complete when: 
  * the generator makes perfect fakes
  * the discriminator has a 50/50 chance of identifying real or fake

The generator can only decrease the quality of its outputs by making changes to its routine. 
