# ⚙️ Setup Guide

Follow these steps to set up and run the Diabetes Prediction project on your local machine.

---

## 📋 Prerequisites

Make sure the following are installed on your system:

- **Python** 3.8 or higher → [Download](https://www.python.org/downloads/)
- **pip** (Python package manager)
- **Git** → [Download](https://git-scm.com/)
- **Jupyter Notebook** (optional, for `.ipynb` files)

---

## 📥 1. Clone the Repository

```bash
git clone https://github.com/your-username/y-DiabetesPrediction.git
cd y-DiabetesPrediction
```

---

## 🐍 2. Create a Virtual Environment (Recommended)

```bash
# Create virtual environment
python -m venv venv

# Activate on Linux/macOS
source venv/bin/activate

# Activate on Windows
venv\Scripts\activate
```

---

## 📦 3. Install Dependencies

```bash
pip install numpy pandas scikit-learn tensorflow keras matplotlib seaborn jupyter
```

> **Tip:** If a `requirements.txt` file is present, install all dependencies at once:
> ```bash
> pip install -r requirements.txt
> ```

---

## 📂 4. Navigate to the Project Folder

```bash
cd "Diabetes Prediction"
```

---

## ▶️ 5. Run the Models

### Option A — Run a Python Script

```bash
# Dense Layer model
python "PIMA using Dense Layer.py"

# MLP model
python "PIMA Diabetes prediction using MLP.py"

# ELM model
python "PIMA Diabetes prediction using ELM.py"
```

### Option B — Open a Jupyter Notebook

```bash
jupyter notebook
```

Then open one of the following notebooks in your browser:
- `Diabetes_Prediction_using_SVM.ipynb`
- `PIMA_With_Multiple_Algorithms.ipynb`
- `PIMA using MLP.ipynb`

---

## 📊 Dataset

The dataset (`diabetes.csv`) is included in the `Diabetes Prediction/` folder. It is the **PIMA Indians Diabetes Dataset** originally available on [Kaggle](https://www.kaggle.com/uciml/pima-indians-diabetes-database).

---

## ❓ Troubleshooting

| Issue | Solution |
|---|---|
| `ModuleNotFoundError` | Run `pip install <module-name>` |
| Jupyter not found | Run `pip install notebook` |
| GPU not detected | Ensure CUDA and cuDNN are configured for TensorFlow |

---

## ✅ Expected Output

After running any model, you should see:
- Training accuracy and loss per epoch
- Final test accuracy
- Confusion matrix or classification report (where applicable)
