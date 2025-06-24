# PaperTeller

**PaperTeller** is an AI-powered platform that analyzes research papers and documents, providing:
- Summaries
- Stories
- Songs
- Analytical ratings
- Strengths, weaknesses, and suggestions

It uses state-of-the-art AI models (OpenAI, Hugging Face, or your own custom model) and offers a modern web interface for researchers, students, and enthusiasts.

---

## 🚀 Features
- **Document Upload**: Supports PDF, DOCX, TXT, and RTF
- **AI Summarization**: Converts papers into concise summaries
- **Creative Conversion**: Turns research into stories or songs
- **Analysis**: Rates papers, lists strengths/weaknesses, and suggests improvements
- **Custom Model Training**: Train your own summarizer for offline, domain-specific use
- **Modern UI**: React frontend for easy interaction
- **API-first**: FastAPI backend with REST endpoints

---

## 🛠️ Tech Stack
- **Backend**: Python, FastAPI, Hugging Face Transformers, PyTorch
- **Frontend**: React.js
- **AI Models**: OpenAI GPT, Hugging Face, or custom fine-tuned models

---

## ⚡ Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/PaperTeller.git
cd PaperTeller
```

### 2. Backend Setup
```bash
cd backend
python -m venv venv
venv\Scripts\activate  # On Windows
# or
source venv/bin/activate  # On Mac/Linux
pip install -r requirements.txt
```

### 3. Frontend Setup
```bash
cd ../frontend
npm install
npm start
```

### 4. Run the Backend
```bash
cd ../backend
uvicorn main:app --reload
```

---

## 🤖 Custom Model Training (Optional)
You can train your own summarization model for offline, domain-specific use!

1. Install training dependencies:
   ```bash
   pip install -r requirements_training.txt
   ```
2. Add research papers to `backend/training_papers/`
3. Run:
   ```bash
   python train_model.py
   ```
4. Restart the backend server. The custom model will be used automatically.

---

## 🌐 API Endpoints
- `POST /upload` — Upload and extract text from a document
- `POST /convert` — Convert text to summary, story, or song
- `POST /analyze` — Get analysis, rating, and suggestions
- `GET /model-status` — Check which AI model is active

---

## 📚 Example Usage

### Summarize a Paper
```python
import requests

with open('sample.pdf', 'rb') as f:
    r = requests.post('http://localhost:8000/upload', files={'file': f})
    text = r.json()['content']

summary = requests.post('http://localhost:8000/convert', data={
    'content': text,
    'type': 'summary',
    'use_custom': 'true'
})
print(summary.json()['result'])
```

---

## 🤝 Contributing
1. Fork the repo
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

---

## 📄 License
MIT License. See [LICENSE](LICENSE) for details.

---

## 🙏 Acknowledgements
- [OpenAI](https://openai.com/)
- [Hugging Face](https://huggingface.co/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [React](https://reactjs.org/)

---

**PaperTeller — Making research accessible, creative, and insightful!** 