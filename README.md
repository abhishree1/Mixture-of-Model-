# **Mixture-of-Agents (MoA) Framework**

A Python implementation of the **Mixture-of-Agents (MoA)** architecture for leveraging multiple large language models (LLMs) collaboratively to enhance natural language generation. This framework integrates state-of-the-art Hugging Face models, such as **Qwen1.5**, **WizardLM**, **Mixtral**, and **dbrx-instruct**, to iteratively synthesize and refine responses across multiple layers.

---

## **Features**
- Multi-layer architecture for collaborative response refinement.
- Integration of open-source Hugging Face LLMs for proposers and aggregators.
- GPU-accelerated inference using PyTorch and Hugging Face's `transformers`.
- Customizable for different benchmarks and evaluation use cases.

---

## **How It Works**
1. **Proposers**: Generate diverse responses using multiple LLMs in the first layer.
2. **Aggregator**: Combine and refine the proposers' outputs iteratively through multiple layers.
3. **Final Output**: The last layer synthesizes the final, high-quality response.

The architecture is inspired by the paper *"Mixture-of-Agents Enhances Large Language Model Capabilities"*.

---

## **Installation**

1. Install the required dependencies:
   ```bash
   pip install transformers torch
   ```

2. Ensure a GPU-enabled environment for optimal performance.

---

## **Project Structure**
```
.
├── moa_framework.py       # Contains the Mixture-of-Agents framework and LLMClient class
├── README.md              # Documentation for the repository
```

---

## **Acknowledgments**
- Inspired by the paper *"Mixture-of-Agents Enhances Large Language Model Capabilities"*.
- Open-source models provided by Hugging Face.
