# Customer Segmentation

This project performs **customer segmentation** using the [Online Retail Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/). It applies **EDA, RFM analysis, and K-Means clustering** to uncover customer behavior patterns for both UK and Non-UK customers.

---

## 📊 Dataset
- Source: Online Retail Dataset (UCI Machine Learning Repository)  
- Records: 406,829 transactions  
- Columns: `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## ⚙️ Methods
1. **Data Cleaning**  
   - Handle missing values  
   - Remove anomalies (`Quantity <= 0`, `UnitPrice <= 0`)  

2. **Exploratory Data Analysis (EDA)**  
   - Descriptive statistics  
   - Customer origin distribution  
   - Weekly and monthly purchase trends  

3. **Feature Engineering (RFM)**  
   - **Recency**: days since last purchase  
   - **Frequency**: number of purchases  
   - **Monetary**: total amount spent  

4. **Modeling**  
   - Standardization with `StandardScaler`  
   - K-Means clustering  
   - Optimal clusters evaluated using **Silhouette Score**  

---

## 🚀 How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

3. Open the notebook:
   ```bash
   jupyter notebook customer_segmentation.ipynb

## 📈 Results
    -  Customers segmented into different clusters based on RFM metrics.
    -  Clear differences observed between UK and Non-UK customers.

## 🛠️ Tools & Libraries
    -  Python, Jupyter Notebook
    -  Numpy, Pandas, Matplotlib, Seaborn
    -  Scikit-learn
