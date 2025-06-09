# ANA-ChatBot

# 🧠 AI Query Answering Assistant using Gemini API

This project is designed to generate human-like answers to user queries based on the contents of either a **shared PDF file** or a **YouTube video link**. It leverages the **Gemini API (by Google AI)** for context understanding, language modeling, and intelligent response generation.

## 🚀 Features

* 📄 Accepts **PDF** documents and parses their content.
* 📺 Supports **YouTube** video links using transcript extraction.
* 🤖 Uses **Gemini API** to analyze and generate accurate and context-aware answers.
* 💬 Interactive user interface for seamless question-answer sessions.
* 🔒 Secure handling of files and API keys.

## 📁 Project Structure

```
ana_new/
├── app.py                  # Main Streamlit or Flask app
├── utils/
│   ├── pdf_parser.py       # Parses uploaded PDF documents
│   ├── youtube_parser.py   # Extracts transcript from YouTube video
│   ├── gemini_helper.py    # Handles Gemini API queries
├── templates/              # HTML templates (if using Flask)
├── static/                 # CSS, JS, or image files
├── requirements.txt        # Python dependencies
└── README.md               # Project overview
```

## 🧰 Tech Stack

* Python 3.10+
* Google Gemini API
* Streamlit or Flask (for UI)
* PyMuPDF / PDFPlumber (for PDF parsing)
* `youtube_transcript_api` (for extracting YouTube captions)

## 🛠️ Installation

1. **Clone the Repository**

```bash
git clone https://github.com/yourusername/ana_new.git
cd ana_new
```

2. **Install Dependencies**

```bash
pip install -r requirements.txt
```

3. **Set up Gemini API**

* Get your API key from [Gemini Console](https://makersuite.google.com/).
* Store it securely in a `.env` or `secrets.toml` file:

```env
GEMINI_API_KEY=your_api_key_here
```

4. **Run the Application**

```bash
streamlit run app.py
```

## 🧪 How It Works

1. **Input**:

   * Upload a PDF file or enter a YouTube video link.
2. **Processing**:

   * Extract text content using PDF or YouTube transcript parser.
   * Send content and user query to the Gemini API.
3. **Output**:

   * Receive and display the generated answer.

## 💡 Example Use Cases

* Academic paper summarization and Q\&A
* YouTube lecture or tutorial comprehension
* Document-based chatbots or research assistants

## 🧩 Future Improvements

* Support for DOCX, PPT, and web articles
* Multilingual PDF and subtitle support
* Contextual follow-up questions (memory retention)
* Chat history and export options

## 📝 License

This project is licensed under the [MIT License](LICENSE).

