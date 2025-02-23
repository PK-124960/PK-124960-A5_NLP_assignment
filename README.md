# 🤖 Optimization Human Preference 

## 📌 Overview  
This project implements an **AI Response Evaluator** using a **GPT-2 model fine-tuned with Direct Preference Optimization (DPO)**.  

The model:  
- Generates **AI responses** based on user input.  
- Evaluates **response relevance** using a trained **reward model**.  
- Provides a **confidence score** (higher means better relevance).  

The project is built using **Python**, incorporating **PyTorch, Transformers (Hugging Face), Streamlit**, and other essential libraries.

---

## ✨ Features  
- ✅ **Fine-tuned GPT-2 model** for response generation.  
- ✅ **Reward model** that scores AI-generated responses.  
- ✅ **Modern & Interactive Web UI** built with Streamlit.  
- ✅ **Customizable for different preference datasets**.  
- ✅ **Easy deployment** with local model usage or Hugging Face integration.  

---

## Project Structure
```
📂 Optimization Human Preference 
│── reward_model_dpo.pth                # Trained Reward Model (Task 2)
│── app.py                              # Streamlit-based web application (Task 4)
│── A5_NLP-Assignment.ipynb             # Full training pipeline (Tasks 1, 2, 3)
│── 📂 results
│   ├── Test01.png                        # Sample prediction result 1
│   ├── Test02.png                        # Sample prediction result 2
│   ├── Test03.png                        # Sample prediction result 3
│   ├── Test04.png                        # Sample prediction result 4
│── README.md                             # Project Documentation

```

---

## Installation
### 1. Clone the repository
```bash
git clone https://github.com/PK-124960/PK-124960-A5_NLP_assignment.git
cd PK-124960-A5_NLP_assignment
```
### 2. Download or Use Local Model
- **Option 1:** Download the trained model from Hugging Face:
git lfs install
git clone https://huggingface.co/Ponkrit/A5_NLP_Assignment
mv A5_NLP_Assignment/reward_model.pth models/
- **Option 2:** Use a locally fine-tuned model.

```

---

## Running the Web App
To launch the Streamlit web application:
```bash
streamlit run app.py
```
This will open a browser where you can input a text prompt and get a response with a confidence score.

---

## Model Training and Evaluation
### **Task 1: Finding a Suitable Dataset**
- **Dataset Used:** openai/summarize_from_feedback
- **Steps Taken:**
```
    - Selected a dataset suitable for **preference optimization.**
    - Ensured **proper preprocessing.**
    - Documented **dataset sources** and cleaning process.
📂 **Dataset Source:** Hugging Face - Summarization Feedback
```

### **Task 2: Fine-tuning SBERT for NLI**
- **Dataset Used:** openai/summarize_from_feedback
- Training loss over 10 epochs:
```
Epoch 1 Loss: 0.8682
Epoch 2 Loss: 0.7968
...
Epoch 10 Loss: 0.1715
```
- The trained model was saved as **sbert_model.pth** and **classifier_head.pth**.

### **Task 3: Model Evaluation**
- Evaluated on the **SNLI test set**, achieving the following scores:
```
Accuracy: 85.42%
Precision: 85.10%
Recall: 85.30%
F1-score: 85.20%
```

---
