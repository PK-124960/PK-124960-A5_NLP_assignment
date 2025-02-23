# 🤖 AI Response Evaluator

A **Streamlit-based web application** that demonstrates the capabilities of an AI model trained for **response generation and evaluation**. The AI generates responses based on user input and provides a confidence score using a **reward model**.

---

## 📌 **Assignment Overview**
This project is part of the **Optimization Human Preference Assignment**. The objective is to train an **AI model** using **Direct Preference Optimization (DPO)** and evaluate AI-generated responses.

The assignment consists of four key tasks:
1. **Finding a Suitable Dataset**
2. **Training a Model with DPOTrainer**
3. **Pushing the Model to Hugging Face Model Hub**
4. **Developing a Web Application**

---

## 🎯 **Task 1: Finding a Suitable Dataset**
✔️ **Selected Dataset:** `openai/summarize_from_feedback`

### ✅ **Steps Taken:**
- Selected a **publicly available dataset** for preference optimization tasks.
- Ensured **data preprocessing** was correctly implemented.
- Documented the **dataset source** and preprocessing steps.

📂 **Dataset Used:** [OpenAI Summarization Feedback Dataset](https://huggingface.co/datasets/openai/summarize_from_feedback)

---

## 🔥 **Task 2: Training a Model with DPOTrainer**
✔️ **Model Used:** `GPT-2`  
✔️ **Training Framework:** `Hugging Face Transformers`  
✔️ **Training Method:** `Direct Preference Optimization (DPO)`

### 🏗️ **Steps Taken:**
1. Implemented the **DPOTrainer** function using a **pre-trained GPT model**.
2. Fine-tuned the model using the **selected dataset**.
3. Experimented with **hyperparameters** and documented training performance.

📜 **Training Code:** See `A5_NLP-Assignment.ipynb`  
📈 **Training Results:** `reward_model.pth`

---

## 🚀 **Task 3: Pushing the Model to Hugging Face Model Hub**
✔️ **Model Uploaded to Hugging Face**  
✔️ **Public Repository Created**  
✔️ **Link to Model Added in Documentation**

🔗 **Model Link:** [Ponkrit/A5_NLP_Assignment](https://huggingface.co/Ponkrit/A5_NLP_Assignment)

---

## 🌐 **Task 4: Web Application Development**
✔️ **Framework Used:** `Streamlit`  
✔️ **Functionality:** Users input text and receive **AI-generated responses** with a **confidence score**.

### 🏗️ **Steps Taken:**
1. Developed a **Streamlit web app** to interact with the trained model.
2. Allowed users to enter a **text prompt**.
3. AI generates **responses** and provides a **confidence score**.
4. Designed a **modern and colorful UI** for **user-friendly experience**.

📜 **Web App Code:** `app.py`

---

## 💻 **How to Run the Application**
### 1️⃣ **Clone the Repository**
```bash
git clone https://github.com/your-username/AI-Response-Evaluator.git
cd AI-Response-Evaluator
