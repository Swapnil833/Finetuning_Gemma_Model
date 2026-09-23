# 🤖 Gemma 2B Fine-Tuning

This project demonstrates fine-tuning the Gemma 2B language model using **KerasNLP and TensorFlow** in Google Colab.

The model is fine-tuned on the **Databricks Dolly 15K instruction dataset** using **LoRA (Low-Rank Adaptation)** and quantization for more efficient training.

## 🛠️ Tech Stack

| Technology               | Purpose                           |
| ------------------------ | --------------------------------- |
| **Python**               | Programming language              |
| **Gemma 2B**             | Base language model               |
| **KerasNLP**             | Model loading and text generation |
| **TensorFlow / Keras**   | Model training                    |
| **LoRA**                 | Parameter-efficient fine-tuning   |
| **Databricks Dolly 15K** | Training dataset                  |
| **Google Colab**         | GPU-based training                |

## 🔄 Workflow

```text
Dolly 15K Dataset
       ↓
Data Preprocessing
       ↓
Load Quantized Gemma 2B
       ↓
Enable LoRA
       ↓
Fine-Tune Model
       ↓
Generate Response
```

## 🚀 How to Run

### 1. Open the Notebook

Open the `Gemma finetuning with colab.ipynb` notebook in **Google Colab**.

### 2. Enable GPU

In Colab, go to:

**Runtime → Change runtime type → GPU**

### 3. Install Dependencies

```bash
pip install -q -U keras-nlp
pip install -q -U keras
```

### 4. Configure Kaggle

Add your `kaggle.json` credentials to access the Gemma model.

> **Do not upload your API credentials to GitHub.**

### 5. Run the Notebook

Execute the notebook cells sequentially to:

1. Load the dataset.
2. Preprocess the instruction-response data.
3. Load the quantized Gemma 2B model.
4. Enable LoRA fine-tuning.
5. Train the model.
6. Generate responses using the fine-tuned model.

## 🧠 Key Concepts

* **Gemma 2B** — Pre-trained language model.
* **LoRA** — Fine-tunes a small number of additional parameters instead of the entire model.
* **Quantization** — Reduces memory requirements during model loading.
* **Top-K Sampling** — Used for generating responses from the fine-tuned model.
