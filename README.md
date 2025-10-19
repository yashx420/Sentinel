# 🛰️ Sentinel

> *“In a world where information is weaponized, Sentinel stands watch.”*

**Sentinel** is an open-source political bias detection system designed to expose hidden ideological leanings in modern news.  
It analyzes headlines and descriptions in real time, classifying content as **Left**, **Center**, or **Right**, helping users cut through narrative fog and recognize the shape of the message behind the words.

---

## ⚡ What Sentinel Does

- 🧠 **Bias Detection** — Uses a fine-tuned transformer model to analyze text and assign political leanings.  
- 📰 **Real-Time News Feed** — Connects to [NewsAPI](https://newsapi.org) or compatible sources to pull fresh articles.  
- 🕵️ **Heuristic Safety Net** — Combines ML predictions with sentiment and source rules to reduce misclassification.  
- 🧭 **Clear Classification** — Displays results in an interactive UI sorted into Left, Center, or Right categories.  
- 🌐 **Local & Contained** — Model runs on your machine, not the cloud.

---

## 🧱 Tech Stack

- **Frontend:** React + Axios  
- **Backend:** Python (Flask / FastAPI)  
- **Model:** Fine-tuned BERT stored in `safetensors` format  
- **NLP:** HuggingFace Transformers  
- **Extras:** Optional sentiment layer for better contextual signals

---

## 🚀 Getting Started

### 1. Clone the Project
```bash
git clone https://github.com/yourusername/sentinel.git
cd sentinel
````

### 2. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### 3. Backend Setup

```bash
cd backend
pip install -r requirements.txt
python app.py
```

### 4. Model Placement

Place your trained model in:

```
/backend/news-bias-model/
├── config.json
├── model.safetensors
├── special_tokens_map.json
├── tokenizer_config.json
├── vocab.txt
```

---

## 🧠 How Sentinel Works

1. **Ingest** — Retrieves articles from the news feed.
2. **Encode** — Combines title, description, and source into a model-ready input.
3. **Infer** — Model outputs political leaning + confidence score.
4. **Refine** — Optional heuristics (e.g., sentiment, neutral sources) adjust results.
5. **Reveal** — Articles are sorted and displayed by bias category in the UI.

---

## 🕳️ Philosophy

> “The machine doesn’t decide truth.
> It shows where the fingerprints are.”

Sentinel is not a fact-checker or censorship tool.
It is a **lens** — meant to reveal linguistic and ideological signals so humans can judge more clearly.

---

## 🧭 Roadmap

* [ ] Topic-based clustering of narratives
* [ ] More granular bias scale (beyond L / C / R)
* [ ] Confidence visualization
* [ ] Multilingual model support
* [ ] Real-time dashboard mode

---

## ⚠️ Disclaimer

Sentinel is a **research and transparency** tool.
Its classifications reflect linguistic patterns — not objective truth.
Use it to **analyze**, not to censor or oversimplify complex narratives.

---

## 🤝 Contributing

Contributions are welcome.
Help make the lens sharper.

```bash
git checkout -b feature/your-feature
git commit -m "Add feature"
git push origin feature/your-feature
```

---

## 📜 License

MIT License © 2025 — **Sentinel Project**

> *“Every signal leaves a trace.”*
