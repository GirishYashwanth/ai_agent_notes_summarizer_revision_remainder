# AI Agent Prototype - Fine-tuning FLAN-T5 with LoRA
## 📌Details
Name: BHUMIREDDI GIRISH YASWANTH
University: INDIAN INSTITUTE OF TECHNOLOGY KHARAGPUR
Department: MECHANICAL ENGINEERING
   

## 📌 Project Overview
This project implements an **AI Agent Prototype** that automates academic tasks such as **summarization** and **Q&A generation**.  
The agent integrates a **fine-tuned FLAN-T5 Large model** using **LoRA (Low-Rank Adaptation)** for parameter-efficient training.

---

## 🚀 Features
- Fine-tunes **FLAN-T5 Large** for summarization and academic tasks.
- Uses **LoRA** for efficient training on limited GPU resources.
- Integrated into an **AI agent workflow** (Planner + Executor).
- Supports **summarization, Q&A generation, and task classification**.
- Evaluation with **ROUGE, BLEU, Accuracy, F1** and **human feedback**.

---

## 📂 Code Structure
1. **Environment Setup**  
   Installs required dependencies: `transformers`, `datasets`, `accelerate`, `peft`, `bitsandbytes`.

2. **Model Loading**  
   Loads `google/flan-t5-large` with Hugging Face Transformers.

3. **Dataset Preparation**  
   Preprocesses text into tokenized format for fine-tuning.

4. **LoRA Fine-tuning**  
   Applies LoRA adapters for efficient fine-tuning.

5. **Training**  
   Uses Hugging Face `Trainer` for model optimization.

6. **Inference**  
   Generates summaries and Q&A from input text.

---

## 🧩 Integration into Agent
The AI agent follows a **Planner + Executor** architecture:
- **Planner** → Decides task (summarize, generate Q&A, extract deadlines).  
- **Executor** → Runs the fine-tuned FLAN-T5 model for the selected task.

---

## ❓ Why This Fine-tuning Target?
- **Task Specialization**: Tailored for academic content.  
- **Improved Reliability**: Reduces hallucinations and irrelevant outputs.  
- **Adapted Style**: Produces structured, concise summaries.  
- **Parameter Efficiency**: LoRA enables training on smaller GPUs.

---

## 📊 Evaluation Metrics
- **ROUGE / BLEU** → Summarization & Q&A quality.  
- **Accuracy / F1** → Task classification performance.  
- **Human Feedback** → Subjective relevance and usefulness.  

---

## ⚠️ Challenges Faced
- High GPU memory requirements → frequent CUDA OOM errors.  
- Dataset quality issues (inconsistent notes, noisy text).  
- Occasional **hallucinations** in generated summaries.  
- Training instability (overfitting on small datasets).  
- Integration overhead for agent workflow.  

---

## 🔮 Future Improvements
- Multi-agent collaboration (Planner + Summarizer + Scheduler).  
- Integration with **RAG (Retrieval-Augmented Generation)** for better context.  
- Deployment as a **Gradio/Web App** for student usability.  
- Larger domain datasets for improved accuracy and reduced hallucination.

---

## 📦 Installation
```bash
pip install -U transformers datasets accelerate peft bitsandbytes
```

---

## ▶️ Usage
1. Open the notebook `Copy_of_flan_t5_large.ipynb`.  
2. Run the setup and training cells.  
3. Upload text/lecture notes for summarization.  
4. Use inference cells to generate outputs.

---

## 📝 License
This project is for **academic purposes** only.
