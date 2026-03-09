# AssignmentOSSD_Phedra

Final assignment for the **Open Source Software Development** course — Saigon University, 2026.

This project implements a **RAG (Retrieval-Augmented Generation)** system that allows users to upload PDF documents and ask questions about their content. The system uses the Qwen2.5:7b language model via Ollama, multilingual embeddings, and a FAISS vector database — running entirely offline on a local machine.

---

## Tech Stack

- **Backend**: Django 4.2
- **RAG Pipeline**: LangChain
- **LLM**: Qwen2.5:7b via Ollama
- **Embeddings**: paraphrase-multilingual-mpnet-base-v2 (HuggingFace)
- **Vector Store**: FAISS
- **PDF Parsing**: PDFPlumberLoader
- **Frontend**: HTML/CSS (Django Templates)

---

## Project Structure

```
AssignmentOSSD_Phedra/
├── myapp/                  # Main Django application
│   ├── static/myapp/       # CSS, images, PDF resume
│   ├── templates/myapp/    # HTML templates
│   ├── views.py
│   └── ...
├── simply/                 # Django project settings
├── manage.py
└── requirements.txt
```

---

## Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/myphedra/AssignmentOSSD_Phedra.git
cd AssignmentOSSD_Phedra
```

**2. Create and activate virtual environment**
```bash
python3 -m venv myenv
source myenv/bin/activate        # macOS/Linux
myenv\Scripts\activate           # Windows
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

**4. Run the development server**
```bash
python3 manage.py runserver
```

Visit `http://127.0.0.1:8000` in your browser.

---

## Deployment

The application is deployed on **AWS EC2** (Ubuntu) with Nginx as the web server.

Live URL: `http://3.27.10.42:8000`

---

## Author

**Phedra Nguyen** — Software Engineering Student, Saigon University  
Faculty of Information Technology