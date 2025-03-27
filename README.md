# 🧠 DeepSeek Hack Benchmark

Welcome to the official repository for **Compete Hack Hours – AI/ML Edition | DeepSeek**! This project benchmarks Large Language Models (LLMs) deployed in **Azure AI Foundry** and GitHub, focusing on code generation tasks and practical evaluations.

## 🚀 Project Overview

- Compare models such as `DeepSeek-R1`, `o3-mini`, `o1-mini`, `gpt-4o`, and `DeepSeek-V3`, with the option to use either **Azure AI Foundry** or **GitHub-hosted models** depending on your setup.
- Evaluate tasks such as logical reasoning, math, and Python coding.
- Visualize pass rates, latency, and token usage.
- Designed for developers of all skill levels with a user-friendly Jupyter Notebook.
- Run locally, in GitHub Codespaces, or directly using either Azure AI Foundry or GitHub models.

---

## 🧪 Model Groups Compared
This project compares two distinct groups of models, each optimized for different capabilities:

- **Group 1 – Azure AI Foundry Deployed Models**: `DeepSeek-R1`, `o3-mini`, `o1-mini`
  - These models are fine-tuned for **logical reasoning, instruction following**, and general **code generation tasks**.

- **Group 2 – GitHub-Hosted or External Models**: `gpt-4o`, `DeepSeek-V3`
  - These models are more recent and designed for **advanced reasoning**, **multimodal** use cases, and **enhanced generalization**.

---

## 📆 Use in GitHub Codespaces

This repository includes full support for **GitHub Codespaces** using a preconfigured `devcontainer`.

### 🚀 Quick Start in Codespaces
1. Click the green **"Code"** button on this repository.
2. Select **"Codespaces > Create codespace on main"**.
3. Wait for setup (devcontainer will install everything automatically).
4. Explore either of the following notebooks:
   - `azure_foundry_benchmark.ipynb`
   - `github_model_benchmark.ipynb`

You'll be working in a fully pre-configured environment — no local setup needed!

---

## 📆 Setup Instructions

### 🔧 Requirements
- Python 3.9+
- Access to Azure AI Foundry and/or GitHub tokens

### 📁 Environment Setup
Create a `.env` file with the following keys:
```env
AZURE_PROJECT_CONNECTION_STRING=<your-azure-connection-string>
AZURE_INFERENCE_SDK_ENDPOINT=<azure-inference-endpoint>
ENDPOINT_URL=<azure-openai-endpoint>
AZURE_INFERENCE_SDK_KEY=<your-foundry-api-key>
OPENAI_API_KEY=<your-openai-api-key>
GITHUB_TOKEN=<your-github-token>
```

### 📅 Install Dependencies
```bash
pip install -r requirements.txt
```

Or run in Jupyter Notebook:
```python
!pip install openai azure-identity azure-ai-resources azure-ai-projects pandas matplotlib seaborn python-dotenv
```

---

## 💻 How to Use

### 🔬 Benchmark via Notebook
You can run one of the following notebooks depending on the platform you want to use:

- `azure_foundry_benchmark.ipynb` → for models deployed on **Azure AI Foundry**
- `github_model_benchmark.ipynb` → for models accessed via **GitHub** endpoints

Each notebook will:
- Authenticate to the appropriate backend
- Run prompts across selected models
- Auto-evaluate results
- Generate CSV & charts

You can execute these notebooks in **three ways**:
- 🖥️ Locally with Python & Jupyter installed
- ☁️ Inside a **GitHub Codespace** (recommended for simplicity)
- 🌐 Using the **Azure AI Foundry Environment** (within the Azure AI Studio)

Run locally or in Codespaces with:

```bash
jupyter notebook azure_foundry_benchmark.ipynb
# or
jupyter notebook github_model_benchmark.ipynb
```

### 🤖 Tasks Benchmarked
- ✅ Prime number checker
- 🔄 String reversal
- ➗ Math equations
- 🤖 Creative writing
- 💬 Multi-turn dialog

---

## 📊 Visual Outputs
- Response time bar charts
- Token usage comparisons
- Pass/fail accuracy
- Heatmaps for model-task performance

---

## 🤝 Contributing
Pull requests and feedback are welcome! Feel free to fork and expand on:
- More tasks and test cases
- Advanced metrics (e.g., hallucination rate)
- Additional models or endpoints

---

## 📄 License
This project is licensed under the MIT License.

---

## 🎉 Event Credits
Built for **Compete Hack Hours – AI/ML Edition | DeepSeek** by an awesome developer team. Good luck, hackers!
