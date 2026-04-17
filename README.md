# 🧠 Brain Connectivity Analysis: Child vs Adult

## Objective
To analyze open-source fMRI data and identify functional connectivity differences between **children** and **adults**, and to build a **machine learning classifier** that predicts age group based on brain connectivity patterns.

---

## Tools & Libraries
- **Python** – Primary programming language  
- **Nilearn** – Neuroimaging data handling, atlas mapping, and visualization  
- **Scikit-learn** – Machine Learning (Support Vector Machine)  
- **Pandas / NumPy** – Data manipulation and preprocessing  

---

## Dataset
- Open-access fMRI data from the **Development fMRI dataset**  
- Included in **Nilearn**, originally derived from **OpenNeuro**  

---

## Methodology

### 1. Preprocessing
- Applied **standardization**  
- Applied **spatial smoothing** (6mm FWHM)

### 2. Region of Interest (ROI) Extraction
- Used the **Harvard-Oxford Atlas**  
- Extracted time-series data from **48 cortical regions**

### 3. Connectivity Analysis
- Computed **Pearson correlation matrices**  
- Represented functional connections between brain regions  

### 4. Machine Learning
- Implemented **Linear Support Vector Machine (SVM)**  
- Applied **cross-validation**  
- Classified subjects into:
  - **Child**
  - **Adult**
- Features used: **connectome (connectivity matrices)**  

---

## Key Findings
- The model successfully identified **distinct connectivity patterns** in children  
- Visualization highlights **fronto-parietal connectivity differences** between age groups  
- **Limitation:** Small sample size (**N = 10**) impacts generalization  

---

## Visual Outputs
- **Atlas Overlay** – Mapping of brain regions  
- **Correlation Matrix** – Heatmap of inter-regional connectivity  
- **Connectome Graph** – Visualization of most predictive brain connections  

---

## How to Run

1. Install dependencies:
   ```bash
   pip install nilearn pandas matplotlib scikit-learn jupyter
   
2. Open the notebook:
   Neuro_Connectome_Analysis.ipynb
   
3. Run all cells to produce results.
