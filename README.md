# MomoData Analysis Dashboard

## 📊 Project Overview

This project is an end-to-end fullstack application designed to analyze and visualize SMS transaction data from MTN MoMo, a major mobile payment provider in Rwanda. The application parses and processes SMS data stored in XML format, stores cleaned and categorized information in a relational database, and provides a dynamic dashboard for users to explore key insights.

## 🎯 Objectives

- Parse and clean raw SMS data from XML files.
- Categorize transactions into meaningful types.
- Store structured data in a relational database.
- Build a user-friendly web dashboard to visualize transaction insights.

## 🧩 Features

- **Backend Data Processing**:
  - XML parsing and data extraction
  - Data cleaning and normalization (amounts, dates, text)
  - Categorization into transaction types (e.g., withdrawals, transfers, payments)

- **Database Integration**:
  - Relational database schema design (sqlite)
  - Data insertion scripts with duplicate handling
  - Logging for unprocessable entries

- **Frontend Dashboard**:
  - Interactive filtering by transaction type, amount, date (mm/dd/yy, mm/yy & yy)
  - Data visualizations: pie charts, bar charts
  - Detailed transaction view

## 🏗️ Tech Stack

- **Backend**: Python (flask)
- **Database**: sqlite
- **Frontend**: HTML, CSS
- **Visualization**: python(plotly)

## 🗃️ Project Structure
```
├── Data
    ├── modifies_sms_v2.xml
├── static
    ├── styles.css
├── templates
    ├── Index.html
├── db_setup.py
├── insert_data.py
├── parse_data.py
├── load_data.py
├── app.py
├── requirements.txt
├── transactions.db
```
## 🚀 Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Gaddy01/MomoData-Analysis-Summative.git
   cd MomoData-Analysis-Summative
   ```
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   ⚠️ To avoid conflicts, it is advised to delete the 'transactions.db' file before continuing.
   
4. **Create your database structure**
   ```bash
   python db_setup.py
   ```
5. **Parse and load the data into the database**
   ```bash
   python load_data.py
   ```
6. **Launch the web app**
   ```bash
   python app.py
   ```
7. **Access the dashboard**
   Visit http://localhost:5000 in your browser.

⚠️ **NB. Run the 'db_setup.py' & 'load_data.py' scripts only once. if you want to rerun the web app, just run 'app.py' script only!**

## 📌 Additional links:

1. **Demonstration video link**
   ```bash
   https://drive.google.com/file/d/1ONcZcYORdkjZpnGV5FOWvXU3vmep6p_i/view?usp=sharing
   ```
2. **Project report link**
   ```bash
   https://docs.google.com/document/d/15D54p-Jztp8zniLw3eeuKH6C1esYZZxNImzVYiWPCHk/edit?usp=sharing
   ```

## 📝 Authors

   Gaddiel Irakoze