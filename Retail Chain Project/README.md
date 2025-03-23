# Retail Chain Project
This project uses a **synthetically generated dataset** that simulates real-world sales transaction data for a large UK-based retail chain.  

- The **dataset** was generated using Python and includes **1.5 million rows** of transactional data.  
- The **business scenario** and challenges were provided by ChatGPT, mimicking realistic struggles a retail company may face.  
- The **goal** of this project is to **perform data cleaning, exploratory data analysis (EDA)**, and create a **Power BI dashboard** to extract actionable insights.  

### **Company Overview**
Client is a multi-channel retail chain operating in the UK.  
- It has **50 physical stores** and a growing **online platform**.  
- The company sells products across four main categories:  
  - **Groceries:** Fresh produce, packaged food, and beverages.  
  - **Electronics:** Gadgets, home appliances, and personal devices.  
  - **Clothing:** Apparel, footwear, and accessories.  
  - **Home Goods:** Furniture, decor, and household items.  
- Customers can pay via **Cash, Credit Card, Debit Card, or Digital Wallet**.  

---

### **Data Source**
The dataset simulates real-world sales data pulled from:  
- **Point of Sale (POS)** systems at physical store locations.  
- **E-commerce platform** logs for online transactions.  
- **Customer loyalty programme** data, providing demographic insights.  
- **Payment processor logs**, capturing payment methods, discounts, and transaction details.  

---

### **Business Struggles**
1. **Revenue leakage** due to inconsistent discount practices.  
2. Unclear performance comparison between **online vs in-store** channels.  
3. Lack of insights into **customer demographics** and purchasing behaviour.  
4. Limited visibility into **payment method preferences**.  
5. **Data quality issues** with duplicate transactions, missing customer details, and inconsistent date formats.  

---

### **Main Objectives of the Project**
- Clean and standardise the dataset by:  
  - Removing duplicates.  
  - Handling missing values.  
  - Standardising date formats.  
- Perform **exploratory data analysis (EDA)** to:  
  - Identify revenue drivers.  
  - Compare online vs in-store performance.  
  - Analyse customer demographics.  
  - Examine payment method trends.  
- Create a **Power BI dashboard** to visualise insights, including:  
  - Sales performance by category and store.  
  - Discount and promotion analysis.  
  - Customer demographics trends.  
  - Online vs in-store sales comparison.  
  - Payment method preferences.  

---

## **Dataset Description**
- **Rows:** 1,600,000 (including 0.5% duplicates)  
- **Columns:** 14  
- **Attributes:**  
    - `transaction_id`: Unique identifier for each transaction.  
    - `customer_id`: Unique customer ID.  
    - `store_id`: Store location (including online).  
    - `date`: Transaction date (with some inconsistent formats).  
    - `product_category`: Category of the purchased item.  
    - `product_name`: Product name.  
    - `quantity`: Number of items purchased.  
    - `unit_price`: Price per unit.  
    - `total_amount`: Total transaction amount.  
    - `payment_method`: Payment method used.  
    - `discount_applied`: Discount percentage applied.  
    - `customer_age`: Age of the customer (with some missing values).  
    - `customer_gender`: Gender of the customer (with some missing values).  
    - `online_order`: 1 = online, 0 = physical store.  

---

### 🛠️ **Data Generation Code**
The dataset was generated using the Python script below:  
[Link to Data Generation Notebook](https://github.com/HSSC01/Portfolio/tree/main/Retail%Chain%Project/retail_chain_synthetic_data_generation.ipynb)  

---