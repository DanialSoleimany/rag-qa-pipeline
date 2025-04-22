# 🌟 RAG Question-Answering System with Gemini | Seven Wonders of the Ancient World 🏛️

This project showcases a **Retrieval-Augmented Generation (RAG)** pipeline that answers questions about the **Seven Wonders of the Ancient World** by combining **document retrieval** with **LLM-based generation**.

Powered by **Haystack**, **Google Gemini**, and **Sentence-Transformers**, this system fetches relevant historical documents and generates insightful answers.

---

## 🚀 Features

- **Document Retrieval**: Fetches Wikipedia content on the Seven Wonders (preprocessed dataset).
- **Embedding with Sentence-Transformers**: Uses `all-MiniLM-L6-v2` for both documents and queries.
- **Vector Search**: Retrieves relevant documents based on query embeddings.
- **Prompt Engineering**: Custom Jinja2-based prompts to provide rich context for the LLM.
- **LLM Generation with Gemini**: Integrates **Google Gemini (gemini-2.0-flash)** for high-quality answers.
- **Pipeline Architecture**: Modular design using **Haystack** components.

---

## 🛠️ Tech Stack

- **Haystack**: Orchestrates the pipeline (retriever, embedder, generator).
- **Google Gemini**: LLM for generating answers.
- **Sentence-Transformers**: Embedding model for documents and queries.
- **Hugging Face Datasets**: Preprocessed Wikipedia dataset on the Seven Wonders.

---

## 📄 Pipeline Overview

1. **DocumentStore**: Stores preprocessed Wikipedia pages with embeddings.
2. **Embedder**: Embeds both documents and queries using `sentence-transformers/all-MiniLM-L6-v2`.
3. **Retriever**: Retrieves the most relevant documents based on query embeddings.
4. **PromptBuilder**: Constructs prompts by combining document content and user questions.
5. **ChatGenerator**: Uses **Google Gemini** to generate answers from the prompts.

---

## ⚙️ How to Run

1. **Install Dependencies:**

```bash
pip install haystack-ai google-ai-haystack datasets sentence-transformers
```

2. **Get your Google API Key**  
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)  
   - Set the key as an environment variable:  
   ```bash
   export GOOGLE_API_KEY="your_api_key_here"
   ```

3. **Run the Notebook:**  
   Open `RAG_Pipeline.ipynb` and follow along step by step!

---

## ❓ Sample Query

> **Question:** Why did people visit the Temple of Artemis?  
> **Answer:** The Temple of Artemis was visited as a place of worship and pilgrimage, known for its grandeur and dedication to the goddess Artemis.

---

## 📚 References

- [Haystack Documentation](https://docs.haystack.deepset.ai/docs)
- [Google Gemini](https://makersuite.google.com/)
- [Seven Wonders Dataset](https://huggingface.co/datasets/bilgeyucel/seven-wonders)

---

## 🤝 Contributing

Feel free to fork the repo, open issues, or submit pull requests! Let’s enhance this system together!

---

## 📢 Connect with Me

Let’s discuss more about **RAG systems**, **LLMs**, or **NLP pipelines**!  
Find me on [LinkedIn](#) or feel free to reach out.

---

Let me know if you want to customize any section further (like **About Me**, **License**, etc.)! 🚀
