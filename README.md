![image](https://github.com/user-attachments/assets/fe71ebd2-0d26-40ab-9249-c48580fdcf77)

# Evaluating Language Models with `lighteval`

This repository provides tools and guidance for evaluating and comparing language models (LLMs) across a wide range of tasks and benchmarks. Evaluation is essential for understanding model performance, identifying strengths and weaknesses, and ensuring alignment with specific use cases. Using `lighteval`, this repository demonstrates how to perform standard benchmark evaluations as well as create custom evaluation pipelines tailored to domain-specific requirements.

---

## Repository Contents

### Automatic Benchmarks
This section focuses on evaluating LLMs using standardized benchmarks like MMLU, TruthfulQA, and BBH. These benchmarks assess model capabilities such as:
- General knowledge and reasoning.
- Logical thinking and problem-solving.
- Language understanding and common sense.

---

## Notebooks

The repository includes interactive notebooks for hands-on exploration of `lighteval`:

### Evaluating and Analyzing LLMs
- **Description**: Demonstrates how to use `lighteval` to evaluate and compare LLMs on various benchmarks and tasks.
- **What's Inside**:
  - Evaluation of two models (`Qwen2.5-0.5B` and `SmolLM2-360M-Instruct`) on medical domain tasks.
  - Setup and configuration of evaluation pipelines.
  - Visualization and analysis of results.
- **Notebook**: [Evaluate and Analyze Your LLM](./notebooks/lighteval_evaluate_and_analyse_your_LLM.ipynb)

---

## Why Use `lighteval`?

`lighteval` simplifies the evaluation process by providing:
- **Task Flexibility**: Define evaluation tasks using a structured format that supports benchmarks like MMLU and custom tasks.
- **Python Integration**: Seamlessly integrate evaluation into Python workflows for automated and programmatic analysis.
- **Efficient Processing**: Evaluate models with minimal setup, making it ideal for quick experimentation and benchmarking.

---

## Getting Started

1. **Run Automatic Benchmarks**:
   Start by evaluating your model on standard benchmarks to establish a baseline.
   ```python
   "leaderboard|mmlu:anatomy|5|0,leaderboard|mmlu:professional_medicine|5|0"
   ```

2.  **Create Custom Domain Evaluations**: Define tasks and datasets specific to your application. For example:
    
    ```python
    [
        "mmlu|anatomy|0|0",
        "mmlu|high_school_biology|0|0",
        "mmlu|high_school_chemistry|0|0",
        "mmlu|professional_medicine|0|0"
    ]
    
    ```
    
3.  **Visualize Results**: Analyze model performance with side-by-side comparisons, detailed metrics, and flexible visualization options.
