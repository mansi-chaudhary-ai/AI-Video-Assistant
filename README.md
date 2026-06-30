Zaroor, yahan dono files ka complete code ek jagah par hai. Aap inhe VS Code mein alag-alag files banakar seedha paste kar sakte hain.

### 1. `requirements.txt`

VS Code mein `requirements.txt` naam ki file banayein aur yeh copy-paste karein:

```text
# UI Framework
streamlit

# Audio & Video processing
yt-dlp
openai-whisper
torch
ffmpeg-python

# LLM Orchestration & APIs
langchain
langchain-core
langchain-community
langchain-mistralai
mistralai

# RAG & Embeddings
chromadb
langchain-huggingface
sentence-transformers

# PDF Generation
fpdf2

```

---

### 2. `README.md`

VS Code mein `README.md` naam ki file banayein aur yeh copy-paste karein:

```markdown
# AI Meeting Assistant 🎙️🤖

An intelligent meeting assistant designed to streamline your workflow by transcribing, translating, and analyzing meeting audio. Built with a robust LLM architecture, this tool not only summarizes meetings and extracts actionable insights but also allows you to interactively chat with your meeting transcripts.

## 🚀 Features

* **Flexible Audio Ingestion:** Upload local audio/video files or fetch audio directly from YouTube URLs.
* **Local Transcription & Translation:** Utilizes local OpenAI Whisper models to transcribe audio and seamlessly translate Hindi meetings into English.
* **Smart Summarization:** Leverages LangChain (LCEL) and the Mistral Free API to automatically generate concise meeting summaries, extract action items, and identify key decisions.
* **Interactive RAG Q&A:** Chat directly with your meeting transcripts! Powered by a Retrieval-Augmented Generation (RAG) pipeline using ChromaDB and Hugging Face embeddings.
* **User-Friendly Interface:** A clean, interactive web UI built entirely with Streamlit.
* **One-Click Export:** Download your final meeting reports instantly in PDF or Text format.

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **Audio Processing:** yt-dlp, FFmpeg
* **Transcription/Translation:** OpenAI Whisper (Local, PyTorch)
* **LLM & Orchestration:** Mistral Free API, Sarvam API, LangChain (LCEL)
* **Vector Database & Embeddings:** ChromaDB, Hugging Face Sentence Transformers
* **Document Generation:** FPDF2

## ⚙️ Installation & Setup

### 1. Prerequisites
Before installing the Python packages, ensure that you have **FFmpeg** installed on your system, as it is required by Whisper for audio processing.

* **Windows:** Install via [Scoop](https://scoop.sh/): `scoop install ffmpeg` or download from the official site.
* **macOS:** `brew install ffmpeg`
* **Linux (Ubuntu/Debian):** `sudo apt update && sudo apt install ffmpeg`

### 2. Clone the Repository
```bash
git clone [https://github.com/mansi-chaudhary-ai/AI-Video_Assistant.git]

```

### 3. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

```

### 4. Install Dependencies

Install all required Python packages using the provided `requirements.txt`:

```bash
pip install -r requirements.txt

```

### 5. Environment Variables

Create a `.env` file in the root directory and add your Mistral API key:

```env
MISTRAL_API_KEY=your_mistral_api_key_here

```

## 💻 Usage

Start the Streamlit application by running the following command in your terminal:

```bash
streamlit run app.py

```

1. **Input Audio:** Paste a YouTube link or upload a file.
2. **Process:** Click process to let Whisper transcribe (and translate, if it detects Hindi).
3. **Analyze:** View the generated summary, action items, and key decisions.
4. **Chat:** Use the chat interface to ask specific questions about the meeting.
5. **Export:** Click the export button to save your report as a PDF or TXT file.

## 🔮 Future Enhancements

* Adding multi-speaker diarization to identify who said what.
* Support for additional languages and local LLM integration for fully offline analysis.

```

```