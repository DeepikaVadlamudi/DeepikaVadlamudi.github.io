<p>A fundamental task in the field of Computer Vision is Edge Detection. A sobel filter, a widely used image processing technique, is used for just this purpose. It helps in identifying edges or boundaries of objects within an image by highlighting the areas with rapid changes in intensity. 
  In this article, we shall explore the Sobel filter and demonstrate its implementation in Python using CUDA for GPU acceleration.</p>

![A sobel filter applied to an image](assets/images/Sobel_Wiki_Image.png) 

### Understanding the Sobel Filter

<p>The Sobel filter consists of two 3x3 convolution kernels: one for detecting changes in the horizontal direction and the other in the vertical direction. These kernels compute the gradient of the image intensity at each pixel, highlighting the edges. 
  The gradient magnitude can be used to identify edges, and the gradient direction can be used for further analysis.</p>

<p>Here are the two Sobel Kernels:</p>

<p>Horizontal Sobel Kernel (```Gx```)</p>
