# Revisit-Renaissance

## Introduction
Revisit Renaissance is a project created with the aim to bridge the gap between art and humans. Over the years, art has become much isolated with its admirers and its creators overlapping to a large extent. Whereas the general public has increasingly become disconnected from the whole process.

Thus this project was created to bring awareness and the common man's interest back into art using Generative AI. The aim was also to give basic knowledge about the great masters of art so as to give users a solid base to start exploring further. 
 
## Overview
The project is divided into two independent modules namely, **Image generation** and **Poem synthesis**.
Each module deals with a different kind of art.

### Image Generation
This module uses Neural Style Transfer (NST) to transfer the *style* of an image onto an user specified image. In the module specifically, we use NST to impart knowledge about famous painters of the Renaissance and after by transferring the style of such famous paintings onto the photos uploaded by users. This makes the whole experience a memorable one, thus providing positive recall for the painting and its information.

In this module, I selected six iconic paintings and using Magenta Library of Tensoflow Hub, implemented Neural Style Transfer from the style image onto the content image.

![starrynight](https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/starrynight.jpg)
+
<img src='https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/iiit%20pune.jpg' width='450'/>
gives us
![starrynightiiitpune](https://github.com/ThePrincipleMan/Revisit-Renaissance/blob/main/client/src/images/starrynight-iiitpune.jpg)
