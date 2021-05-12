##What are GANs?
Generative Adversarial Networks (GANs) are one of the most interesting ideas in computer science today. Two models are trained simultaneously by an adversarial process. A generator ("the artist") learns to create images that look real, while a discriminator ("the art critic") learns to tell real images apart from fakes.

A diagram of a generator and discriminator
<img src="https://camo.githubusercontent.com/a57330da3aef59f5f0795bf2df0212ec181ddaf6/68747470733a2f2f6769746875622e636f6d2f74656e736f72666c6f772f646f63732f626c6f622f6d61737465722f736974652f656e2f7475746f7269616c732f67656e657261746976652f696d616765732f67616e312e706e673f7261773d31">
During training, the generator progressively becomes better at creating images that look real, while the discriminator becomes better at telling them apart. The process reaches equilibrium when the discriminator can no longer distinguish real images from fakes
<img src="https://camo.githubusercontent.com/039e94235ebf1c7262b72fe0743570fda8d48374/68747470733a2f2f6769746875622e636f6d2f74656e736f72666c6f772f646f63732f626c6f622f6d61737465722f736974652f656e2f7475746f7269616c732f67656e657261746976652f696d616765732f67616e322e706e673f7261773d31">
This notebook demonstrates this process on the MNIST dataset. The following animation shows a series of images produced by the generator as it was trained for 50 epochs. The images begin as random noise, and increasingly resemble hand written digits over time.

