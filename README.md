# Neural Style Transfer

[Neural Style Transfer](https://en.wikipedia.org/wiki/Neural_Style_Transfer) is the process of composing an image in the style of another image. Neural Style Transfer algorithms are characterized by their use of deep neural networks in order to perform the image transformation. 

This technique was first introduced by Gatys et al. in [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576). 

A content image and a style image are input to a neural network. The goal is to generate a mixed image that has contours of the content image and texture, color pattern of the style image. How it works? 

The loss function for the content image minimizes the difference of the features activated for the content image corresponding to the mixed image. Whereas the loss function for the style image minimizes the difference between so-called Gram-matrices between style image and the mixed image. This is done at one or more layers. Gram matrix is used to identify which features are activated simultaneously at a given layer.

I used the VGG-19 model (pre-trained weights) to perform the NST. 

# Examples
## Bordeaux paintings

### Bordeaux - Afremov

<div align='center'>
  <img src='content images/bordeaux.jpg' height="225px">
  <img src='style images/afremov.jpeg' height="225px">
  <img src='NST Paintings/bdx_afremov_stylized.png' height="225px">
</div>

### Bordeaux - Van Gogh

<div align='center'>
  <img src='content images/bordeaux.jpg' height="225px">
  <img src='style images/vangogh.jpeg' height="225px">
  <img src='NST Paintings/van_gogh2.png' height="225px">
</div>

### Bordeaux - Monet 

<div align='center'>
  <img src='content images/bordeaux.jpg' height="225px">
  <img src='style images/monet.jpeg' height="225px">
  <img src='NST Paintings/monet_bdx.png' height="225px">
</div>

### Bordeaux - Dali

<div align='center'>
  <img src='content images/bordeaux.jpg' height="225px">
  <img src='style images/dali.jpg' height="225px">
  <img src='NST Paintings/bdx_dali_stylized.png' height="225px">
</div>

## Own picture

<div align='center'>
  <img src='content images/PP Linkedin.jpg' height="225px">
  <img src='style images/vangogh.jpeg' height="225px">
  <img src='NST Paintings/van_gogh (1).png' height="225px">
</div>
