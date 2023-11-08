# Revisit-Renaissance

## Introduction
Revisit Renaissance is a project created with the aim to bridge the gap between art and humans. Over the years, art has become much isolated with its admirers and its creators overlapping to a large extent. Whereas the general public has increasingly become disconnected from the whole process.

Thus this project was created to bring awareness and the common man's interest back into art using Generative AI. The aim was also to give basic knowledge about the great masters of art so as to give users a solid base to start exploring further. 
 
## Overview
The project is divided into two independent modules namely, **Image generation** and **Poem synthesis**.
Each module deals with a different kind of art.

The basic architecture of the application is as follows - 


![architecture](https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/application_architecture.jpg)

### Image Generation
This module uses Neural Style Transfer (NST) to transfer the *style* of an image onto an user specified image. In the module specifically, we use NST to impart knowledge about famous painters of the Renaissance and after by transferring the style of such famous paintings onto the photos uploaded by users. This makes the whole experience a memorable one, thus providing positive recall for the painting and its information.

In this module, I selected six iconic paintings and using Magenta Library of Tensoflow Hub, implemented Neural Style Transfer from the style image onto the content image.

![starrynight](https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/starrynight.jpg)
+
<img src='https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/iiit%20pune.jpg' width='400'/>


gives us
![starrynightiiitpune](https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/starrynight-iiitpune.jpg)

We can use the same for many different user input + painting combinations. Furthermore, this module is highly scalable in terms of adding new painters and paintings as per the need of the hour, or the specific theme (20th century, Chinese Comtemporary etc.)

### Poem Synthesis
This module uses LSTM based Neural Network to generate poems. We use seed taken in from the user and generate a poem in the style of a specific poet at character level. Character level generation means that at each time step, we predict/generate (depending on training/using) the next character upon seeing the previous character stream. An alternative to this is to use a word level model, but this type of model lacks in creativity.

Furthermore the decision to use LSTMs was due to the fact that LSTMs strike the balance between speed and accuracy required in this application. Traditional RNNs were fast but their generations were very inaccurate. On the other hand, GRUs generated coherent text but took far too long to train as well as generate the poem, thus potentially causing problems for our user. Thus the decision to use LSTMs was taken.

![seedinput](https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/poem-seed-input.jpg)
![generatedpoem](https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/generated-poem.jpg)

