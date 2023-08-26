# Federated Mind: Collaborative AI Training with Federated Learning

This repository contains code for a Federated Learning project that demonstrates the collaborative training of machine learning models using a federated approach.

## Table of Contents

- [Introduction](#introduction)
- [Setup](#setup)
- [Usage](#usage)

## Introduction

Federated Learning is a decentralized machine learning approach that enables training models across multiple devices or servers while keeping data localized. This project showcases the implementation of a federated learning scenario with local clients contributing to the improvement of a global model without sharing raw data.

## Setup

To run this project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/federated-learning-project.git
   cd federated-learning-project
   ```
2. Set up a Python environment and install dependencies:
   ```
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
3. Prepare the dataset:
  - Make sure to have the necessary CSV files with client data.
  - Update the file paths in the code to point to your dataset.

## Usage

1. Local and Global Model Definition:

- Define the model architecture and metrics in the Model_alpha class.
- Set hyperparameters, optimizer, and loss in the code.

2. Creating Client Data:

- Use the provided functions to create data for both local and global clients.
- Adjust the data paths according to your dataset.

3. Model Training:

- Train the global model using the global client data.
- Train individual local models using their respective client data.

4. Communication Rounds:

- Iteratively update the global model by averaging weights of local models.
- Evaluate and test the models after each communication round.

5. Visualizations:

- Observe training histories and model performance metrics using the plotted graphs.
