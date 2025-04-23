# Retail Chain Project
This project uses a **synthetically generated dataset** that simulates real-world sales transaction data for a large UK-based retail chain.  

- The **dataset** was generated using Python and includes **1.5 million rows** of transactional data.  
- The **business scenario** and challenges were provided by ChatGPT, mimicking realistic struggles a retail company may face.  
- The **goal** of this project is to **perform data cleaning, exploratory data analysis (EDA)**, and create a **written report** to highlight actionable insights.  

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
- Generate **1.5million rows** of synthetic data by:
  - Generating customer demographics (e.g., age, gender, location, income level).
  - Implementing realistic purchase behaviour, such as:
    - Randomising purchase frequency per customer.
    - Assigning discounts, promotions, and sales events to certain transactions.
    - Simulating payment methods used in the transactions (e.g., credit card, cash, mobile payment).
  - Adding some realistic messiness, such as:
    - Generating a mix of wrong formats for certain data points (e.g., dates in different formats).
    - Introducing missing values in some columns (e.g., incomplete customer details, missing transaction data).
    - Adding duplicates where necessary to simulate errors in large datasets.
- Clean and standardise the dataset by:  
  - Removing duplicates.  
  - Handling missing values.  
  - Standardising date formats.  
- Perform **exploratory data analysis (EDA)** to:  
  - Identify revenue drivers.  
  - Compare online vs in-store performance.  
  - Analyse customer demographics.  
  - Examine payment method trends.  


---

## **Dataset Description**

### **1. Point of Sales (POS) Data** (~1.5 million rows of transactions)

- **Columns:**
  - `transaction_id`: Unique identifier for each transaction.  
  - `customer_id`: Unique customer ID (links to the customer dataset).  
  - `store_id`: Store location (including online).  
  - `date`: Transaction date (with some inconsistent formats).  
  - `category`: Category of the purchased item (links to the product dataset).  
  - `product_name`: Product name (links to the product dataset).  
  - `quantity`: Number of items purchased.  
  - `payment_method`: Payment method used (e.g., credit card, cash, mobile payment).  
  - `discount_applied`: Discount percentage applied to the transaction.  
  - `online_order`: 1 = online, 0 = physical store.

### **2. Customer Data** (~700k unique customers/rows)

- **Columns:**
  - `customer_id`: Unique customer ID (links to the POS dataset).  
  - `age`: Age of the customer (with some missing values).  
  - `gender`: Gender of the customer (with some missing values).

### **3. Product Data** (~800 products)

- **Columns:**
  - `product_name`: Name of the product (links to the POS dataset).  
  - `unit_price`: Price per unit of the product.  
  - `category`: Category of the product (e.g., Electronics, Fashion, Home Appliances).


---

### 🛠️ **Data Generation Code**
The dataset was generated using the Python script below:  
[Link to Data Generation Notebook](https://github.com/HSSC01/Portfolio/blob/main/Retail%20Chain%20Project/code/retail_chain_synthetic_data_generation.ipynb)  

---