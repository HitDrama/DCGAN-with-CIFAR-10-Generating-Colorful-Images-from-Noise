# 🧠 DCGAN with CIFAR-10: Generating Colorful Images from Noise

This project implements a Deep Convolutional Generative Adversarial Network (DCGAN) using PyTorch, trained on the CIFAR-10 dataset. The goal is to generate 32x32 RGB images (such as airplanes, cars, cats, dogs...) starting from random noise vectors.

## 🚀 Overview

- **Framework**: PyTorch
- **Dataset**: CIFAR-10 (32x32 color images)
- **Model**: DCGAN (Deep Convolutional GAN)
- **Objective**: Generate realistic fake images from noise using adversarial learning.

## ⚙️ Key Configurations

| Parameter        | Value       | Description                                           |
|------------------|-------------|-------------------------------------------------------|
| `batch_size`     | 32          | Number of images per training batch                  |
| `image_size`     | 32x32       | Image resolution                                     |
| `nz`             | 100         | Size of latent noise vector fed to Generator         |
| `ngf` / `ndf`    | 128         | Generator/Discriminator feature map size             |
| `num_epochs`     | 20          | Total training epochs                                |
| `lr`             | 0.0002      | Learning rate for both Generator and Discriminator   |
| `betas`          | (0.5, 0.999)| Adam optimizer stability for GAN training            |

Data is normalized to `[-1, 1]`, and models are initialized with Gaussian weights (`mean=0, std=0.02`), following best practices for stable GAN training.

## 📦 Download Trained Model

[👉 Click here to download `checkpoints.zip` from Google Drive](https://drive.google.com/file/d/1rmRcNr6-qEkMksYlXtBy3aZAWdydos-K/view?usp=drive_link)

This `.zip` file contains the trained weights of the Generator (`netG`) and Discriminator (`netD`) after 20 epochs.

## 🖼 Sample Outputs

Below are generated image samples at different training stages (epochs 1, 5, 10, 20):

<div align="center">

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/HitDrama/DCGAN-with-CIFAR-10-Generating-Colorful-Images-from-Noise/blob/main/static/epoch-1.png" width="300"/><br>
      <sub><b>Epoch 1</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/HitDrama/DCGAN-with-CIFAR-10-Generating-Colorful-Images-from-Noise/blob/main/static/epoch-5.png" width="300"/><br>
      <sub><b>Epoch 5</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/HitDrama/DCGAN-with-CIFAR-10-Generating-Colorful-Images-from-Noise/blob/main/static/epoch-15.png" width="300"/><br>
      <sub><b>Epoch 15</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/HitDrama/DCGAN-with-CIFAR-10-Generating-Colorful-Images-from-Noise/blob/main/static/epoch-20.png" width="300"/><br>
      <sub><b>Epoch 20</b></sub>
    </td>
  </tr>
</table>

</div>


## 👤 Author

**Đặng Tố Nhân**  
Developer  
🛠 _Built with PyTorch, coffee, and a passion for learning GANs._
