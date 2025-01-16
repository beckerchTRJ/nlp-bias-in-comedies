# Implicit Bias in Comedic Scripts

### Overview
This project explores the presence of implicit bias in comedic scripts using advanced machine learning models. By analyzing comedy scripts from the early 2000s, the goal is to uncover how humor can reflect or perpetuate societal biases, providing insights into the nuances of comedic language and its implications.

---

## Repository Structure

```plaintext
root/
├── data/                 # Directory for datasets and preprocessed data
├── notebooks/            # Jupyter notebooks for exploration and analysis
├── results/              # Outputs, metrics, and visualizations
├── paper.pdf             # Full write-up of the project
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
├── .gitignore            # Files to exclude from version control
```

---

## Data Handling

Data files are not included in this repository but can be accessed as follows:
- **Datasets Used**:
  - [CrowS-Pairs](https://huggingface.co/datasets/crows_pairs): Annotated sentences for bias detection.
  - [Stereoset](https://huggingface.co/datasets/McGill-NLP/stereoset): Dataset focusing on gender, profession, race, and religion bias.
  - [NewsMediaBias](https://huggingface.co/datasets/newsmediabias/news-bias-full-data/blob/main/train.csv): Tweets labeled for neutrality.
- **Scripts for Data Access**:
  - Scripts are all sourced from publically available texts. You can find them in the data folder.

---

## Installation

1. Clone this repository:
   ```bash
   git clone [repository-url]
   cd [repository-folder]
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Methods

1. **Datasets**:
   - Combined multiple datasets with annotated biases.
   - Used comedy scripts from the early 2000s for evaluation.
2. **Models**:
   - Support Vector Machine (SVM)
   - Perceptron
   - Bidirectional Long Short-Term Memory (BiLSTM)
   - Bidirectional Encoder Representations from Transformers (BERT)
3. **Processing**:
   - Preprocessed datasets with tokenization, cleaning, and embedding transformations.
   - Evaluated model performance using precision, recall, F1-score, and accuracy.

---

## Usage

### Running Notebooks
1. Launch the Jupyter Notebook environment:
   ```bash
   jupyter notebook
   ```
2. Navigate to `notebooks/` and select the desired notebook.

---

## Results
- **Model Metrics**:
  - BERT achieved the highest accuracy (95.01%) and F1-score (94.78%).
  - Outputs include detected biases in comedic scripts, emphasizing gender and race.
- **Future Work**:
  - Annotating comedic scripts with verified bias labels.
  - Integrating humor detection to improve model sensitivity to comedic nuances.

---

## Contributing
Contributions are welcome! You can help by:
- Reporting issues
- Suggesting features
- Submitting pull requests

---


## Acknowledgements
- Thanks to the creators of CrowS-Pairs, Stereoset, and NewsMediaBias datasets.
- Thanks to team members Pia Rodriquez, Frederick Zhang, Rudra Singh, and Ethan Feng
- Inspired by methodologies from Nadeem and Raz (2022) and fine-tuning strategies outlined by Sun et al. (2019).

