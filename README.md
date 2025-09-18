# Quantum-Enhanced AI Auditing for Ethical Recruitment

This project demonstrates how to **audit recruitment AI models** for **fairness, bias, and robustness** using a mix of **classical machine learning** and **quantum-inspired techniques**. It also generates a **fairness certificate** and provides a **visual dashboard** for transparent reporting.

---

## 📌 Overview
AI models are increasingly used in **recruitment pipelines**, but they risk inheriting **biases from historical data**.  
This framework provides:  
- **Bias detection** via quantum kernels.  
- **Privacy-preserving auditing** (encrypted simulation).  
- **Robustness checks** against adversarial inputs.  
- **Fairness certification** using standard metrics.  
- **Visual dashboards** for stakeholders.  

---

## 🚀 Features
- Train multiple recruitment AI models:  
  - Logistic Regression  
  - Random Forest  
  - Neural Network  

- **Auditing methods:**  
  - Quantum kernel-based subgroup bias detection.  
  - Encrypted auditing (homomorphic-style simulation).  
  - Adversarial robustness testing (FGSM-style).  

- **Fairness metrics & certification:**  
  - Demographic Parity Gap  
  - Selection Rate Disparity (80% rule)  
  - Equal Opportunity Difference  

- **Visualization dashboard:**  
  - Selection rate bar plots  
  - Demographic parity heatmaps  
  - Fairness vs Accuracy scatter plots  
  - Radar charts  
  - Confusion matrices by group  
  - PASS/FAIL audit grid  

---

## 📂 Project Structure
```
quantum_ai_auditing_with_visuals.ipynb   # Main notebook
README.md                               # Project documentation
```

---

## ⚙️ Installation

1. Clone the repo:  
```bash
git clone https://github.com/your-username/quantum-ai-auditing.git
cd quantum-ai-auditing
```

2. Install dependencies (recommend virtual env):  
```bash
pip install -r requirements.txt
```

3. Requirements include:  
- `pennylane` (for quantum kernels)  
- `scikit-learn` (classical ML models)  
- `numpy`, `pandas` (data handling)  
- `matplotlib`, `seaborn` (visualization)  

---

## 📖 Usage

1. Open the notebook:  
```bash
jupyter notebook quantum_ai_auditing_with_visuals.ipynb
```

2. Run through the steps:  
   - Load and preprocess recruitment dataset.  
   - Train ML models.  
   - Perform **quantum-enhanced auditing**.  
   - Simulate encrypted auditing.  
   - Run adversarial robustness checks.  
   - Generate fairness certificate.  
   - View **visual dashboards**.  

---

## 🔬 Quantum Circuit Example

The **quantum kernel** circuit encodes data via **Angle Embedding**:  

```python
@qml.qnode(dev)
def kernel_circuit(x1, x2):
    qml.templates.AngleEmbedding(x1, wires=[0,1])
    qml.adjoint(qml.templates.AngleEmbedding)(x2, wires=[0,1])
    return qml.probs(wires=[0])
```

This computes **similarity in Hilbert space**, revealing subgroup biases not visible to classical audits.  

---

## 📊 Visuals

- **Fairness heatmap:** Detects parity gaps across models.  
- **Radar chart:** Multi-metric fairness comparison.  
- **Fairness vs Accuracy scatter:** Trade-off visualization.  
- **PASS/FAIL grid:** Final certification.  

---

## 🏆 Contributions
- Blends **classical ML auditing** with **quantum-enhanced bias detection**.  
- Introduces **privacy-preserving encrypted audit simulations**.  
- Adds **robustness testing** against adversarial bias exploitation.  
- Produces **transparent fairness reports** for regulators and stakeholders.  

---

## 🔮 Future Work
- Scale to larger datasets with hybrid quantum-classical methods.  
- Extend encrypted auditing with true **homomorphic encryption**.  
- Apply to other domains: **finance, healthcare, legal AI**.  

---

## 📜 License
MIT License. Free to use and modify.  
