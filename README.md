# Sentence Classification to detect Gender Bias
This project implements a text classification model using the Mixtral-8x7B-Instruct-v0.1 model, optimized with custom quantization and offloading settings. The aim is to classify text data efficiently while optimizing resource utilization. Detailed evaluations were conducted using confusion matrices and classification reports, providing insights into model performance.

### Introduction
This project focuses on implementing a text classification model using the Mixtral-8x7B-Instruct-v0.1, an advanced model for handling various text classification tasks. The model has been fine-tuned with quantization and offloading settings to balance accuracy and computational efficiency.

### Features
**Custom Quantization and Offloading:** Configured the model to utilize custom quantization and offloading techniques to optimize GPU/CPU utilization, allowing the model to run efficiently on limited hardware.

**Model Evaluation:** Used confusion matrices and classification reports to assess performance, providing a detailed understanding of the model's strengths and areas for improvement.

**Detailed Performance Insights:** Achieved high classification accuracy, with evaluations highlighting precision, recall, and F1-scores for each class.

### Installation
**1. Clone the repository:**
```
git clone https://github.com/Hemangichhaya/LLM-project.git
cd LLM-project
```
**2. Install dependencies:**
```
pip install -r requirements.txt
```
**3. Set up environment:**
* Ensure you have Python 3.8 or above installed.
* Install any additional dependencies required for Mixtral models.

### Dataset
* **Data Used:** The project uses a dataset with multiple text-based features such as `text`, `violence`,`directed_vs_generalized`, `gender`, `race`, `national_origin`, `disability`, `religion`, and `sexual_orientation`.
* **Data Preprocessing:** The data was cleaned and prepared, ensuring optimal input format for the Mixtral-8x7B-Instruct-v0.1 model.

### Model Configuration
* **Mixtral-8x7B-Instruct-v0.1:** A large language model optimized for text classification tasks.
* **Quantization:** Applied custom quantization settings to reduce model size without significantly impacting accuracy.
* **Offloading:** Configured offloading to balance the workload between GPU and CPU, optimizing memory usage.

### Evaluation
The model was evaluated using:
  * **Confusion Matrices:** Provided insights into the true positives, false positives, true negatives, and false negatives for each class.
  * **Classification Reports:** Detailed reports including precision, recall, F1-score, and support for each class, offering a comprehensive evaluation of model performance.

### Results
* **Accuracy:** The model demonstrated strong accuracy across various classes.
* **Detailed Metrics:** High precision, recall, and F1-scores were achieved, indicating effective classification performance.

### Usage
**1. Prepare Data:** Ensure your dataset is preprocessed and formatted correctly.
**2. Run the Model:**
```
python classify.py --config model_config.yaml
```
**3. Evaluate Results:** Use provided scripts to generate confusion matrices and classification reports.
