# ARPAN MAJUMDAR — Master Resume (Full Source)

## CONTACT
+91-9635082849 | arpanmajumdar952@gmail.com
LinkedIn | GitHub | Google Scholar | Kaggle

## PROFESSIONAL SUMMARY OPTIONS
Use the one that matches the target role:

### For ML Engineer roles:
ML Engineer with 2+ years training and deploying production transformer 
models across speech, NLP, and computer vision. Deep expertise in 
fine-tuning WavLM, XLM-RoBERTa, Wav2Vec2, and ViT with multi-task 
learning, AMP mixed-precision, staged unfreezing, and full MLOps 
pipelines. Published ACL 2025 & CLEF 2025. Global rankings 9th & 22nd.

### For AI Engineer roles:
AI Engineer with 2+ years architecting 10+ production-grade AI systems 
spanning forensic speech, real-time deepfake detection, agentic RAG, 
and multimodal meeting intelligence. Expert in Django/FastAPI backends, 
WebSocket pipelines, asyncio concurrency, PyTorch deployment.

### For GenAI Engineer roles:
Generative AI Engineer with 2+ years designing LLM-powered applications,
production RAG pipelines, and agentic AI systems. Delivered 10+ systems 
integrating GPT-4o, Gemini 1.5/2.0, LLaMA3 70B, Qwen-32B, DeepSeek. 
Deep expertise in FAISS, Milvus, prompt engineering, multi-modal LLM 
orchestration.

### For Data Scientist roles:
Data Scientist with 2+ years industry and research experience in 
predictive modeling, NLP, LLMs, and scalable data pipelines. Production 
credit risk models (R²=97.7%), LLM-powered extraction pipelines, 
multilingual transformer systems. Published ACL 2025 & CLEF 2025.

## TECHNICAL SKILLS

### ML Frameworks
PyTorch, TensorFlow, Hugging Face Transformers, Scikit-learn, XGBoost,
LightGBM, Keras, SpeechBrain

### Model Training
Fine-Tuning, Multi-Task Learning, AMP Mixed Precision, Cosine Warmup,
Gradient Clipping, Label Smoothing, EarlyStopping, LoRA/QLoRA

### Speech & Audio
WavLM, ECAPA-TDNN, Wav2Vec2, Whisper, Silero VAD, pyannote 3.1,
Librosa, FFmpeg, Praat/Parselmouth

### NLP & Transformers
BERT, XLM-RoBERTa, SciBERT, MuRIL, IndicBERT, MiniLM, GPT-4o,
Gemini 1.5/2.0/2.5, LLaMA3, Qwen-32B-AWQ, DeepSeek-R1, Claude,
FAISS, Milvus, LangChain, RAG, ReAct Agents

### Embeddings & Vector DBs
BGE-M3, MiniLM, Gemini Embedding API (3072-dim), FAISS,
Milvus (HNSW, M=16), pgvector, Algolia, Supabase

### Backend & APIs
Django (ASGI/Channels/DRF), FastAPI, Flask, WebSockets, REST APIs,
Celery, Redis, HTMX, LiveKit

### Computer Vision
MediaPipe Face Mesh, OpenCV, ViT-CNN Hybrid, ViT-base

### MLOps & Cloud
MLflow, Docker, AWS (S3/RDS/EC2), Linux VPS, Kaggle GPU (T4), Git,
Nginx, Celery, Redis

### Data & Languages
PySpark, Hadoop, Pandas, NumPy, Feature Engineering, ETL Pipelines
Python, R, SQL, C, JavaScript (basic), Linux/Bash

### Visualization
Tableau, Power BI, Matplotlib, Seaborn, Excel

## PROFESSIONAL EXPERIENCE

### Ramakrishna Mission Vidyamandira (Industry Collaboration)
**Role:** ML Engineer / AI Engineer / GenAI Research Engineer
**Location:** Howrah, WB | **Period:** Aug 2025 – Present
**Supervisor:** Dr. Arindam Sarkar

**Audio Deepfake Detection — Multi-Task Model:**
- Unified 4 datasets (ASVspoof 2019 LA/2021 DF, Fake-or-Real, WaveFake)
  into 134k+ sample manifest
