# AI Blog Generator using LLaMA2

An AI-powered blog generation application built with Streamlit, LangChain, and LLaMA 2 running locally using CTransformers. This project generates blogs based on topic, word count, and target audience without relying on paid APIs.

## 🚀 Features
- 🧠 Local LLaMA 2 model inference (No API key required)
- ✍️ Blog generation with customizable:
  - Topic
  - Number of words
  - Writing style (Researchers, Data Scientist, Common People)
- ⚡ Fast inference with model caching
- 🖥️ Simple & interactive Streamlit UI
- 🔒 Fully offline & privacy-friendly
- 🔮 Ready for future RAG & embedding integration

## 🏗️ Tech Stack
- Python 3.9+
- Streamlit – Frontend UI
- LangChain – Prompt orchestration
- CTransformers – Local LLM inference
- LLaMA 2 (GGML / GGUF) – Language Model
- Sentence-Transformers – Embeddings (for future RAG)

## 📂 Project Architecture

```bash
AI-Blog-Generator/
│
├── model/
│   └── llama-2-7b-chat.ggmlv3.q8_0.bin   # LLaMA 2 model file
│
├── app.py                               # Streamlit application
├── requirements.txt                    # Project dependencies
├── README.md                            # Project documentation
└── .gitignore                           # Ignored files & folders
```

## ⚙️ Installation & Setup

1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/ai-blog-generator.git
cd ai-blog-generator
```
2️⃣ Create Virtual Environment (Recommended)
```bash
conda create -n ai_blog_env python=3.9 -y
```
4️⃣ Activate Environment
```bash
conda activate ai_blog_env
```
3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

## 📥 Download LLaMA 2 Model
Download a compatible GGML / GGUF model and place it inside the model/ folder.
Example:
```bash
model/llama-2-7b-chat.ggmlv3.q8_0.bin
```
⚠️ Make sure your system has enough RAM (8GB+ recommended).

## ▶️ Run the Application
```bash
streamlit run app.py
```
Open browser:
```bash
http://localhost:8501
```

## 🧪 How It Works
1. User enters blog topic
2. Selects word limit and target audience
3. Prompt is dynamically created using LangChain
4. LLaMA 2 model generates blog locally
5. Output is displayed in Streamlit UI

## 📌 Example Prompt
Write a blog for a Data Scientist job profile on the topic "Generative AI" within 500 words.

## 🔮 Future Enhancements
- ✅ RAG (Retrieval-Augmented Generation)
- ✅ Vector database integration (FAISS / ChromaDB)
- ✅ Multi-model selection
- ✅ Download blog as .txt or .md
- ✅ FastAPI backend

## 🧑‍💻 Author
Chintan Dabhi
MCA Student | AI & ML Enthusiast

## ⭐ Support
If you find this project useful, please ⭐ star the repository and share it!

## 📜 License
This project is licensed under the MIT License.
