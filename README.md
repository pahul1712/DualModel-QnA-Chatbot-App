# **DualModel-QnA-Chatbot-App**

This repository contains two **Streamlit-based interactive Q&A chatbots** powered by [LangChain](https://www.langchain.com/).  
- **OpenAI Chatbot** → Uses OpenAI models (`gpt-5`, `gpt-4.1`, etc.)  
- **Ollama Chatbot** → Uses open-source models (`mistral`, `phi3`, `gemma3`, `llama2`, `deepseek-r1`)  

Both projects demonstrate how to build flexible question-answering chatbots with customizable parameters like **temperature** and **max tokens**, while leveraging **LangSmith tracking** for observability.

---

## 📂 Repository Structure

├── 1-OpenAI Q&A ChatBot
│   └── app.py             # Streamlit app using OpenAI models
│
├── 2-Ollama ChatBot
│   └── app.py             # Streamlit app using Ollama (open-source) models
│
├── requirements.txt       # Required Python dependencies
├── .gitignore             # Ignored files (add .env, venv/, .DS_Store, etc.)
└── README.md              # Project documentation



---

## ⚡ Features
- 🌐 **Streamlit UI** – clean interface with sidebar settings  
- 🧠 **LangChain Integration** – for prompt management and chaining  
- 🔍 **LangSmith Tracking** – monitor prompts, traces, and projects  
- 🔑 **Environment Variables** – API keys loaded from `.env` file  
- ⚙️ **Customizable Parameters**:
  - Choose different models
  - Adjust **temperature** (creativity)
  - Adjust **max tokens** (response length)

---

## 🚀 Setup Instructions

### 1. Clone the Repository

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name


### 2. Create Virtual Environment

python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows


### 3. Install Dependencies

pip install -r requirements.txt


### 4. Setup Environment Variables

Create a .env file in the root directory:

LANGCHAIN_API_KEY=your_langchain_api_key
OPENAI_API_KEY=your_openai_api_key   # only needed for OpenAI chatbot


## ▶️ Running the Apps

- OpenAI Chatbot

  cd "1-OpenAI Q&A ChatBot"
  streamlit run app.py

- Ollama Chatbot
  cd "2-Ollama ChatBot"
  streamlit run app.py


## 🖼️ App Previews

### OpenAI Q&A Chatbot

- Choose between gpt-5, gpt-5-mini, gpt-5-nano, gpt-4.1
- Enter your OpenAI API key via the sidebar


### Ollama Q&A Chatbot

- Select from open-source models like mistral:latest, phi3:latest, gemma3:latest, llama2:latest, deepseek-r1:7b
- No external API key required (runs locally with Ollama)


## 📌 Future Enhancements

- Add RAG (Retrieval-Augmented Generation) with vector stores
- Support for file-based Q&A (PDFs, CSVs, etc.)
- Add Docker setup for easier deployment


## 👤 Author
**Pahuldeep Singh Dhingra**  
🎓 MS in Data Science & Analytics, Florida Atlantic University  
🔗 [LinkedIn](https://www.linkedin.com/in/pahuldeepsing/) | [GitHub](https://github.com/pahul1712)

---

⭐ If you found this repo helpful, don’t forget to **star it**!

