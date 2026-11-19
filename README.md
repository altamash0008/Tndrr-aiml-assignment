# Tndrr-aiml-assignment

# Task 1 – LoRA Fine-Tuning

## Objective
Fine-tune Qwen2.5-0.5B-Instruct using LoRA for structured extraction of customer support requests into JSON.

## Tools
Python, PyTorch, Hugging Face Transformers, PEFT, Google Colab.

## Results
- Base model accuracy: 70%
- Fine-tuned model accuracy: 100%
- Trainable parameters: 0.1093%
- Test samples: 50

## Files
- `01_LoRA_fine_Tuning.ipynb` – Complete implementation and evaluation.

## Execution
Open the notebook in Google Colab, select a GPU runtime, and run all cells.

# Task 2 – Retrieval-Augmented Generation (RAG)

## Objective
Build a RAG system to retrieve relevant information from the NIST AI Risk Management Framework and generate answers.

## Tools
Python, PyMuPDF, Sentence Transformers, Hugging Face Transformers, Google Colab.

## Results
- Embedding model: all-MiniLM-L6-v2
- Generation model: flan-t5-base
- Best Recall@5: 0.881 (600-word chunks)
- Hit@5: 93.3%
- Answer accuracy: 13.33% (strict)

## Knowledge Source
[NIST AI Risk Management Framework 1.0](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)

## Files
- `02_RAG_From_Scratch.ipynb` – Complete RAG implementation and evaluation.

## Execution
Open the notebook in Google Colab and run all cells sequentially.

# Task 3 – Model Optimization using llama.cpp

## Objective
Compare Q4_K_M and Q8_0 quantized versions of Qwen2.5-0.5B-Instruct for efficient local inference.

## Tools
Python, llama.cpp, GGUF, CUDA, Google Colab, NVIDIA Tesla T4.

## Results

| Metric | Q4_K_M | Q8_0 |
|---|---:|---:|
| Model size | 468.64 MB | 644.41 MB |
| Speed | 217.29 tokens/sec | 205.54 tokens/sec |
| GPU memory | 557 MiB | 685 MiB |

Q4_K_M provided better measured speed and memory efficiency.

## Files
- `03_Model_Optimization.ipynb` – Model loading, benchmarking, and evaluation.

## Execution
Open the notebook in Google Colab with a GPU runtime and run all cells.
