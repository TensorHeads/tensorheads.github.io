## Appendix

## Other Experiments:

### DC-GAN experiment

We tried setting up the DC-GAN with the DeepFashion - Fashion synthesis dataset. The default architecture supports generation of images of size 64x64. After training the model, the generated images of size 64x64 were pretty good. But we required images to be of higher resolution than that. So, we tried making required changes to the default architecture to support generation of higher resolution images but the model seemed to be too slow at learning. After training it for around 1500-2000 iterations, the Generator loss got stuck at 100 and the discriminator loss around 0. And then observing the output, the generated images were very poor, not even vaguely close to human body form. On continuing the training, the model seemed to be stuck at one point and hence we decided to move to StyleGan2 which proved to be working well for high-resolution image generation.


### L2 Objective for GAN:
We tried changing the GAN Objective to L2 Objective to check the quality of the image being generated. Keeping everything else as constant, we changed the GAN Objective from 
WGAN to L2. Below are the loss functions for the Discriminator and the Generators.

<img src="img/loss.png" width=500>

#### Loss Plot

<img src="img/curve1.png" width=400>
<img src="img/curve2.png" width=400>

The orange curve is the Phase 1 training's loss of the Discriminator and the blue curve is the Phase 2 training's loss of both the Discriminator and the Generator. We stopped the Phase 2 training after 12k iterations as the Discriminator's loss was really low but the results were bad as shown below.

#### Results
<img src="img/i1.png" width=800>

The Generator produces parameters such that a major part of the bag is out of frame. It learned a trivial solution, when using the L2 loss.


