# 🏎️Formula 1 Structured Question-Answering Using Transformer Models

This project explores the application of transformer-based models, specifically **RoBERTa** and **Flan-T5**, to structured question-answering (QA) tasks in the high-data-complexity domain of Formula 1 racing. The system is designed to interpret and respond to factual and reasoning-based questions generated from structured F1 data.

---

## 📌 Objectives

- To evaluate the capability of state-of-the-art transformer models on synthetic QA tasks derived from structured F1 race data.
- To analyze performance using standard NLP metrics such as ROUGE and chrF.
- To test model adaptability for domain-specific data in a computationally constrained environment.

---

## 🛠️ Methodology

- **Dataset**: A custom, synthetic QA dataset was constructed using structured data from selected Formula 1 races.
- **Preprocessing**: Data was cleaned and converted into a context-question-answer format suitable for both encoder-decoder and encoder-only models.
- **Models Used**:
  - [RoBERTa](https://arxiv.org/abs/1907.11692) for classification and answer ranking.
  - [Flan-T5](https://arxiv.org/abs/2210.11416) for generative QA.
- **Evaluation Metrics**:
  - `ROUGE-N` for n-gram overlap evaluation.
  - `chrF` for character-level precision/recall analysis.

---

## 📊 Results and Evaluation

- **Metrics**: Evaluated using `ROUGE` and `chrF`.
- **Performance**:
  - Both RoBERTa and Flan-T5 showed potential in handling structured QA.
  - Scores were modest, attributed to limited training data and computational power.
- **Viability**:
  - Demonstrated the adaptability of transformer models to complex, structured domains such as Formula 1.
  - Highlighted the potential of fine-tuned LLMs for domain-specific QA systems.

---

## ⚠️ Limitations

- **Data Size**: The training dataset was small and covered only one race, impacting generalization.
- **Resource Constraints**: Full-race contextualization and larger datasets were restricted due to hardware limitations.

---

## 🔮 Future Work

- Expand the QA corpus to span entire F1 seasons.
- Use high-memory GPUs to allow full-context and long-sequence training.
- Experiment with architectures capable of handling longer inputs (e.g., LongT5, BigBird).
- Improve context construction to enable more nuanced and accurate question-answering.

---

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone [https://github.com/Abhi2748/F1-Race-QA-Generation-using-Transformer-Models-.git]
   cd F1-Race-QA-Generation-using-Transformer-Models-
   ```

2. Set up the environment:
   ```bash
   pip install -r requirements.txt
   ```

3. Run training/evaluation scripts:
   ```bash
   python data_extraction.ipynb
   python single_race_data.ipynb
   python roberta_new.ipynb
   python generative.ipynb
   ```

---
## 📬 Contact

For questions, reach out to [abhireddy2748@gmail.com](mailto:abhireddy2748@gmail.com).

