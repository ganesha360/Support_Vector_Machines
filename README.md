# Support Vector Machines (SVM) — Binary Classification

## 📘 Project Overview
This project demonstrates the implementation of **Support Vector Machines (SVM)** for both **linear and non-linear classification** using the **Breast Cancer dataset**.  
The goal is to classify whether a tumor is **Malignant (M)** or **Benign (B)** using SVMs with different kernels and visualize their performance.

---

## 🧰 Tools & Libraries Used
- **Python**
- **Pandas** – data handling
- **NumPy** – numerical operations
- **Matplotlib / Seaborn** – visualization
- **Scikit-learn** – for preprocessing, model training, and evaluation

---

## 🧩 Steps Performed

### 1️⃣ Load & Explore Data
- Loaded the `breast-cancer.csv` dataset.
- Dropped unnecessary columns (like IDs).
- Checked for missing values and data types.

### 2️⃣ Preprocessing
- Encoded the target column **(diagnosis)**:  
  - `M → 1` (Malignant)  
  - `B → 0` (Benign)
- Standardized all numeric features using **StandardScaler** for better model performance.

### 3️⃣ Train-Test Split
- Split data into **80% training** and **20% testing** sets.

### 4️⃣ Train Models
- Trained two models:
  - 🔹 **Linear Kernel SVM**
  - 🔹 **RBF Kernel SVM (non-linear)**

### 5️⃣ Model Evaluation
- Evaluated using:
  - ✅ **Accuracy Score**
  - ✅ **Confusion Matrix**
  - ✅ **Classification Report** (Precision, Recall, F1-score)
- Compared linear vs RBF performance.

### 6️⃣ Hyperparameter Tuning
- Tuned **C** and **gamma** values in the RBF kernel to improve performance.

### 7️⃣ Cross-Validation
- Used **5-fold Cross Validation** to ensure model reliability and avoid overfitting.

### 8️⃣ Visualization
- Applied **PCA** to reduce features to 2D.
- Plotted decision boundaries to show how SVM separates classes visually.

---

## 📊 Visualization Samples
| Visualization | Purpose |
|----------------|----------|
| `sns.heatmap(confusion_matrix)` | Show model performance |
| `plt.contourf()` | Display decision boundaries after PCA |
| `plt.scatter()` | Visualize class separation |

---

## ✅ Results
- Both SVM models achieved **high accuracy** in classifying cancerous vs non-cancerous cases.  
- **Linear SVM** performed well, but **RBF kernel** captured non-linear relationships better.  
- Achieved a strong **cross-validation accuracy**, confirming model stability.  
- Visualization clearly shows two separable clusters after PCA.

---

## 💾 Files Included
- `breast-cancer.csv` — dataset  
- `SVM_Classification.ipynb` — full implementation code  
- `README.md` — documentation  

---

## 📚 Learning Outcome
Through this project, I learned:
- How **SVMs** work for both linear and non-linear problems.  
- The impact of **kernel choice (linear vs RBF)** on model performance.  
- How to tune hyperparameters like **C** and **gamma**.  
- How to visualize **decision boundaries** using PCA.

---

## 🧑‍💻 Author
**Ganesh R**  
*(Junior AIML Engineer Trainee)*
