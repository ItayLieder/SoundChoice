# SoundChoice
Interactive A/B mastering platform – upload a track, compare two variants, and let the system learn your taste through simple A/B choices. Personalized, safe, and non-technical audio mastering.

# 🎚️ AB Master

**Interactive A/B mastering platform**  
Upload a track, compare two variants, and let the system learn your taste through simple A/B choices.  
Personalized, safe, and non-technical audio finishing for musicians and creators.

---

## 🚀 What is this?

AB Master is an experimental online service for mixing and mastering that flips the workflow:  
instead of sliders, knobs, or technical jargon, users make **simple binary choices**:

- Listen to **A** and **B**  
- Pick the one you prefer  
- Repeat a few times  

The system adapts to your preferences in real time and produces a **final master** that matches your taste — always within professional guardrails (loudness, true peak, stereo safety).

This makes mastering accessible to anyone, from indie musicians to podcasters, without needing to know EQ curves or compression ratios.

---

## ✨ Features (MVP)

- **Upload** stereo track (stems optional later).  
- **Auto-detect preview loop** (10–20s).  
- **A/B comparison flow** with loudness-matched, instant switching.  
- **Preference learning** (pairwise model) to converge on your sound.  
- **Final master export** (LUFS- and peak-safe, streaming-ready).  
- **Taste profiles** saved per user for quick reuse.  

---

## 🛠️ Tech Stack

- **Backend:** Python + FastAPI  
- **Learning:** Pairwise preference (BTL logistic regression)  
- **Audio DSP:** `ffmpeg`, `pydub`, `librosa`, `pyloudnorm`  
- **Workers:** Celery + Redis  
- **Database:** SQLite (MVP), Postgres later  
- **Frontend:** React + Vite (TypeScript)  

---

## 📂 Repo Layout (planned)

