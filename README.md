
# RAG App Demo

A simple web application built with **Streamlit** and **LangChain** that uses Retrieval-Augmented Generation (RAG) to answer questions based on documents retrieved from URLs.

---

## 🚀 Features

- **Load documents from URLs:** Extract and process textual content from websites.
- **Document splitting:** Uses an optimized system to split content into chunks.
- **Vector database:** Indexes content using OpenAI embeddings and manages it with ChromaDB.
- **AI model:** Answers questions using OpenAI GPT models based on retrieved documents.

---

## 🛠️ Requirements

1. **Python 3.8+**
2. **OpenAI API Key**  
   Sign up on [OpenAI](https://openai.com/) to get your API key.

---

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/username/repository-name.git
   cd repository-name
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up the `.env` file**
   Create a `.env` file in the root directory and add your OpenAI API key:
   ```env
   OPENAI_API_KEY=your_openai_api_key
   ```

---

## ▶️ Run the App

Run the Streamlit app with the following command:
```bash
streamlit run app.py
```

The app will be accessible in your browser at `http://localhost:8501`.

---

## 📂 Repository Structure

```
repository-name/
│
├── app.py            # Main application code
├── README.md         # Project documentation
├── requirements.txt  # Project dependencies
└── .env              # Environment variables (to be created manually)
```

---

## 🤖 How It Works

1. **Document loading:**  
   Content from the specified URLs is fetched and processed.
   
2. **Vector database creation:**  
   Documents are split into chunks and indexed using OpenAI embeddings.

3. **Retrieval and answering:**  
   User queries trigger the retrieval of relevant documents. The AI model generates a response based on the provided context.

---

## 📋 Important Notes

- **Supported URLs:**  
  The app works best with accessible, text-based content. Complex URLs or sites with anti-scraping measures may not work properly.
  
- **Model limitations:**  
  Ensure you have sufficient balance to use the OpenAI API. Intensive usage may incur costs.

