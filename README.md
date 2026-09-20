# Hi, I'm Afnan 👋

I'm studying Computer Science and Data Science at Rutgers University–New Brunswick, finishing in 2027 on a three-year track.

Most of what I build is some mix of machine learning and web work. I like problems where the hard part is the data rather than the model, and I care a lot about evaluating things honestly instead of reporting the number that looks best.

**Looking for Summer 2027 software engineering and tech consulting internships.**

---

## What I'm up to

- **Lab Supervisor** at Rutgers Office of Information Technology, since Sept 2024
- **Student Community Manager** at the Rutgers Coding and Social Lounge, since Aug 2026
- **Part-Time Lecturer** for Data Science in the Rutgers CS Department, Sept 2025 to May 2026
- Building retrieval-based tooling to help IT staff resolve tickets faster

---

## Get in touch

- **Email:** [smafnanhaider@gmail.com](mailto:smafnanhaider@gmail.com)
- **Portfolio:** [smafnanhaider.com](https://smafnanhaider.com) · [Resume (PDF)](https://smafnanhaider.com/resume.pdf)
- **LinkedIn:** [linkedin.com/in/AfnanHaider](https://linkedin.com/in/AfnanHaider)

---

## Projects

### [ServiceNow Ticket Assistant](https://smafnanhaider.com/projects/servicenow-rag-assistant) · [code](https://github.com/Afn377/ServiceNow-Ticket-RAG)
A Chrome extension that reads the open ServiceNow incident and suggests troubleshooting steps in a side panel, each with knowledge-base citations and a SUPPORTED / INFERRED / UNCERTAIN label. It searches 1,394 KB articles with BGE embeddings and category-aware ranking, and abstains when the evidence is too weak. It's retrieval-based rather than fine-tuned, and it advises technicians rather than acting on its own.

- **94.5% top-5 hit rate** and **0.845 MRR** on 200 hand-written eval tickets. These measure article retrieval, not ticket resolution.
- FastAPI backend on AWS; PII is redacted client-side before a ticket leaves the browser

`Python` `FastAPI` `RAG` `Chrome Extension` `Docker` `AWS`

---

### [ProfIQ](https://smafnanhaider.com/projects/profiq) · [live demo](https://profiq.smafnanhaider.com) · [code](https://github.com/Afn377/ProfIQ)
A tool for searching and comparing professors using review sentiment, recurring review themes, and recommendations of similar professors.

- Resumable ETL pipeline over the RateMyProfessors GraphQL API, handling pagination, checkpointing, and deduplication across **1.7M+ professor records**
- Sentiment scoring on **350K+ student reviews** with a VADER rule engine and a TF-IDF / logistic-regression classifier (**80.2% accuracy**); DistilBERT was evaluated offline only
- Similar-professor recommendations built from MiniLM embeddings of review text (**4.17x** department-purity lift over random)

`Python` `Django` `React` `PostgreSQL` `PyTorch` `scikit-learn` `Hugging Face`

---

### [UCL Match Forecasting](https://smafnanhaider.com/projects/ucl-match-forecasting) · [code](https://github.com/Afn377/UCL-Predictor)
A pipeline that forecasts regulation-time Champions League outcomes as home / draw / away probabilities, using leak-safe features (Elo, form, xG, rest, congestion) built only from information available before kickoff.

- Five models compared on the same 966 fixtures: football-only logistic reaches **59.8%** vs. a **47.4%** base rate, within 2.4 points of closing odds
- These are retrospective development results, not an untouched holdout, and closing odds remain the hardest benchmark to beat
- An append-only SQLite ledger records predictions before kickoff so they can be scored later

`Python` `pandas` `scikit-learn` `SQLite`

---

## Tools I use

**Languages** · Python, SQL, JavaScript
**ML / Data** · PyTorch, scikit-learn, Hugging Face, pandas, sentence-transformers
**Web** · Django, FastAPI, React, Next.js, PostgreSQL
**Other** · AWS, Git, Docker, MCP

---
