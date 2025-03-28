# AI-Powered PDF QA System

## 🚀 Overview
This project is a **Flask-based AI-powered Question Answering (QA) system** that processes PDF documents and allows users to ask questions based on the content. It uses **LangChain, ChromaDB, Hugging Face embeddings, and Groq's LLaMA 3 model** to provide intelligent responses.

## 🌟 Features
- 📄 **PDF Processing** – Extracts text from PDFs using `PyPDFLoader`.
- 🧠 **AI-Powered QA** – Uses **LLaMA 3** for answering user queries.
- 🔍 **Vector Database** – Stores and retrieves document embeddings with **ChromaDB**.
- 🚀 **Fast & Scalable** – Efficient embeddings with `HuggingFaceBgeEmbeddings`.
- 🌐 **CORS Enabled** – Allows cross-origin requests.

---
## 🛠️ Tech Stack
| Category        | Technologies Used |
|----------------|------------------|
| **Backend**    | Flask, Flask-CORS |
| **NLP Model**  | LLaMA 3 via Groq API |
| **Embeddings** | Hugging Face (`all-MiniLM-L6-v2`) |
| **Database**   | ChromaDB |
| **Document Processing** | LangChain, PyPDFLoader |

---
## 📂 Project Structure
```bash
project/
├── data/                   # Folder containing PDF files
├── chroma_db/              # Persistent vector database
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---
## ⚡ Getting Started

### 1️⃣ Prerequisites
- Install **Python 3.8+**
- Get a **Groq API key**
- Install dependencies

### 2️⃣ Installation
```bash
# Clone the repository
git clone https://github.com/your-repo/flask-pdf-qa.git
cd flask-pdf-qa

# Install required dependencies
pip install -r requirements.txt
```

### 3️⃣ Run the Application
```bash
python app.py
```
The server will start at `http://127.0.0.1:5000`.

---
## 🔥 How It Works
1. **Load PDFs** – The system loads all PDFs from the `data/` folder.
2. **Create Vector Database** – Extracts text, splits it into chunks, and generates embeddings.
3. **User Query** – A user sends a query via the `/ask` endpoint.
4. **Retrieve & Answer** – The chatbot finds the most relevant information and responds.

### 🖥️ API Endpoint
#### `/ask` (POST)
- **Request:** `{ "query": "Your question here" }`
- **Response:** `{ "response": "Answer from the document" }`

---
## 🔧 Configuration
To update the LLM model or embeddings:
- Modify the `initialize_llm()` function for a different **Groq model**.
- Change the `model_name` in `HuggingFaceBgeEmbeddings()` for different **sentence embeddings**.

---
## 📜 License
This project is licensed under the **MIT License**.

---
## 📬 Contact
📧 **Email:** your.email@example.com  
🐱 **GitHub:** [Your GitHub](https://github.com/KartikeyaNainkhwal)  
🔗 **LinkedIn:** [Your LinkedIn](https://www.linkedin.com/in/kartikeya-nainkhwal-6493402b0/)  

---
### ⭐ Show Your Support!
If you find this project useful, consider giving it a ⭐ on GitHub!

