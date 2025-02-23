# Optimization Human Preference 🧠🤖

This repository contains the implementation of an **AI Response Evaluator** built using **Streamlit** and **PyTorch**. The application generates AI responses based on user input, evaluates their relevance using a scoring model, and provides an interactive UI for easy assessment.

---

## 📜 Assignment Details

- **Course:** AT82.05 - Artificial Intelligence: Natural Language Understanding (NLU)
- **Assignment:** A5 - Optimization Human Preference
- **Instructor:** Chaklam Silpasuwanchai, Todsavad Tangtortan
- **Objective:** Use **Direct Preference Optimization (DPO)** to train a model that aligns AI-generated responses with human preferences.
- **Deadline:** One-week assignment (Start early!)
- **Deliverables:**
  - GitHub repository with Jupyter Notebook (`A5_NLP-Assignment.ipynb`).
  - **README.md** (this document).
  - Web application folder (`app/`).
- **Hugging Face Model Link:** [A5_NLP_Assignment Model](https://huggingface.co/Ponkrit/A5_NLP_Assignment)

---

## 🚀 Project Overview

The **AI Response Evaluator** allows users to:
- Input a text prompt and generate AI responses.
- Evaluate the response using a **trained reward model** based on **Direct Preference Optimization (DPO)**.
- Display AI confidence scores to measure response relevance.
- Provide a **modern UI** with an intuitive evaluation system.

---

## 🏗️ Project Structure


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

## 🎯 Assignment Tasks & Implementation

### 🔹 Task 1: Finding a Suitable Dataset (0.5 point)
- Selected **a preference-based dataset** from the **Hugging Face Datasets Hub**.
- Preprocessed the dataset for training a **Direct Preference Optimization (DPO)** model.
- Documented the dataset source and preprocessing steps.

### 🔹 Task 2: Training a Model with DPOTrainer (2 points)
- Implemented **DPOTrainer** using a pre-trained **GPT-2** model.
- Fine-tuned the model using the selected dataset.
- Experimented with **hyperparameters** and reported **training performance**.

📌 **Reference**: [Hugging Face DPOTrainer Documentation](https://huggingface.co/docs/trl/main/dpo_trainer)

### 🔹 Task 3: Pushing the Model to Hugging Face Hub (0.5 point)
- Saved the trained model.
- Uploaded the model to **Hugging Face Model Hub**.
- Provided the link in the documentation.

📌 **Reference**: [How to Upload Models to Hugging Face](https://huggingface.co/docs/hub/models-uploading)

### 🔹 Task 4: Web Application Development (1 point)
- Developed a **Streamlit web application** to demonstrate the trained model’s capabilities.
- Users can **input text** and receive an AI-generated **response + relevance score**.
- Applied **modern UI styling** for a **smooth user experience**.

---

## 📸 Screenshots

### 🏙️ Example 1: Simple Question
![Test01](images/Test01.png)

### 💬 Example 2: Casual Conversation
![Test02](images/Test02.png)

### 🍕 Example 3: Opinion-based Question
![Test03](images/Test03.png)

### 🐍 Example 4: Coding-related Question
![Test04](images/Test04.png)

---

## ⚙️ Installation & Setup

To run this project locally, follow these steps:

1️⃣ **Clone the repository**:
   ```bash
   git clone https://github.com/your_username/AI-Response-Evaluator.git
   cd AI-Response-Evaluator
   ```
2️⃣ **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3️⃣ **Download the trained model from Hugging Face**:
   ```bash
   git lfs install
   git clone https://huggingface.co/Ponkrit/A5_NLP_Assignment
   ```
4️⃣ **Run the Streamlit application**:
   ```bash
   streamlit run app.py
   ```
---

## 🔬 Model Details
- **Response Model**: gpt2 (Fine-tuned on a preference dataset)
- **Reward Model**: gpt2 (Used for scoring responses)
- **Evaluation Method**: Converts model logits into probability scores to determine response relevance.
  
---

## 💡 Features
✅ Generates AI responses using a fine-tuned GPT-2 model.
✅ Evaluates relevance with a reward model trained using Direct Preference Optimization (DPO).
✅ Displays confidence scores indicating the AI’s certainty in its response.
✅ Stylish UI with a gradient background and modern design.

---
