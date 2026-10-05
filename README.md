<h1 align="center">Yash Bajpai</h1>

<p align="center">
  <strong>AI Engineer</strong> · building autonomous agents, custom LLMs & edge AI systems
</p>

<p align="center">
  <a href="https://linkedin.com/in/yash-bajpai-b5a86332a/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white"/>
  </a>
  &nbsp;
  <a href="mailto:bajpaiyash2707@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=flat&logo=gmail&logoColor=white"/>
  </a>
  &nbsp;
  <a href="https://huggingface.co/Yash1bajpai">
    <img src="https://img.shields.io/badge/%F0%9F%A4%97_Hugging_Face-Models-black?style=flat"/>
  </a>
  &nbsp;
  <a href="https://pypi.org/project/nexus-agent-ai/">
    <img src="https://img.shields.io/badge/PyPI-nexus--agent--ai-3776AB?style=flat&logo=pypi&logoColor=white"/>
  </a>
</p>

---

## What I Do

I build AI systems end-to-end — from training custom models to shipping autonomous agents and production ML products.

- 🤖 **Agentic AI** — ReAct loops, tool calling, multi-provider LLM systems with automatic fallback
- 🧠 **Custom LLMs** — trained a 246M-parameter coding foundation model from scratch (pretraining, FIM, quantization)
- 📱 **Edge AI** — on-device LLM inference on Android via llama.cpp; I benchmark what actually fits in a phone's RAM
- 🔧 **Production ML** — FastAPI backends, vector databases, automated cloud retraining, full-stack dashboards

---

## Featured Work

<table>
<tr>
<td width="50%" valign="top">

**[⚡ nexus-agent](https://github.com/Yash1bajpai/nexus-agent)**
Autonomous ReAct coding agent, published on PyPI

- Multi-provider backend: Claude · Gemini · OpenAI + auto-fallback on rate limits
- 8 sandboxed tools: file I/O, code execution, web search, git
- Real-time token/cost tracking · runs on Android (Termux)
- 111 tests · CI matrix on Python 3.11 / 3.12 / 3.13

`Python` `ReAct` `Typer` `Multi-provider LLM`

</td>
<td width="50%" valign="top">

**[🧠 CodeForge-250M](https://github.com/Yash1bajpai/CodeForge-250M)**
Custom 246M-parameter coding foundation model **(in progress)** — [interim checkpoint on Hugging Face](https://huggingface.co/Yash1bajpai/CodeForge-250M)

- Built from scratch: 16 layers, 1024 hidden, custom 32k FIM tokenizer
- PyTorch SDPA (FlashAttention-2): >50% activation-memory cut (15 GB → 5.05 GB on a T4)
- Live run at 7.24 training perplexity (step 2100 / 2898 of a 1.52B-token pass)
- 50% FIM infill rate (StarCoder/DeepSeek standard) + MinHash deduplication
- Grammar-constrained decoding for guaranteed-valid JSON tool calls

`PyTorch` `SDPA` `FIM` `MinHash` `GPU Training`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[📈 Inditrade AI](https://github.com/Yash1bajpai/Inditrade_AI)** — [Live Site](https://inditrade.vercel.app/)
Global trade intelligence engine for India

- XGBoost forecasting (log-scale R² 0.958, dollar RMSE $0.90B) + Isolation Forest anomalies
- Node2Vec trade-network embeddings
- **"Vanijya AI"** — RAG chatbot over trade documents (Qdrant + chat history)
- Next.js + FastAPI + Supabase · monthly auto-retraining via GitHub Actions

`XGBoost` `FastAPI` `Next.js` `Qdrant` `RAG`

</td>
<td width="50%" valign="top">

**[📊 Global MacroForecast](https://github.com/Yash1bajpai/Global-MacroForecast)** — [Live Site](https://global-macro-forecast.vercel.app/)
GDP nowcasting engine — US · India · Japan · Germany

- LightGBM + SARIMA ensemble, inverse-RMSE weighted
- Optuna-tuned, chronological hold-out (zero data leakage)
- Deployed on Vercel + Render with static-snapshot fallback

`LightGBM` `SARIMA` `Optuna` `FastAPI`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[🛡️ Vision](https://github.com/Yash1bajpai/vision_app)**
Fail-closed execution boundary for on-device AI agents

- Strict 4-key JSON action schema + bounded &le;3-action plans — no provider output reaches execution unvalidated
- Risk-tiered confirmation · zero disk persistence (no state poisoning, no injection side-effects)
- 91/91 JVM tests + 5/5 on-device instrumentation tests · signed APK verified on physical hardware
- LLM runtime deliberately deferred — the boundary exists so a model cannot bypass it

`Java` `Android` `Fail-closed` `Prompt-injection Defense`

</td>
<td width="50%" valign="top">

**[📱 Edge LLM Benchmarks](https://github.com/Yash1bajpai/edge-llm-benchmarks)**
Quantization limits of real Android hardware

- 4 sub-4B models, Q4_K_M vs Q8_0, on a 6 GB Snapdragon 695 phone vs PC
- Found the ~3.0–3.5 GB usable-RAM wall: Q4_K_M runs to 3.8B, Q8_0 OOMs above 2B
- Qwen2.5-3B Q4_K_M: 17.5 tok/s prompt, 5.35 tok/s generation at 1.90 GiB

`llama.cpp` `GGUF` `ARM NEON` `Quantization`

</td>
</tr>
<tr>
<td colspan="2" valign="top">

**Also:** [🧮 ML Algorithms](https://github.com/Yash1bajpai/ml-algorithms) — from-scratch implementations matched against sklearn · [🛍️ Olist E-commerce EDA](https://github.com/Yash1bajpai/olist-ecommerce-eda) · [🔌 MCP Doc CLI](https://github.com/Yash1bajpai/mcp-doc-cli)

</td>
</tr>
</table>

---

## Tech Stack

**AI / ML** &nbsp;
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-2980B9?style=flat)
![XGBoost](https://img.shields.io/badge/XGBoost-6a9fb5?style=flat)
![llama.cpp](https://img.shields.io/badge/llama.cpp-555555?style=flat)
![Qdrant](https://img.shields.io/badge/Qdrant-DC382D?style=flat)

**LLM APIs** &nbsp;
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic-191919?style=flat&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white)

**Backend** &nbsp;
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-black?style=flat&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)

**Core** &nbsp;
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

---

<p align="center">
  <i>Looking for AI engineering roles — remote-friendly · bajpaiyash2707@gmail.com</i>
</p>
