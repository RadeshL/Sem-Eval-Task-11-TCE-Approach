# SemEval Task 11 2026 - Natural Language Inference and Syllogistic Reasoning

## Overview

This project implements solutions for SemEval Task 11 2026, focusing on natural language inference and syllogistic reasoning. The task involves assessing the logical validity of textual arguments and syllogisms using both machine learning and rule-based approaches.

## Project Structure

### 📁 Dataset Creation
- **`Train_dataset_creation.ipynb`** - Notebook for creating training datasets from raw premise-hypothesis pairs
- **`training.csv`** - Raw training data with premise statements
- **`actual_training.csv`** - Canonical form representations of logical relationships
- **`train_data.json`** - Structured training data with validity and plausibility labels
- **`training_t5.jsonl`** - T5-formatted training data in JSONL format

### 📁 Model Implementation
- **`Model_fine_tune.ipynb`** - T5 model fine-tuning for natural language inference
- **`Model_rule_based.ipynb`** - Rule-based approach for logical validity assessment
- **`t5_logic/`** - Directory containing T5 model weights and configuration files

### 📁 Output Files
- **`output.csv`** - Model predictions and evaluation results
- **`training2.csv`** - Additional training data subset

## 🚀 Features

### Machine Learning Approach
- **T5-based fine-tuning** for text-to-text natural language inference
- **Custom dataset preprocessing** for syllogistic reasoning tasks
- **JSONL format** compatibility with T5 training pipeline

### Rule-Based Approach
- **Logical pattern matching** for syllogism validation
- **Canonical form extraction** and analysis
- **Type-based reasoning** (A, E, I, O categorical propositions)

## 📊 Dataset Statistics

- **Training samples**: 2,880 premise statements
- **Canonical forms**: 5,168 logical relationships
- **Combined dataset**: 2,480 training pairs
- **Categories**: Universal affirmative (A), Universal negative (E), Particular affirmative (I), Particular negative (O)

## 🛠️ Installation

### Prerequisites
- Python 3.8+
- PyTorch
- Transformers (Hugging Face)
- Pandas
- Jupyter Notebook

### Setup
```bash
git clone https://github.com/RadeshL/Sem-Eval-Task-11-TCE-Approach.git
cd Sem-Eval-Task-11-TCE-Approach
pip install -r requirements.txt
```

## 📖 Usage

### Dataset Creation
1. Open `Train_dataset_creation.ipynb`
2. Run all cells to generate the training dataset
3. The output will be saved as `training_t5.jsonl`

### Model Fine-Tuning
1. Open `Model_fine_tune.ipynb`
2. Configure the T5 model parameters
3. Train the model on the prepared dataset
4. Evaluate performance on validation set

### Rule-Based Evaluation
1. Open `Model_rule_based.ipynb`
2. Run the logical pattern matching algorithms
3. Compare results with machine learning approach

## 🎯 Task Description

SemEval Task 11 focuses on evaluating systems' ability to:
- **Assess logical validity** of textual arguments
- **Identify syllogistic patterns** in natural language
- **Determine plausibility** of logical conclusions
- **Handle categorical propositions** with quantifiers and negations

## 📈 Evaluation Metrics

- **Accuracy**: Correct validity assessment percentage
- **Precision/Recall**: Performance per logical category
- **F1-Score**: Harmonic mean of precision and recall
- **Cross-validation**: Robustness across different splits

## 🔬 Methodology

### T5 Fine-Tuning Approach
1. **Text preprocessing** and tokenization
2. **Input-output formatting** for text-to-text generation
3. **Hyperparameter optimization** for best performance
4. **Transfer learning** from pre-trained T5 model

### Rule-Based Approach
1. **Pattern extraction** from canonical forms
2. **Logical rule application** for validity checking
3. **Type-based reasoning** for categorical propositions
4. **Syntactic analysis** of premise-conclusion relationships

## Acknowledgments

- SemEval 2026 organizers for Task 11
- Hugging Face for the Transformers library
- Research community in natural language inference


