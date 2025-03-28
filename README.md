# Fine-Tuning and Evaluation of GPT-3.5 Turbo

This repository contains scripts for fine-tuning and evaluating a customized GPT-3.5 Turbo model using OpenAI's API.

## 1. Fine-Tuning the Model (fine_tuning.py)
##Description

This script fine-tunes a GPT-3.5 Turbo model using custom training data.

## Steps Performed

1. Uploads training and validation data to OpenAI servers.

2. Starts the fine-tuning process with specified hyperparameters.

3. Monitors the training status until completion.

## How to Run
1. Install required dependencies:
   ```python
   pip install openai
2. Set up the OpenAI API key in openai_client.py:
   ```python
   import openai
   client = openai.OpenAI(api_key="your-api-key")
3. Run the fine-tuning script:
   ```python
   python fine_tuning.py

After the fine-tuning completes, the model ID will be generated. This ID is needed for evaluation.

## 2. Evaluating the Fine-Tuned Model (evaluate_fine_tuned.py)
   ## Description
      
   1. This script evaluates the fine-tuned model by:
      
   2. Passing validation data to the model.
      
   3. Comparing the model's predictions against ground truth labels.
      
   4. Calculating classification metrics such as Accuracy, Precision, Recall, and F1-score.

  ## Steps Performed
   
   1. Loads validation dataset (filtered_val.jsonl).
   
   2. Extracts ground truth classifications from the dataset.
   
   3. Uses the fine-tuned model to classify the data.
   
   4. Calculates and prints evaluation metrics.

   ## How to Run
   1. Install required dependencies:
      ```python
      pip install openai scikit-learn
   2. Set up the OpenAI API key in openai_client.py.
   3. Update the script with your fine-tuned model ID:
      ```python
      model_id = "your-fine-tuned-model-id"
   4. Run the evaluation script:
      ```python
      python evaluate_fine_tuned.py
      
## Expected Output
```python
Accuracy: 1.00
Precision: 1.00
Recall: 1.00
F1 Score: 1.00
