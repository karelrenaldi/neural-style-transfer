# Neural Style Transfer

This repository implements **Neural Style Transfer (NST)** using a fine-tuned **pretrained CNN model (VGG-19)**. NST is a technique that applies the artistic style of one image to the content of another image using deep learning.

## Features
- Fine-tune a **pretrained VGG-19 model** for NST
- Extract **content** and **style** representations using different layers of VGG-19
- Compute **content loss**, **style loss**, and **total variation loss**
- Optimize the generated image using **gradient descent**

## Prerequisites
- Python 3.x
- TensorFlow
- NumPy
- Matplotlib
- PIL (Pillow)

Install dependencies using:
```bash
pip install tensorflow numpy matplotlib pillow
```

## How It Works
1. Load **VGG-19**, a pre-trained CNN model trained on ImageNet.
2. Extract **content features** from deep layers of the network.
3. Extract **style features** from shallow and deep layers.
4. Compute **content loss** and **style loss** to measure the difference between images.
5. Optimize the input image iteratively using **gradient descent**.
6. Generate a final image that combines the **content of the first image** and **style of the second image**.

## Example
Input:
- Content Image: A regular photograph
- Style Image: A famous painting (e.g., Van Gogh's *Starry Night*)

Output:
- A transformed image that retains the structure of the content image but with the artistic style applied.

## References
- [Original Neural Style Transfer Paper (Gatys et al., 2015)](https://arxiv.org/abs/1508.06576)
- [VGG-19 Model](https://arxiv.org/abs/1409.1556)
