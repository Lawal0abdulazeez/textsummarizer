# End to end Text-Summarizer-Project

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the pipeline
7. update the main.py
8. update the app.py


# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/entbappy/End-to-end-Text-Summarization
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n summary python=3.11 -y
```

```bash
conda activate summary
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```


```bash
Author: Krish Naik
Data Scientist
Email: krishnaik06@gmail.com

```

# Azure CI/CD Deployment with GitHub Actions

This guide explains how to set up a CI/CD pipeline for Azure using GitHub Actions, with equivalents to common AWS services.

## Prerequisites
- Azure account
- Azure CLI installed
- GitHub repository
- Basic understanding of Docker and CI/CD concepts

## Setup Instructions


### 1. Login to Azure Portal
1. Go to [portal.azure.com](https://portal.azure.com)
2. Sign in with your Azure account

### 2. Create Azure Service Principal for Deployment
```bash
# Using Azure CLI
az login
az ad sp create-for-rbac --name "github-actions-deploy" --role contributor \
  --scopes /subscriptions/<subscription-id> \
  --sdk-auth


