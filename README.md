# FinSight AI – News Research AssistantNLP
 FinSight AI – A powerful news research app using Mistral-7B, LangChain, and Hugging Face

FinSight AI is a powerful, intelligent news research assistant built using **Streamlit**, **LangChain**, and **Hugging Face Transformers**. It extracts and processes content from article URLs, embeds them using semantic search, and answers user questions using the high-performance `mistralai/Mistral-7B-Instruct-v0.1` LLM.

---

## 🚀 Features

- ✅ Accepts up to 3 news article URLs
- ✅ Extracts article content using web scrapers
- ✅ Splits and embeds content using semantic vector embeddings (`all-MiniLM-L6-v2`)
- ✅ Uses **FAISS** for fast similarity-based document retrieval
- ✅ Answers natural language questions about the content
- ✅ Built with **LangChain** and runs via **Streamlit** in **Google Colab**
- ✅ Uses the powerful `mistralai/Mistral-7B-Instruct-v0.1` model for accurate and fluent answers

---

## ⚙️ LLM Model Used

> I’ve used **`mistralai/Mistral-7B-Instruct-v0.1`** in this project since I have access to sufficient local system resources (e.g., high-memory GPUs or local inference setups).

If you’re using **Google Colab free tier or low-resource systems**, you can easily switch to one of the lighter models:

### 🔄 Suggested Alternatives:

| Model Name                          | Hugging Face ID                      | Notes                          |
|-------------------------------------|--------------------------------------|--------------------------------|
| ✅ Falcon-RW-1B                     | `tiiuae/falcon-rw-1b`                | Instruction-tuned, small GPT   |
| ✅ TinyRoberta SQuAD2              | `deepset/tinyroberta-squad2`         | QA-tuned, very fast            |
| ✅ FLAN-T5 Large (local only)      | `google/flan-t5-large`               | Best used via transformers     |
| ✅ T5 Base QA                      | `timpal0l/mdeberta-v3-base-squad2`   | Lightweight & accurate         |

---

## 🧰 Tech Stack

- [LangChain](https://www.langchain.com/)
- [Hugging Face Transformers](https://huggingface.co/models)
- [Sentence-Transformers](https://www.sbert.net/)
- [FAISS](https://github.com/facebookresearch/faiss)
- [Streamlit](https://streamlit.io/)
- [Google Colab](https://colab.research.google.com/)
- [cloudflared](https://developers.cloudflare.com/cloudflared/)

---

## 🖥️ How to Run (Google Colab)

1. Open the project in Google Colab.
2. Install dependencies:
    ```bash
    pip install streamlit langchain langchain-community transformers sentence-transformers faiss-cpu PyMuPDF feedparser
    ```
3. Save the script as `main.py`
4. Launch the app with:
    ```python
    !streamlit run main.py & !cloudflared tunnel --url http://localhost:8501
    ```

---



## 📌 Example Use Case

Paste 2–3 articles from economic or financial news. Ask questions like:
- _“What are the key takeaways?”_
- _“How will this affect the stock market?”_

You’ll get concise, context-aware answers based on the article content.

---

## 👨‍💻 Author

**Debanick Banerjee**  
_Data Scientist | AI Engineer | NLP + LLM Practitioner_  
[LinkedIn](https://www.linkedin.com/in/debanick-banerjee/) • [GitHub](https://github.com/debanick19)

---

## 📄 License

This project is licensed under the MIT License.
