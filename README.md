Here’s a complete `README.md` for the project Enhancing Fake News Detection with Retrieval Augmented Generation (RAG) for Fact Verification in U.S. Political News.
It includes:

- ✅ Installing dependencies  
- 🚀 Running the scraper  
- 🌐 Starting a Streamlit app
- 🧠 Uploading the file  
- 💬 Chatting with the data  

---

```markdown
# 🕵️‍♂️ FactCheck.org and Politifact Scraper & Chatbot

This project scrapes articles from [FactCheck.org](https://www.factcheck.org), PolitiFact (https://www.politifact.com/factchecks/) and lets you interact with the data using a Streamlit chatbot interface powered by a Google AI model.

---

## 🧰 Setup Instructions

### 1. Clone the Repository

```bash
unzip(extract) the news_assistant.zip
cd news_assistant
```

---

### 2. Create and Activate a Virtual Environment

#### 🪟 On Windows:
```bash
python -m venv venv
venv\Scripts\activate
```

#### 🍎 On macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4. Set Up Your Google API Key

To use the chatbot (with Google Gemini or similar), you need a `GOOGLE_API_KEY`.

#### 🛠 How to Get One:

1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey).
2. Sign in and generate a new API key.
3. Copy the key.

#### 🔐 Create a `.env` File

In the project root, create a `.env` file:

```
GOOGLE_API_KEY=your_real_api_key_here
```

> Make sure to never share your API key publicly.

---

## 🧹 Run the Scraper

```bash
python factcheck_scraper.py
```

This will scrape articles and save them in `scraped_results/` as:
- `factcheck_articles.csv`

```bash
python politifact_scraper.py
```

This will scrape articles and save them in `scraped_results/` as:
- `politifact_articles.csv`

---

## 💬 Start the Chatbot

```bash
streamlit run chat_app.py
```

Then your default browser will open automatically with the chat UI.

---

## 📁 Upload the File & Start Chatting

1. In the Streamlit app, click **"Browse files"**
2. Upload `scraped_results/factcheck_articles.csv` or `.xlsx`
3. Ask anything about the articles!

---
