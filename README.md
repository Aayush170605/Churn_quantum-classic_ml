# 💳 Quantum-Inspired Credit Card Churn Prediction

A comparative study of **Classical Machine Learning models** and a **Variational Quantum Classifier (VQC)** for predicting customer churn in credit card services.

This project evaluates whether quantum-inspired models can outperform traditional ML techniques on structured tabular data.

---

## 📌 Project Overview

Customer churn prediction is a critical problem in the banking and fintech industry. Accurately identifying customers likely to leave allows companies to:

- Improve retention strategies  
- Reduce revenue loss  
- Optimize marketing efforts  

This project explores:

- Classical ML models with dimensionality reduction (PCA)
- Classical ML models without PCA
- A Variational Quantum Classifier (VQC)

We compare performance across all approaches to evaluate practical viability.

---

## ⚙️ Methodology

### 1️⃣ Data Preprocessing
- Data cleaning and handling missing values  
- Feature scaling  
- Train-test split  
- PCA (for classical pipeline comparison)

---

### 2️⃣ Models Implemented

#### 🔵 Classical Models (With PCA)
- Logistic Regression  
- SVM (RBF Kernel)  
- Random Forest  

#### 🟢 Classical Model (Without PCA)
- Random Forest (No PCA)

#### 🔴 Quantum Model
- Variational Quantum Classifier (VQC)

---

## 📊 Results

### Phase 5 — Model Accuracy Comparison

| Model | Accuracy |
|-------|----------|
| Logistic Regression | **71.97%** |
| SVM (RBF Kernel) | **72.68%** |
| Random Forest (PCA) | **73.81%** |
| Random Forest (No PCA) | **74.73%** |
| VQC | **53.73%** |

---

## 📈 Observations

- Random Forest (No PCA) achieved the **highest accuracy (74.73%)**.
- PCA did not significantly improve performance for tree-based models.
- The Variational Quantum Classifier underperformed compared to classical models.

### About the VQC Performance

While the VQC model achieved lower accuracy (~53%), this result is not entirely unexpected:

- Current quantum hardware and simulators are still limited.
- Feature encoding into quantum circuits remains challenging.
- As the number of qubits (features) increases, the quantum state space grows exponentially (≈ 2ⁿ), which significantly increases simulation complexity and training time on classical hardware.
- Classical models are highly optimized for structured tabular datasets.
- Quantum advantage is typically more promising in high-dimensional or complex optimization problems under ideal hardware conditions.

This experiment demonstrates that **classical ML remains more practical and reliable for structured churn prediction tasks at the current stage of quantum computing development.**

---

## 🧠 Key Learnings

- Tree-based models perform strongly on structured financial datasets.
- PCA is not always beneficial for ensemble models.
- Quantum ML requires careful feature encoding and circuit design.
- Increasing qubits introduces exponential scaling challenges in simulation.
- Hybrid classical-quantum approaches may be more promising than standalone VQC.

---

## 🔮 Future Improvements

- Hyperparameter tuning for VQC  
- Experiment with different quantum feature maps  
- Hybrid classical-quantum ensemble models  
- Cross-validation instead of single train-test split  
- Deployment-ready churn prediction API  

---

## 📚 Conclusion

This project provides a practical comparison between classical ML and quantum ML approaches for churn prediction.

At present, **classical ensemble methods outperform quantum classifiers on structured tabular data**, while quantum approaches face scalability and hardware-related limitations. However, the exploration offers valuable insight into the evolving landscape of Quantum Machine Learning.

---

## 👨‍💻 Author

**Aayush Sharda**  
Computer Science (AI & ML)  
Manipal Institute of Technology, Bengaluru  