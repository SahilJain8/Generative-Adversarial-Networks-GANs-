# Generative Adversarial Networks (GANs)


![Alt Text](https://www.google.com/imgres?imgurl=https%3A%2F%2Flh4.googleusercontent.com%2FyAT4vN1GFT8D0QUDMAReZS0BLD_vi7KZc-AE02RFWI9ZVSQHLqKTTthtgx_BK-DlKOeFDgtkA3byl9VMHPEI0r5ZTn1nKYLbeEflJuspuykXcNMOmEmXomWZzMwdzUBbxf-BlkjJ&tbnid=hXalGgUIxn3iGM&vet=12ahUKEwipw8e3946CAxX35TgGHSx-A6kQMygAegQIARBP..i&imgrefurl=https%3A%2F%2Fneptune.ai%2Fblog%2Fgan-loss-functions&docid=g3NLtNOXH4QF1M&w=754&h=133&q=loss%20function%20gans&ved=2ahUKEwipw8e3946CAxX35TgGHSx-A6kQMygAegQIARBP) 

GANs work by using two neural networks: a generator and a discriminator. The generator creates data, while the discriminator evaluates how real that data looks. They train in a competitive manner:

#### Generator: 
It takes random noise as input and generates data.

#### Discriminator:
It distinguishes between real and generated data, learning to assign high probabilities to real data.

#### Training: 
The generator minimizes its loss, making its output more convincing. The discriminator maximizes its loss, improving its ability to classify.


![Alt Text](img_2.png) 

##### Generating Data: 
Once trained, the generator can create new data samples by inputting random noise.

GANs have been successful in generating various types of data, including images and text. They have applications in image synthesis, style transfer, and more.


## Loss funtion 

![Alt Text](img.png) 
In Generative Adversarial Networks (GANs), there are two primary loss functions:

#### Generator Loss: 
The generator aims to produce data that looks real. Its loss function is typically binary cross-entropy, encouraging it to minimize the difference between the discriminator's probability for the generated data and 1.

#### Discriminator Loss: 
The discriminator's job is to distinguish real from generated data. It also uses binary cross-entropy, with a goal to maximize the difference between its probability for real data and generated data.