- Corrected mislabeled bonafide samples (+43% real data recovery → 56,710
  real samples)
- Architected WavLM-Base-Plus (94M params) with 12-layer learnable 
  attention aggregation + 2-layer 8-head Transformer encoder + attentive
  statistics pooling
- Joint real/fake + 7-way codec + 4-way attack-family classification
- 2-stage training: 5 frozen + 15 full-tuning epochs
- AdamW + cosine warmup + AMP mixed-precision + label smoothing on Kaggle T4

**Speech Emotion Recognition Model:**
- Fine-tuned WavLM-Base-Plus on 9,587 utterances (RAVDESS, CREMA-D, 
  TESS, SAVEE)
- Softmax layerwise attention across all 12 transformer layers
- Self-attention pooling, 2-layer MLP (768→384→6) + LayerNorm + Dropout(0.3)
- Staged unfreezing at epoch 4
- Production augmentation: Opus codec 16–64 kbps, telephony bandpass 
  300–3400 Hz, 2–10% packet loss, reverberation
- Result: Weighted F1=0.7105, best-class anger F1=0.8197, neutral recall=0.8863

**SWAR CHIHNAYAN — Forensic Speaker Recognition System:**
- Architected offline-first Django + Celery + Redis backend
- ECAPA-TDNN (6.19M params) + dual-pass scanning (600s sparse + 1.5s 
  sliding window)
- Gatekeeper cosine-similarity algorithm (85/15 dynamic embedding mixing)
- Strict Validator: mathematically guaranteed zero false-positives
- Reduced investigation time 93% (8 hrs → 30–45 min)
- HTMX + WaveSurfer.js frontend with court-admissible timestamped 
  PDF/WAV/JSON evidence packages

**Neuro-Symbolic Agentic RAG — Embedding & Retrieval Pipeline:**
- Dual-LLM architecture: Qwen-32B-AWQ reasoner + DeepSeek-R1-7B critic
- ReAct (Reason+Act) agentic loop with custom tool registry
  (hybrid_search, expand_context, critique, database_stats)
- GPU-accelerated BGE-M3 pipeline: 1024-dim L2-normalized dense vectors
  (64 chunks/batch, NaN/Inf/zero-vector validation)
- BGE-Reranker-v2-M3 cross-encoder re-ranking
- Milvus HNSW (M=16, efConstruction=200, 20+ schema fields including 
  scalar & JSONB array fields)
- Multi-angle query expansion & police-jargon translation
- 3-stage retrieval: bi-encoder + reranker + smart context stitching

**FACE_MEET — Real-Time Multimodal Meeting AI:**
- Django 5 + Channels + DRF + LiveKit platform
- Captures PCM/YUV streams via WebSockets
- Concurrent asyncio: WavLM emotion inference + multi-task audio deepfake
  detection + ViT-CNN video deepfake pipeline
- MediaPipe face mesh, lip/eye crops, 5-frame score smoothing
- Live fraud verdict overlay ("AUDIO DETECTED FAKE")
- ReportLab PDF reports with LOW/MEDIUM/CRITICAL risk scoring

**AI Interview System:**
- FastAPI WebSocket NexusOrchestrator
- Async STT + speculative RAG + forensics as concurrent asyncio.TaskGroup
- Sub-200ms latency
- Gemini Live API / Gemini 2.5 Flash Native Audio voice streaming
- Bidirectional PCM + auto-reconnection + exponential backoff
- Gemini Embedding API (3072-dim) + Milvus COSINE/HNSW
- Tri-modal forensics: Wav2Vec2 audio + Gemini LLM text + Gemini Vision
- PostgreSQL 9-table persistence (pipeline_tasks, decision_log, etc.)
- Multi-format doc ingestion: PDF/DOCX/XLSX via PyMuPDF/python-docx/Pandas
- 512-token overlapping chunking into Milvus

**AI Call Screener (Twilio + FastAPI):**
- 8 kHz real-time telephony pipeline
- Silero VAD (256-sample frames, 1.2s min speech / 1.5s silence)
- Gemini 2.0 Flash multilingual ASR + Faster-Whisper int8 fallback
- WavLM deepfake scorer (5-frame smoothing)
- 6-class emotion inference
- JWT cookie auth (pbkdf2_sha256)
- Docker/docker-compose deployment
- Rule-based explainability engine with forensic threat timelines 
  and volatility indices

