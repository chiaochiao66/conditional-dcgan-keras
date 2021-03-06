## KERAS CONDITIONAL GAN ##

Implementation of conditional DCGAN https://arxiv.org/abs/1411.1784 with [keras](https://github.com/fchollet/keras).

Implements the improvements and architecture of https://arxiv.org/pdf/1611.07004v1.pdf.

Code borrows from the Keras DCGAN https://github.com/jacobgil/keras-dcgan and the tensorflow conditional GAN https://github.com/ppwwyyxx/tensorpack/blob/master/examples/GAN/Image2Image.py.

---

This assumes theano ordering.

---

## Usage


**Training:**

 `KERAS_BACKEND=theano THEANO_FLAGS=optimizer=fast_compile,device=cuda0,floatX=float32 ./conditional_gan.py --data train`



  KERAS_BACKEND=theano THEANO_FLAGS=optimizer=fast_compile,device=cuda0,floatX=float32 ./conditional_gan.py --data train



**Image generation:**

 `KERAS_BACKEND=theano THEANO_FLAGS=optimizer=fast_compile,device=cuda0,floatX=float32 ./conditional_gan.py --data test`



  KERAS_BACKEND=theano THEANO_FLAGS=optimizer=fast_compile,device=cuda0,floatX=float32 ./conditional_gan.py --data test


---


## Result



**generated images (conditioned on RGB) :** 



![generated_image.png](./assets/generated.png)



**train process :**



![training_process1.gif](./assets/0_0.png)
![training_process2.gif](./assets/13_0.png)
![training_process3.gif](./assets/99_0.png)




---
