# <font color="#003366">Workshop: Introduction to Local LLMs with Ollama</font>

Welcome to the **Local LLM Workshop**! This repository is designed to teach you the fundamentals of running Large Language Models (LLMs) directly on your laptop—**no internet connection required** after the initial setup.

This guide covers everything from basic text generation to advanced vision-language tasks and custom model creation.

---

## <font color="#003366">1. Project Overview</font>

Running LLMs locally ensures **data privacy**, eliminates **API costs**, and allows for **offline development**. This workshop focuses on using the **Ollama** framework to manage and interact with these models efficiently.

### <font color="#008080">What's Inside:</font>
* **`Introduction_to_Ollama.ipynb`**: The main hands-on notebook.
* **`Modelfile`**: A blueprint to create your own customized AI persona.
* **`Images/`**: Sample images for testing multimodal (Vision) capabilities.
* **`requirements.txt`**: List of Python dependencies.

---

## <font color="#003366">2. Setup Instructions</font>

### <font color="#008080">Prerequisites</font>
1.  **Install Ollama**: Download and install from [ollama.com](https://ollama.com).
2.  **Python**: Ensure you have Python 3.8+ installed.

### <font color="#008080">Installation</font>
Clone this repository and install the necessary Python library:

```bash
pip install -r requirements.txt
```

## <font color="#003366">3. Custom Model Creation</font>
One of the most powerful features of Ollama is the ability to create **custom models** using a `Modelfile`. This allows you to "bake" specific instructions, parameters, and system prompts into a reusable model identity.

### <font color="#008080">How to build your model:</font>
Open your terminal in this project folder and run the following command:

```bash
ollama create my-custom-model -f Modelfile
```

### <font color="#003366">4. Workshop Modules</font>
The included notebook is divided into the following technical sections:

Library Integration: Connecting Python to the Ollama server.

Response Generation: Simple and Streaming outputs.

Vision Tasks: Analyzing single and multiple images locally.

Hyperparameter Tuning: Mastering temperature, num_ctx, and repeat_penalty.

Model Management: Pulling, listing, and inspecting local models.

### <font color="#003366">5. Vision Capabilities</font>
To test the Vision modules, ensure you have a multimodal model pulled:

```bash
ollama pull llava
```
The notebook will reference files inside the /Images folder to demonstrate how LLMs can "see" and describe visual data without cloud processing.

### <font color="#003366">6. Resource Usage Tips</font>
RAM/VRAM: Ensure your laptop has at least 8GB of RAM for 7B models (like Llama 3 or Mistral).

GPU Acceleration: Ollama automatically detects NVIDIA or Apple Silicon GPUs for faster inference.

Battery: Running LLMs is CPU/GPU intensive; keep your laptop plugged in for best performance!

### <font color="#003366">Share your feedback If you have attended the Workshop</font>
https://forms.gle/PL4HpEX9ZgArKoxo8
