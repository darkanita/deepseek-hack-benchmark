# 🧠 DeepSeek Hack Benchmark

Welcome to the official repository for **Compete Hack Hours – AI/ML Edition | DeepSeek**! This project benchmarks Large Language Models (LLMs) deployed in **Azure AI Foundry** and GitHub, focusing on code generation tasks and practical evaluations.

## 🚀 Project Overview

- Compare models like `DeepSeek-R1`, `o3-mini`, and `o1-mini`.
- Evaluate tasks such as logical reasoning, math, and Python coding.
- Use Azure AI Foundry and GitHub-hosted endpoints.
- Visualize pass rates, latency, and token usage.
- Designed for developers of all skill levels with a user-friendly Jupyter Notebook.

---

## 📆 Use in GitHub Codespaces

1. Click the green **"Code"** button and select **"Codespaces > Create codespace on main"**.
2. Wait for setup to complete.
3. Open `azure_model_benchmark.ipynb` and start exploring!

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
Run the included Jupyter Notebook to:
- Authenticate to Azure
- Run prompts across models
- Auto-evaluate results
- Generate CSV & charts

```bash
jupyter notebook azure_model_benchmark.ipynb
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
