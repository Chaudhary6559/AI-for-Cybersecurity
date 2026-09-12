# AI for Cybersecurity

A collection of hands-on machine learning, deep learning, natural language processing, probabilistic modeling, and generative AI projects focused on **cybersecurity applications**.

This repository documents practical implementations developed as part of an **AI for Cybersecurity** course, covering problems such as IoT malware detection, spam filtering, metamorphic malware detection, and synthetic security-data generation.

---

## 📌 Repository Overview

The projects in this repository demonstrate how Artificial Intelligence and Machine Learning can be applied to identify, analyze, and simulate cybersecurity threats.

The labs progressively explore different types of cybersecurity data:

* **Network traffic** → IoT malware and botnet detection
* **Text messages** → SMS spam classification
* **Opcode sequences** → Metamorphic malware detection
* **Images / QR codes** → Synthetic data generation using GANs

The repository combines traditional machine learning, deep learning, NLP, probabilistic models, and generative models to demonstrate different approaches to cybersecurity problems.

---

## 📂 Repository Structure

```text
AI-for-Cybersecurity/
│
├── Detecting-IoT-Malware-Behavior-in-Network-Traffic/
│   ├── Detecting_IoT_Malware_Behavior.ipynb
│   └── README.md
│
├── SMS-Spam-Collection-Naive-Bayes/
│   ├── SMS_Spam_Collection_Naive_Bayes.ipynb
│   └── README.md
│
├── HMM-for-Metamorphic-Malware-Detection/
│   ├── HMM_Metamorphic_Malware_Detection.ipynb
│   └── README.md
│
├── Generating-Synthetic-QR-Codes-with-GAN/
│   ├── Generating_Synthetic_QR_Codes_with_GAN.ipynb
│   └── README.md
│
└── README.md
```

Each project folder contains the corresponding notebook and a dedicated README explaining the implementation, methodology, technologies, and cybersecurity application.

---

## 🧪 Projects

### 1. Detecting IoT Malware Behavior in Network Traffic

**Focus:** Network Security · IoT Security · Malware Detection · Machine Learning · Deep Learning

This project analyzes IoT network traffic to identify patterns associated with malicious and botnet behavior.

Two approaches are explored:

* Random Forest classification
* Neural Network classification

The project includes data preprocessing, feature preparation, scaling, dimensionality reduction, model training, evaluation, and visualization of deep-learning training history.

**Key concepts:**

* IoT Security
* Network Traffic Analysis
* Botnet Detection
* Malware Detection
* Random Forest
* Neural Networks
* Feature Scaling
* Dimensionality Reduction
* Model Evaluation

---

### 2. SMS Spam Collection — Naïve Bayes Spam Filter

**Focus:** NLP · Text Classification · Spam Detection · Supervised Learning

This project develops a machine-learning-based spam filter capable of distinguishing between **spam** and **legitimate (ham)** messages.

The implementation demonstrates how text can be transformed into numerical features and classified using a Naïve Bayes model.

The workflow includes:

```text
SMS Dataset
     ↓
Text Preprocessing
     ↓
Tokenization / Stop-word Removal
     ↓
Feature Extraction
     ↓
Train/Test Split
     ↓
Naïve Bayes Classifier
     ↓
Model Evaluation
     ↓
Model Export
     ↓
New Message Classification
```

**Key concepts:**

* Naïve Bayes
* Bayes Theorem
* NLP
* Tokenization
* Stop-word Removal
* Text Vectorization
* TF-IDF
* Spam Detection
* Classification
* Model Evaluation
* Model Serialization

---

### 3. HMM for Metamorphic Malware Detection

**Focus:** Malware Analysis · Sequence Modeling · Hidden Markov Models

This project applies a **Hidden Markov Model (HMM)** to the analysis of opcode sequences in order to distinguish potentially malicious software from legitimate programs.

Metamorphic malware can modify its code structure while maintaining its underlying malicious functionality. Sequence-based analysis provides a way to identify behavioral patterns that may remain across these transformations.

The project covers:

* Opcode preprocessing
* Sequence representation
* HMM training
* Sequence likelihood
* Malware classification
* Error and edge-case handling

**Key concepts:**

* Hidden Markov Models
* Hidden States
* Transition Probabilities
* Observation Probabilities
* Opcode Sequences
* Sequence Modeling
* Metamorphic Malware
* Static Analysis
* Probabilistic Machine Learning

---

### 4. Generating Synthetic QR Codes with GAN

**Focus:** Generative AI · Computer Vision · Synthetic Data · GANs

This project explores the use of **Generative Adversarial Networks (GANs)** to generate synthetic QR-code images containing embedded messages.

The project involves creating a dataset of QR codes, preprocessing the images, training a generator and discriminator, and producing new synthetic QR-code samples.

The basic GAN architecture is:

