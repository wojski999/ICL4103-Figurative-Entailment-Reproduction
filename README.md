🧠 Figurative Entailment Reproduction

Reproducing Results of Figurative Language Detection in Textual Entailment
by Jamal Mohammad (ID: 24001883)
Course: ICL4103 – Introduction to Computational Linguistics
Institution: Shahzain’s Beta Bhellar | November 2025

📘 Overview

This project reproduces Chakrabarty et al. (2021), Figurative Language in Recognizing Textual Entailment (ACL-IJCNLP 2021).
It evaluates how RoBERTa handles figurative forms such as metaphor, simile, sarcasm, and irony within the Figurative-NLI benchmark.
The pipeline includes dataset integration, cleaning, model fine-tuning, evaluation, and result visualization.

🎯 Objectives

Reproduce and validate the original Figurative-NLI results.

Compare RoBERTa performance on literal vs. figurative entailment.

Analyze error cases and reproducibility variance.

Document the full benchmark workflow (dataset → model → report → results).

⚙️ Method Summary

Model: RoBERTa-base (Liu et al., 2019)

Learning Rate: 2e-5 | Epochs: 2 | Batch: 4 | Max Len: 128

Dataset: Metaphor, Simile, Sarcasm, Irony subsets (≈ 31 K pairs)

Metrics: Accuracy, Precision, Recall, F1 | Confusion Matrix + Charts

Environment: Google Colab CPU (~28 min runtime)

📊 Results
Metric	Paper	Reproduced
Accuracy	78–80 %	82–84 %
F1 Score	0.77	0.76–0.78
Seed Variance	±1.1 %	Controlled

✅ Results confirm reproducibility within acceptable variance.

💬 Error Highlights

Sarcasm: Missed polarity reversal (“I love getting stuck in traffic.”)

Metaphor: Misread figurative mapping (“Plan crashed and burned.”)

Idiom: Literal interpretation (“Spilled the beans.”)

📁 Contents

Final_Reproduction_Code.ipynb | Cleaned_master_dataset.csv | ICL_Assignment2_Report.docx | Presentation.pptx | README.md

🚀 Future Work

Extend to RoBERTa-large / DeBERTa-v3, integrate conceptual mappings, multilingual figurative datasets, and explanation-based interpretability tools.

🧾 Reference Benchmark

Chakrabarty et al. (2021); Poliak et al. (2018); Liu et al. (2019); Muresan et al. (2022); Stowe et al. (2021)
