# Generating Synthetic QR Codes with GAN

## Overview

This project explores the use of a **Generative Adversarial Network (GAN)** to generate synthetic QR code images containing embedded messages.

The project begins by creating a dataset of QR codes and dividing the images into training and validation sets. The images are then preprocessed and used to train a GAN consisting of two competing neural networks:

* **Generator** — creates synthetic QR code images.
* **Discriminator** — determines whether an image is real or generated.

Through adversarial training, the generator learns to produce increasingly realistic QR code images.

## Objectives

* Understand the fundamental architecture of Generative Adversarial Networks.
* Generate a dataset of QR codes containing embedded messages.
* Prepare QR-code images for deep learning.
* Build a GAN generator and discriminator.
* Train the GAN through adversarial optimization.
* Monitor the training process.
* Generate new synthetic QR codes using the trained generator.
* Save and inspect generated QR-code images.
* Evaluate the quality of generated outputs.

## Problem Statement

QR codes are widely used for authentication, payments, URLs, information sharing, and other digital applications. Generative models can be used to investigate how realistic synthetic QR-code images can be produced.

The goal of this project is to train a GAN that learns the visual structure of QR codes and generates new images that resemble the training examples.

The project demonstrates the broader cybersecurity relevance of **generative AI, synthetic data generation, and adversarial machine learning**.

## GAN Architecture

A GAN consists of two neural networks trained against each other.

```text id="k8g2lr"
                    Random Noise
                         ↓
                  ┌─────────────┐
                  │  Generator  │
                  └──────┬──────┘
                         ↓
                 Synthetic QR Code
                         │
                         ↓
Real QR Code ─────→ ┌──────────────┐
                    │ Discriminator│
                    └──────┬───────┘
                           ↓
                     Real / Fake
```

### Generator

The generator receives random input and transforms it into a synthetic QR-code image.

Its objective is to produce images that the discriminator cannot distinguish from real training examples.

### Discriminator

The discriminator receives both real and generated images and attempts to determine whether each image comes from the original dataset or the generator.

The competition between the two networks drives the generator toward producing increasingly realistic outputs.

## Dataset Preparation

The project creates a dataset containing **100 QR-code images** with embedded messages.

The dataset is divided into:

* Training data
* Validation data

The images are then preprocessed into a format suitable for GAN training.

The preprocessing stage prepares the QR-code images for input to the neural networks and helps provide consistent image dimensions and numerical representations.

## Training Workflow

```text id="s6z9eq"
QR Code Messages
       ↓
QR Code Generation
       ↓
Image Dataset
       ↓
Train / Validation Split
       ↓
Image Preprocessing
       ↓
       ┌─────────────────────┐
       │    GAN Training     │
       │                     │
       │ Generator ↔         │
       │ Discriminator       │
       └──────────┬──────────┘
                  ↓
          Trained Generator
                  ↓
       Synthetic QR Code Images
                  ↓
          Output Evaluation
```

## Adversarial Training

GAN training is based on competition between the generator and discriminator.

During training:

1. The generator creates synthetic QR-code images.
2. The discriminator receives real and synthetic images.
3. The discriminator learns to distinguish real images from generated images.
4. The generator receives feedback from the discriminator.
5. The generator improves its ability to create realistic images.
6. The process is repeated over many training iterations.

The lab trains the GAN for **5,000 epochs** to progressively optimize the generator and discriminator.

## Generated QR Codes

After training, the generator is used independently to create new QR-code images.

The generated outputs can then be saved and inspected to determine whether the generator has successfully learned the visual characteristics of the training dataset.

Conceptually:

```text id="v9w0zn"
Trained Generator
       ↓
Random Input
       ↓
Synthetic QR Code
       ↓
Save Image
       ↓
Visual Inspection
```

## Evaluation

The generated images are evaluated primarily by examining their visual quality and similarity to the original QR-code dataset.

Evaluation can consider:

* Visual similarity
* QR-code structure
* Image quality
* Generator output consistency
* Training behavior
* Whether generated QR codes preserve useful encoded information

The generated outputs provide an empirical way to assess whether the GAN successfully learned the underlying image distribution.

## Cybersecurity Applications

Generative models such as GANs have applications in cybersecurity and security research, including:

* Synthetic security-data generation
* Adversarial machine learning research
* Security-system testing
* Dataset augmentation
* Privacy-preserving synthetic data
* Robustness testing
* Computer-vision security research
* Simulation of realistic digital artifacts

QR-code generation can also serve as an example of how generative models may be used to create synthetic visual data for testing computer-vision and security systems.

## Key Concepts

* Generative Adversarial Networks
* GAN Generator
* GAN Discriminator
* Adversarial Training
* Deep Learning
* Synthetic Data Generation
* Image Generation
* QR Codes
* Neural Networks
* Image Preprocessing
* Training and Validation
* Model Optimization
* Generative AI
* Computer Vision
* Cybersecurity Applications

## Technologies

* **Python**
* **Deep Learning Framework**
* **NumPy**
* **QR Code Generation**
* **Image Processing**
* **Jupyter Notebook**

## Project Structure

```text id="9l1vpe"
Generating-Synthetic-QR-Codes-with-GAN/
│
├── Generating_Synthetic_QR_Codes_with_GAN.ipynb
└── README.md
```

## Learning Outcome

This project provides hands-on experience with **Generative Adversarial Networks and synthetic image generation**. It demonstrates how a generator and discriminator can be trained together to learn the visual distribution of QR-code images.

The project also introduces the broader use of generative models in **cybersecurity research, synthetic data generation, adversarial testing, and computer-vision security applications**.

## Course Information

**Course:** AI for Cybersecurity
**Lab:** Generating Synthetic QR Codes with the Trained Generator
**Model:** Generative Adversarial Network (GAN)
**Domain:** Generative AI / Computer Vision / Cybersecurity
**Data Type:** QR Code Images
**Language:** Python
