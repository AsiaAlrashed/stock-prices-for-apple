# Fine-Tuning and Evaluation of GPT-3.5 Turbo

This repository contains scripts for fine-tuning and evaluating a customized GPT-3.5 Turbo model using OpenAI's API.

##1. Fine-Tuning the Model (fine_tuning.py)
##Description

This script fine-tunes a GPT-3.5 Turbo model using custom training data.

##Steps Performed

1. Uploads training and validation data to OpenAI servers.

2. Starts the fine-tuning process with specified hyperparameters.

3. Monitors the training status until completion.

##How to Run
1. Install required dependencies:
   '''pip install openai'''
2. Set up the OpenAI API key in openai_client.py:
'''   import openai
client = openai.OpenAI(api_key="your-api-key")'''

4. 
