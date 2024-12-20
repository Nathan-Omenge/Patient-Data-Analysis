# Patient-Data-Analysis


This project focuses on analyzing patient data using R, with the primary goals of data cleaning, imputation, and identifying the best-fitting statistical distributions for various subsets of the dataset. Visualizations and metrics provide actionable insights for healthcare management.

---

## 📂 Files in This Repository:
- **Patient_Data_Analysis.Rmd**: R Markdown file containing the code for data preprocessing, statistical analysis, and visualizations.

---

## 💻 Key Topics Covered:
### 1. **Data Cleaning and Imputation**
- Identified and handled missing data points using:
  - **Mode imputation** for categorical variables like gender.
  - **Median imputation** for numerical variables like age.
- Validated and corrected inconsistencies in dates (e.g., swapped check-in and check-out dates).

### 2. **Data Normalization and Transformation**
- Applied min-max normalization to prepare data for fitting beta distributions.

### 3. **Fitting Statistical Distributions**
- Evaluated multiple distributions (`norm`, `gamma`, `logis`, `weibull`, `exp`, etc.) to find the best fit for different patient subsets.
- Used AIC and BIC scores to identify the best-fitting model.

### 4. **Subset Analysis**
- Analyzed distinct patient groups:
  - Male and female patients.
  - Resident and non-resident patients.
- Generated histograms and overlaid fitted distributions for better understanding.

### 5. **Visualization**
- Created interactive and static visualizations using `ggplot2` and `plotly` to display:
  - Histograms with density curves for patient subsets.
  - Distributions fitted to days spent at the hospital.

---

## 🛠️ Libraries Used:
- **dplyr**: For data manipulation and filtering.
- **fitdistrplus**: For fitting statistical distributions.
- **ggplot2**: For creating static visualizations.
- **plotly**: For interactive visualizations.
- **readxl**: For reading Excel files.
- **lubridate**: For date manipulation.
- **naniar**: For identifying and visualizing missing data.

---

## 📊 Visualizations:
1. **Histograms with Fitted Distributions**:
   - Showed the number of days spent in the hospital across different patient groups.
   - Overlaid with density curves for various fitted distributions.

2. **Interactive Plots**:
   - Used `plotly` to provide dynamic exploration of patient data distributions.

---

## 🚀 How to Run:
1. Open `Patient_Data_Analysis.Rmd` in RStudio.
2. Install the required libraries if not already installed:
   ```R
   install.packages(c("dplyr", "fitdistrplus", "ggplot2", "plotly", "readxl", "lubridate", "naniar"))