**AI Audio Cutter + Audio-Text AI Agent:**
- Automated speaker-separation pipeline
- pyannote/speaker-diarization-3.1 with speaker-drift prevention 
  (cosine ≥0.85 merge)
- Quality rules: reject overlaps, filter <1.2s, ZIP export
- Gemini 1.5 Django chatbot over transcribed audio
- Whisper + ECAPA-TDNN diarization
- Multilingual emotion/sentiment analysis
- HITL Celery fine-tuning pipeline + ReportLab reporting

---

### Insightrix Consulting Pvt. Ltd. — Remote
**Role:** Data Scientist | **Period:** May 2025 – Jan 2026

- Built production credit risk scoring system on 200k+ invoices/receipts 
  (9 years data) using XGBoost + LightGBM + Random Forest ensemble
  Result: R²=97.7%, Accuracy=93.1%
- Normalized 1,200-column financial dataset → 50 key features with schema 
  validation; loaded to AWS RDS (MS SQL Server)
- Engineered LLM-assisted carbon accounting pipeline (GPT-4o) extracting 
  25+ structured fields from 40k+ HTML files per run
- Integrated with Wasabi S3 & Linux VPS
- Designed & deployed production RAG chatbot (Algolia + Groq LLaMA3 70B) 
  for Dubai travel product with semantic query parsing & fallback logic
- Engineered music/audio embeddings (MFCCs, tempo, valence, popularity) 
  for unsupervised consumer personality clustering
- Automated LLM pipelines with Cursor AI & Lovable.ai

---

### JUNLP (ANNEX) Lab, Jadavpur University — Kolkata
**Role:** NLP Research Intern – M.Sc. Thesis
**Period:** Aug 2024 – Jul 2025 | **Supervisor:** Dr. Dipankar Das

**ACL 2025 — SemEval-2025 Task 7:**
- Designed cross-lingual multilingual claim retrieval system
- MiniLM sentence embeddings + FAISS ANN vector search
- Ranked 22nd globally (50+ international teams)
- Published: ACL Anthology, Vienna 2025, pp. 2084–2089

**CLEF 2025 — Task 4a (CheckThat!):**
- Architected dual-encoder (SciBERT + Twitter-RoBERTa)
- Scientific social-media multi-label discourse classification
- Macro F1=0.8262
- Ranked 9th globally
- Published: CEUR-WS Working Notes, Madrid 2025, pp. 1038–1043

**DRDO-Funded Research (Under Review):**
- Built 7,000+ Indian-language news corpus via BeautifulSoup + Selenium
- Implemented 3-evidence retrieval/claim using GPT-4o Mini, DeepSeek, Qwen
- Fine-tuned XLM-RoBERTa & MuRIL with human Support/Refute/NEI annotations
- Result: 86.08% accuracy
- Paper under review

## PUBLICATIONS & ACHIEVEMENTS

- **ACL 2025** (SemEval Workshop, Vienna): "JU_NLP at SemEval-2025 Task 7:
  Leveraging Transformer-Based Models for Multilingual & Crosslingual 
  Fact-Checked Claim Retrieval" — ACL Anthology pp. 2084–2089 | Rank: 22nd globally

- **CLEF 2025** (Working Notes, Madrid): "JU_NLP at CheckThat! 2025: 
  Leveraging Hybrid Embeddings for Multi-Label Classification in Scientific 
  Social Media Discourse" — CEUR-WS pp. 1038–1043 | Rank: 9th globally

- **DRDO-Funded (Under Review):** Multilingual Indian-language news claim 
  verification using transformer models with LLM-assisted evidence retrieval
  (XLM-RoBERTa, MuRIL, GPT-4o Mini)

- **NeuroHack Challenge 2026 — Certificate of Excellence:** Organized by 
  IITG.ai × Smallest.ai at IIT Guwahati — Rank 34

## EDUCATION

- M.Sc. in Data Science — University of Kalyani, West Bengal | 2023–2025 | CGPA: 7.75/10
- B.Sc. (Hons.) Computer Science — Memari College, Burdwan University | 2020–2023 | CGPA: 9.1/10