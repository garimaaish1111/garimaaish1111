<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./header-dark.svg">
  <img alt="Garima Aishwarya: Computer Science at UPES, minor in Aerospace" src="./header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://www.linkedin.com/in/garimaaish1111">LinkedIn</a> ·
  <a href="mailto:garimaaish1111@gmail.com">Email</a>
</p>

## 📓 Research log

### 01 · QuantProbe &nbsp;[`→ repo`](https://github.com/garimaaish1111/quantprobe-research)

> **Question.** Can a hallucination detector still read an LLM's hidden states after the model is quantized?
>
> **Approach.** Linear truthfulness probes on Llama-3.2-1B and Qwen2.5-1.5B at FP16, INT8 and INT4. 6,049 true/false statements, topic-held-out splits, byte-identical inputs across precisions.
>
> **Result.** Probe accuracy doesn't change under quantization (p = 0.38), and moving a probe across precisions costs under 0.02 AUROC.

`Python` `PyTorch` `Transformers` `bitsandbytes` `scikit-learn`

### 02 · LEXAI &nbsp;[`→ repo`](https://github.com/garimaaish1111/LEXAI)

> **Question.** Can a model classify leukemia subtypes from a blood smear and show *why*?
>
> **Approach.** A CNN ensemble for the whole image plus a GNN over segmented cells, fused with cross-modal attention. Grad-CAM and GNN attention show where it looked; MC dropout gives confidence intervals.
>
> **My part.** The data pipeline: four public datasets, class imbalance, train/val/test manifests, and preprocessing (stain normalisation, cell segmentation) that feeds both pathways. I also presented the idea.

`PyTorch` `PyTorch Geometric` `OpenCV` `FastAPI` · Team project at UPES with Brajraj Singh Pathania, Piyush Bharadwaj and Ayushmaan Singh, guided by Prof. Gouranga Duari

### 03 · Email Job Scheduler &nbsp;[`→ repo`](https://github.com/garimaaish1111/email-job-scheduler)

> **Question.** How do you send thousands of scheduled emails exactly once, when the server can die mid-campaign?
>
> **Approach.** Keep the schedule in Redis and Postgres, not in a process. BullMQ delayed jobs, per-sender hourly limits enforced by an atomic Lua script, and jobs over the limit move to the next hour instead of failing.
>
> **Result.** 1,000 emails scheduled in 1.8 s, spaced exactly 2.0 s apart, and nothing lost or duplicated across restarts.

`TypeScript` `Express` `PostgreSQL` `Redis` `BullMQ` `Elasticsearch` `Next.js`

### 04 · PromptMaker &nbsp;[`→ repo`](https://github.com/garimaaish1111/promptmaker)

> **Question.** How cheaply can you turn a rough instruction into a good prompt, and what will that prompt cost to run?
>
> **Approach.** Two stages on different models: a small model finds the gaps in the draft, a frontier model writes the fix. Response caching, prompt caching, and a free cost estimate before anything is spent.

`TypeScript` `Next.js` `Claude API`

### 05 · Crypto Market Analysis &nbsp;[`→ repo`](https://github.com/garimaaish1111/crypto-market-analysis) · [`→ live`](https://cryptomarketanalysis.streamlit.app)

> **Question.** How risky are crypto markets, which phase of the cycle are they in, and do they move with traditional assets?
>
> **Approach.** Volatility and VaR, GARCH, market-cycle phases, rolling correlation against equities, gold, the dollar and oil, and walk-forward ARIMA checked against a random-walk baseline.

`Python` `pandas` `statsmodels` `Plotly` `Streamlit`

### 06 · Resume Matcher &nbsp;[`→ repo`](https://github.com/garimaaish1111/resume-matcher)

> **Question.** Can a resume be scored against a job description the way a careful reader would?
>
> **Approach.** Text extraction, then Sentence-BERT similarity plus skill overlap, ranked into a match score.

`Python` `Sentence-BERT` `Streamlit`

<br/>

## 🧰 Toolbox

| | |
|---|---|
| **Research & ML** | Python · PyTorch · Transformers · scikit-learn · pandas · NumPy · statsmodels · OpenCV |
| **Backend** | TypeScript · Node.js · Express · FastAPI · PostgreSQL · Prisma · Redis · BullMQ · Elasticsearch |
| **Apps** | Next.js · Streamlit · Plotly |
| **Also** | Java · C · SQL · Docker · Git · Colab |
