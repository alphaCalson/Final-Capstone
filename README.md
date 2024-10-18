# Breaking Barriers: Hate Speech Detection in South African Indigenous Languages

## Executive Summary

This project aims to develop a comprehensive solution for hate speech detection specifically for South African indigenous languages, particularly the Nguni languages (isiXhosa, isiZulu, etc.). These languages are underrepresented in Natural Language Processing (NLP). The system utilizes three machine learning architectures: Capsule Network, LSTM, and CNN, tailored to capture the nuances of hate speech in online conversations. The project's ultimate goal is to provide a robust tool for making online spaces safer for speakers of these languages, filling a crucial gap in the existing hate speech detection landscape.

## Business Domain

This project is designed for use in online content moderation on platforms like social media, news websites, and forums. The intended users are platform administrators, content moderators, and policymakers who need to detect and prevent hate speech across South African indigenous languages. It also supports government initiatives to curb online hate speech and foster inclusive digital spaces.

## Problem Statement

Online platforms see an increase in toxic and hateful speech, especially in underrepresented languages like those spoken in South Africa. Current hate speech detection systems are tailored primarily for globally dominant languages (like English), leaving a significant gap in coverage for Nguni languages. This project addresses the challenges of detecting hate speech in these languages and provides a tool for more inclusive moderation.

## Objectives

- Develop a multilingual hate speech detection system for Nguni languages using CapsuleNet, LSTM, and CNN architectures.
- Achieve high accuracy (90% or higher) in detecting toxic comments in isiNdebele, isiXhosa, isiZulu, Siswati, and English.
- Create an intuitive Gradio application to allow platform administrators to utilize the models for hate speech detection.

## Scope

### In-Scope:
- Collection and annotation of hate speech datasets in indigenous South African languages.
- Training and evaluation of CapsuleNet, LSTM, and CNN models on these datasets.
- Ethical considerations and mitigation of biases during model development.

### Out-of-Scope:
- Detection in languages outside the Nguni family.
- Policy and legal implementations beyond technical deployment.

## Methodology

The project follows the **Microsoft Team Data Science Process (TDSP)**, which is a systematic and structured approach to conducting data science projects. The stages include:
1. **Business Understanding**
2. **Data Acquisition and Understanding**
3. **Modelling**
4. **Evaluation**
5. **Deployment**
6. **Customer Acceptance**

The model is trained on datasets from the **Kaggle Jigsaw toxic comment classification dataset** and South African Twitter data. Each phase adheres to TDSP’s best practices to ensure efficiency and effective model performance.

## Results

The final system was trained using the following models:
- **Capsule Network**
- **LSTM with Attention**
- **Convolutional Neural Network (CNN)**

### Model Performance:

| Model                       | Epoch | Accuracy | Validation Accuracy | Loss   | ROC-AUC |
|-----------------------------|-------|----------|---------------------|--------|---------|
| **CapsuleNet**               | 1     | 93.08%   | 84.66%              | 0.1974 | 0.7416  |
| **LSTM with Attention**      | 2     | 90.44%   | 84.63%              | 0.3188 | 0.4670  |
| **Convolutional Neural Network (CNN)** | 2     | 90.44%   | 84.63%              | 0.3108 | 0.4949  |

Despite CapsuleNet performing better in some metrics, the CNN model was chosen for deployment due to computational constraints. The models can be evaluated on a user-friendly interface via the Gradio app, making it accessible to non-technical stakeholders.

## Recommendations

1. Deploy the CNN model to monitor social media platforms in real time for toxic content in indigenous languages.
2. Expand the dataset to include other underrepresented African languages to improve model generalization.
3. Collaborate with online platforms and policymakers to adopt the models in curbing hate speech.

## Challenges and Risks

- **Data Scarcity**: Overcome using data synthesis and manual annotation.
- **Bias**: Continue refining models with the help of linguistic experts to ensure fair detection.

## Links

- **GitHub Repository**: [Final Capstone](https://github.com/alphaCalson/Final-Capstone/tree/main)
- **Gradio Deployment**: (Link to Gradio app)

## References

- [Miran, A. Z., & Abdulazeez, A. M. (2023). Detection of Hate-Speech Tweets Based on Deep Learning: A Review](https://doi.org/10.31326/jisa.v6i2.1813)
- [Oriola, Oluwafemi, & Kotzé, Eduan. (2020). Improved semi-supervised learning technique for automatic detection of South African abusive language on Twitter](https://dx.doi.org/10.18489/sacj.v32i2.847)
- [Zhang, Z., & Luo, L. (2018). Hate Speech Detection: A Solved Problem? The Challenging Case of Long Tail on Twitter](https://doi.org/10.48550/arXiv.1803.03662)
