# 🧾 Legal Text Summarization using GPT Models

This project performs **abstractive summarization** of Indian legal documents using various large language models (LLMs) including **GPT-2, GPT-Neo, OPT**, and **Pythia**. The models are compared on their performance in summarizing complex legal case descriptions from the **FD_IND dataset**.

---

## 📌 Objective

To evaluate the effectiveness of different open-source LLMs in generating coherent and concise summaries of factual legal case descriptions, and identify which model best captures the legal context.

---

## 📂 Dataset

- **Name:** FD_IND (Fact Description – Indian Legal Dataset)
- **Description:** Contains fact descriptions, charges, and judgments from Indian criminal court cases.
- **Usage:** Only the `facts` field was used as input to generate abstractive summaries.

---

## 🧠 Models Used

| Model     | Provider         | Size     |
|-----------|------------------|----------|
| GPT-2     | OpenAI/Hugging Face | 124M     |
| GPT-Neo   | EleutherAI        | 125M     |
| OPT       | Meta AI           | 125M     |
| Pythia    | EleutherAI        | 160M     |

All models were accessed via [Hugging Face Transformers](https://huggingface.co/transformers/).

---

## 📈 Evaluation Metric

- **ROUGE Scores** (ROUGE-1, ROUGE-2, ROUGE-L)
- Best Performance by **GPT-2**:
  - ROUGE-1: `0.547`
  - ROUGE-2: `0.2501`
  - ROUGE-L: `0.2481`

---

## ⚙️ Technologies Used

- Python
- Hugging Face Transformers
- PyTorch
- ROUGE Score (via `evaluate` library or `rouge-score`)
- Jupyter Notebook
