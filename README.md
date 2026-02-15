# RAZORWIRE-LIVE
LIVE Binary Analysis with Radare2 + Forensic Classifier + AI (Qwen 0.5B)

<h1 align="center">🧬 RAZORWIRE-LIVE 🧬</h1>

<p align="center">
<em>Live Binary Analysis • Behavioral Signal Scoring • AI-Assisted Forensics</em>
</p>

<p align="center">
<img src="https://img.shields.io/badge/Platform-Google%20Colab-black?style=flat-square&logo=googlecolab&logoColor=orange">
<img src="https://img.shields.io/badge/Engine-radare2-black?style=flat-square&logo=gnu&logoColor=cyan">
<img src="https://img.shields.io/badge/LLM-Qwen%202.5%200.5B-black?style=flat-square">
<img src="https://img.shields.io/badge/UI-Gradio-black?style=flat-square&logo=gradio&logoColor=ff4b4b">
<img src="https://img.shields.io/badge/Forensics-Behavioral%20Scoring-black?style=flat-square&logo=hackaday&logoColor=red">
<img src="https://img.shields.io/badge/License-Research%20Use-black?style=flat-square">
</p>

---

# 🚀 What Is RAZORWIRE-LIVE?

**RAZORWIRE-LIVE** is a real-time binary analysis environment built for Google Colab that combines:

- ⚙️ `radare2` static analysis
- 🧠 AI-assisted forensic reasoning (Qwen 0.5B local model)
- 📊 Behavioral signal scoring engine
- 🧾 Evidence-preserving forensic buffer
- 🎯 Intent classification & threat correlation

It transforms raw disassembly into structured, explainable forensic intelligence.

No cloud API keys.  
No external LLM calls.  
Fully local inference inside Colab.

---

# 🧠 Core Concept

Instead of dumping raw strings and functions, this notebook:

1. Extracts static artifacts (imports, functions, strings, sections)
2. Tags behavioral signals (crypto, injection, ransomware, banking, cracking, tamper)
3. Correlates patterns across categories
4. Builds a structured forensic buffer
5. Feeds structured evidence into a local AI model
6. Returns concise analyst-style answers grounded in evidence

It’s signal > noise binary analysis.

---

# 🛠 Feature Set

## 🔍 Live radare2 Execution
- `aaaa`, `afl`, `ii`, `iS`, `iz`, `iE`
- Entry point detection
- DLL export handling
- Function disassembly by symbol or address
- Byte search & reference tracing

---

## 📊 Behavioral Signal Engine

Weighted detection categories:

- 🌐 Network communication
- 🔐 Cryptography
- 🔑 Key material detection
- 📁 File operations
- ⚙️ Process injection
- 📝 Registry persistence
- 🛡 Anti-debug / anti-tamper
- ☣️ Ransomware correlation
- 💰 Banking indicators
- 🔓 Cracking / keygen patterns
- 🔒 License validation logic

Each category contributes to a total risk score.

---

## 🎯 Risk Classification

Produces:

- 🟢 LOW
- 🟡 MEDIUM
- 🔴 HIGH
- 🔴 CRITICAL

Based on weighted behavioral scoring + correlated behaviors.

---

## 🧾 Forensic Buffer

Every command executed is appended into an evidence log:
This buffer becomes the AI’s contextual dataset.

No hallucinated analysis.  
AI only reasons over captured forensic evidence.

---

## 🤖 Local LLM (Qwen 2.5 0.5B)

- CPU optimized
- No API tokens required
- Truncated context protection
- Deterministic low-temperature inference
- Evidence-referenced answers

- # 📂 Supported File Types

- .exe
- .dll
- .sys
- .drv
- .bin
- .elf
- .so
- .apk
- .dex
- .jar
- .wasm
- and more

Automatic file-type detection modifies radare2 flags accordingly.

---

# 🔬 Example Use Cases

- Malware triage
- Suspicious loader analysis
- Packed binary inspection
- Ransomware indicator detection
- DRM / cracking logic review
- Credential harvesting detection
- Behavioral clustering experiments

---

# ⚠️ Research Notice

This project is intended for:

- Security research
- Malware analysis education
- Defensive reverse engineering
- Academic study

Do not use on systems you do not own or have permission to analyze.

<p align="center">
  <a href="https://colab.research.google.com/github/400lbhacker/RAZORWIRE-LIVE/blob/main/RAZORWIRE_LIVE.ipynb" target="_blank">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
  </a>
</p>