```text
Random Noise
     ↓
Generator
     ↓
Synthetic QR Code
     ↓
┌─────────────────────┐
│                     │
│     Discriminator    │
│                     │
└─────────────────────┘
     ↑           ↑
     │           │
Real QR       Generated QR
Codes            Codes
```

The generator attempts to create realistic QR codes while the discriminator learns to distinguish real images from generated ones.

**Key concepts:**

* Generative Adversarial Networks
* Generator
* Discriminator
* Adversarial Training
* Deep Learning
* Synthetic Data
* Image Generation
* Computer Vision
* QR Codes
* Generative AI

---

## 🔬 Machine Learning Techniques Covered

| Area                 | Techniques                                          |
| -------------------- | --------------------------------------------------- |
| Network Security     | Network Traffic Analysis, Botnet Detection          |
| Machine Learning     | Random Forest, Naïve Bayes                          |
| Deep Learning        | Neural Networks, GANs                               |
| NLP                  | Tokenization, Stop-word Removal, Text Vectorization |
| Malware Analysis     | Opcode Sequence Analysis                            |
| Probabilistic Models | Hidden Markov Models                                |
| Generative AI        | Generative Adversarial Networks                     |
| Computer Vision      | Image Preprocessing, Synthetic Image Generation     |
| Model Evaluation     | Classification Metrics, Training History            |

---

## 🛡️ Cybersecurity Applications

The techniques demonstrated throughout this repository can be applied to a variety of cybersecurity scenarios, including:

* **IoT malware and botnet detection**
* **Network traffic analysis**
* **Spam and malicious-message filtering**
* **Phishing and social-engineering detection**
* **Malware classification**
* **Metamorphic malware analysis**
* **Static malware analysis**
* **Security-data generation**
* **Adversarial machine-learning research**
* **Cybersecurity dataset augmentation**
* **Security testing and simulation**
* **AI-assisted threat detection**

---

## 🛠️ Technologies & Tools

The projects use a combination of Python-based data science and AI technologies.

### Programming

* Python 3.x
* Jupyter Notebook

### Data Science & Machine Learning

* NumPy
* Pandas
* Scikit-learn

### Deep Learning

* TensorFlow / Keras
* Neural Networks
* GAN architectures

### NLP

* NLTK
* Text preprocessing
* Text vectorization

### Probabilistic Modeling

* `hmmlearn`
* Hidden Markov Models

### Visualization

* Matplotlib

### Other Tools

* QR-code generation libraries
* Image-processing utilities
* Model serialization tools

---

## 📈 Overall Learning Progression

The repository demonstrates a progression from traditional machine learning techniques toward more advanced AI approaches:

```text
Cybersecurity Data
       │
       ├── Network Traffic
       │       ↓
       │   Random Forest
       │       ↓
       │   Neural Networks
       │
       ├── Text Messages
       │       ↓
       │   NLP Preprocessing
       │       ↓
       │   Naïve Bayes
       │
       ├── Opcode Sequences
       │       ↓
       │   Sequence Modeling
       │       ↓
       │   Hidden Markov Models
       │
       └── QR Code Images
               ↓
          Deep Learning
               ↓
              GAN
               ↓
       Synthetic Data Generation
```

This progression highlights how different AI techniques can be selected according to the **type and structure of cybersecurity data**.

---

## 🎯 Learning Outcomes

Through these projects, the repository demonstrates practical experience with:

* Applying machine learning to cybersecurity problems
* Preparing and preprocessing security-related datasets
* Training and evaluating classification models
* Applying deep learning to threat detection
* Working with textual cybersecurity data
* Performing sequence-based malware analysis
* Understanding probabilistic models for security applications
* Building generative models for synthetic data
* Visualizing model behavior and training performance
* Translating AI concepts into practical cybersecurity use cases

---

## 📚 Course Projects

| #  | Project                                           | Main Technique                 |
| -- | ------------------------------------------------- | ------------------------------ |
| 01 | Detecting IoT Malware Behavior in Network Traffic | Random Forest + Neural Network |
| 02 | SMS Spam Collection                               | Naïve Bayes + NLP              |
| 03 | HMM for Metamorphic Malware Detection             | Hidden Markov Model            |
| 04 | Generating Synthetic QR Codes                     | GAN                            |

---

## 👨‍💻 Purpose

This repository serves as a practical portfolio of **AI-driven cybersecurity projects**, demonstrating the application of machine learning, deep learning, NLP, probabilistic modeling, and generative AI to real-world security challenges.

It is intended for **learning, experimentation, portfolio development, and demonstrating practical AI/cybersecurity skills**.

---

## ⭐ Key Skills Demonstrated

**Artificial Intelligence · Machine Learning · Deep Learning · Cybersecurity · NLP · Computer Vision · Malware Detection · Network Security · Anomaly Detection · Sequence Modeling · Generative AI · Synthetic Data · Python · Scikit-learn · TensorFlow/Keras · NLTK · hmmlearn · Jupyter Notebook**
