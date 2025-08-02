# Enhancing Explainability in Multimodal Decision Support Systems  
**A Framework for Transparent AI Integration in Healthcare**

**Author:** Èric Sánchez López  
**Program:** Advanced Master’s degree in Artificial Intelligence, KU Leuven  

---

## Repository Structure

```
.
├── 01_analysis_and_modeling.ipynb   # Data ingestion, EDA, model training/optimization & evaluation
├── 02_dashboard.ipynb               # Dash-based dashboard for visualizing and interpreting results
├── 03_lm_sft_pipeline.ipynb         # Supervised fine-tuning pipeline for a language model
├── requirements.txt                 # Python dependencies
└── assets/                          # Supplementary files (e.g., images, configs)
```

> **Note:** Notebooks are prefixed to indicate execution order.

---

## Installation & Setup

1. **Clone the repository**  
   ```bash
   git clone https://github.com/EricSanLopez/AD-XAI-Thesis.git
   cd AD-XAI-Thesis
   ```

2. **Create and activate a virtual environment**  
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Prepare the data**  
   - Place your clinical multimodal dataset under `data/` (create this directory if it doesn't exist).  
   - Update file paths in notebooks if necessary.

---

## Notebooks Overview

### 01_analysis_and_modeling.ipynb
- **Purpose:**  
  - Exploratory Data Analysis (EDA)  
  - Data preprocessing  
  - Model definition  
  - Hyperparameter tuning & evaluation  
  - Explainability methods (SHAP, importance maps)

### 02_dashboard.ipynb
- **Purpose:**  
  - Dash application for interactive result visualisation  
  - User-friendly interface for clinicians to explore predictions and explanations

### 03_lm_sft_pipeline.ipynb
- **Purpose:**  
  - Supervised fine-tuning pipeline for a pretrained language model  
  - Dataset creation from Gemini, training loop, validation, and checkpointing

---

## Usage

- **Run analysis & modeling**  
  1. Launch Jupyter: `jupyter notebook`  
  2. Execute `01_analysis_and_modeling.ipynb` end-to-end.

- **Start the dashboard**  
  ```bash
  jupyter nbconvert --to script 02_dashboard.ipynb
  python 02_dashboard.py
  ```  
  Visit `http://127.0.0.1:8000/` in your browser.

- **Fine-tune the language model**  
  Execute `03_lm_sft_pipeline.ipynb` in Jupyter or convert to a script similarly.

---

## Requirements

- Python ≥ 3.8  
- Jupyter Notebook / JupyterLab  
- Dash  
- scikit-learn, pandas, numpy  
- SHAP  
- Hugging Face Transformers

Refer to `requirements.txt` for the full dependency list.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

**Èric Sánchez López**  
- Email: ericsanlopez@gmail.com  

- LinkedIn: https://www.linkedin.com/in/eric-sanchez-lopez
