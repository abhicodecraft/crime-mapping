# Crime Mapping and Forecasting System

A web-based data analytics and machine learning application for analyzing crime patterns, visualizing crime hotspots, and forecasting future crime trends using historical crime data.

---

## 🚀 Features

### 🔥 Interactive Crime Heatmap
- Visualizes city-wise crime density using geospatial heatmaps.
- Helps identify high-risk and low-risk areas instantly.

### 🎛️ Smart Filters
Filter crime data dynamically by:
- Time of day (Morning, Afternoon, Evening, Night, Late Night)
- Victim gender
- Crime domain (e.g., Theft, Assault, Fraud)
- City

### 🚨 Crime Severity Classification
- Uses police deployment data to classify crime severity into:
  - **Low**
  - **Medium**
  - **High**

### 📈 7-Day Crime Forecast
- Predicts total crime count for the next 7 days.
- Uses **ARIMA time series forecasting**.
- Displays both historical and forecasted trends in a graph.

### 🏙️ City-wise Crime Prediction
For a selected city, the system predicts:
- Most likely crime types
- Most frequent crime domains
- Expected crime severity
- Confidence level based on data availability

---

## 🧠 Tech Stack

| Category | Technologies |
|--------|-------------|
| Backend | Python, Flask |
| Data Processing | Pandas, NumPy |
| Machine Learning | ARIMA (pmdarima) |
| Visualization | Folium, Matplotlib |
| Frontend | HTML, CSS, JavaScript |

## 📂 Project Structure

```
Crime-Mapping/
│
├── app.py                    # Main Flask application
├── src/
│   ├── data_loader.py        # Loads crime dataset
│   ├── preprocess.py         # Date & time preprocessing
│   ├── aggregations.py       # City-level aggregations
│   ├── geocode.py            # City latitude & longitude mapping
│   └── viz.py                # Heatmap generation logic
│
├── data/                     # Crime dataset
├── notebooks/                # Exploratory data analysis
├── templates/                # HTML templates
├── static/                   # CSS files and generated map
├── tests/                    # Unit tests
├── requirements.txt          # Python dependencies
└── README.md
```


## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/AbhiCodeCraft/Crime-Mapping.git
cd Crime-Mapping
```

### 2️⃣ Install dependencies
```
pip install -r requirements.txt
```

### 3️⃣Run the application
```
python app.py
```

### 4️⃣ Open in browser
```
http://127.0.0.1:5000
```
