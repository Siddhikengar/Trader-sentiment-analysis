# Trader-Sentiment-Analysis

Analyze how trader performance changes with market sentiment using the **Fear & Greed Index** and historical trading data.

---

## 📌 Project Objective
This project studies the relationship between **market sentiment** and **trading performance**.  

We aim to answer questions like:  
- Do traders earn more during **Fear** or **Greed**?  
- Does trading frequency change with sentiment?  
- How does risk-taking vary across market moods?  

---

## 📁 Project Structure


``` project/
│
├── data/                 # Input datasets
│   ├── fear_greed_index.csv
│   └── historical_data.csv
│
├── output/               # Generated charts and visualizations
│   └── *.png / *.jpg
│
├── analysis.ipynb         # Main analysis notebook
├── requirements.txt
└── README.md

```


---

## 📂 Datasets

### Fear & Greed Index (`data/fear_greed_index.csv`)
Daily crypto market sentiment.

| Column | Description |
|--------|-------------|
| date | Date of sentiment |
| value | Score (0–100) |
| classification | Fear / Neutral / Greed |

### Historical Trades (`data/historical_data.csv`)
Trader transaction history.

| Column | Description |
|--------|-------------|
| timestamp | Trade time |
| symbol | Asset traded |
| side | Buy / Sell |
| price | Trade price |
| quantity | Amount traded |
| pnl | Profit/Loss |

---

## 🧰 Requirements
Install the following Python libraries. Add them to `requirements.txt`:

pandas
numpy
matplotlib
seaborn
jupyter




---

## ⚙️ Setup Instructions

### Step 1 — Download Project
Download the project folder and place datasets inside the `data/` folder.

### Step 2 — Create Virtual Environment
**Windows**
```bash
python -m venv venv
venv\Scripts\activate


Mac/Linux

python3 -m venv venv
source venv/bin/activate

Step 3 — Install Dependencies
pip install -r requirements.txt 
```



## ▶️ How to Run

Start Jupyter Notebook:

jupyter notebook


Open analysis.ipynb and run all cells.

Charts and visualizations will be saved automatically in the output/ folder.



## 🧠 Notebook Workflow

1️⃣ Load Data

sentiment = pd.read_csv("data/fear_greed_index.csv")
trades = pd.read_csv("data/historical_data.csv")


2️⃣ Data Cleaning

Convert timestamps to datetime

Handle missing values

Extract trade date

3️⃣ Merge Datasets

Join trades with sentiment using date

4️⃣ Exploratory Data Analysis

Profit vs sentiment

Trade count vs sentiment

Win rate vs sentiment

5️⃣ Visualizations

Charts and insights explaining trader behavior



## 📊 Output

The notebook generates:

Insightful charts (saved in output/)

Aggregated performance metrics

Sentiment-based trading insights
