# TOPSIS – Multi Criteria Decision Making System

**Name:** Raghav Pahwa  
**Roll No:** 102303608  
**Course:** UCS654

---

## 📖 Introduction

This project implements **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)**, a multi-criteria decision analysis method used to rank alternatives based on multiple criteria. TOPSIS helps identify the best option by measuring proximity to the ideal solution.

**Project Components:**
- **Part 1:** Command Line TOPSIS Program
- **Part 2:** Python Package (PyPI)
- **Part 3:** Streamlit Web Application

---

## 🔄 Methodology

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│      Data       │────▶│      Data       │────▶│  Normalization  │────▶│     Weight      │
│   Collection    │     │ Pre-processing  │     │                 │     │   Assignment    │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
                                                                                  │
                                                                                  ▼
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│     Result      │◀────│     Ranking     │◀────│    Distance     │◀────│  Ideal Best/    │
│    Analysis     │     │                 │     │   Calculation   │     │  Ideal Worst    │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
```

---

## 📋 Description

- **Input:** CSV file with alternatives and multiple criteria
- **Processing:** Normalization, weight assignment, and distance calculation
- **Output:** TOPSIS scores and rankings for all alternatives
- **Features:** Command-line tool, Python package, and interactive web interface

---

## 📊 Input / Output

### Sample Input Data

**File:** `input.csv`

```csv
Model,Price,Storage,Camera,Looks,Battery
M1,250,16,12,5,2500
M2,200,8,8,3,1800
M3,300,16,16,4,2200
M4,275,32,8,4,2000
M5,225,16,16,2,1500
```

### Parameters

- **Weights:** `0.25,0.25,0.25,0.15,0.10`
- **Impacts:** `+,-,+,+,+`

### Sample Output

**File:** `result.csv`

```csv
Model,Price,Storage,Camera,Looks,Battery,TOPSIS Score,Rank
M1,250,16,12,5,2500,0.5345,3
M2,200,8,8,3,1800,0.4234,5
M3,300,16,16,4,2200,0.6912,1
M4,275,32,8,4,2000,0.4789,4
M5,225,16,16,2,1500,0.6124,2
```

---

## 🔗 Live Links

### PyPI Package
**Installation:**
```bash
pip install topsis-raghav-102303608
```
**Link:** [PyPI Package](https://pypi.org/project/topsis-raghav-102303608/)

### Streamlit Application
**Link:** [Streamlit App](https://topsis-raghav.streamlit.app/)

---

## 📁 Project Structure

```
TOPSIS-Project/
│
├── Part1/
│   ├── topsis.py
│   └── data.csv
│
├── Part2/
│   ├── setup.py
│   └── topsis_raghav_102303608/
│
├── Part3/
│   └── app.py
│
└── README.md
```

---

## 📸 Screenshots

### Command Line Interface
![CLI Screenshot](screenshots/cli.png)

### Streamlit Web Application
![Streamlit Interface](screenshots/streamlit_app.png)

---

## 🚀 Usage

### Command Line
```bash
python topsis.py input.csv "0.25,0.25,0.25,0.15,0.10" "+,-,+,+,+" result.csv
```

### Python Package
```python
from topsis_raghav_102303608 import topsis
topsis.calculate('input.csv', '0.25,0.25,0.25,0.15,0.10', '+,-,+,+,+', 'result.csv')
```

### Web Application
```bash
streamlit run app.py
```

---

## 📄 License

MIT License

---

**Raghav Pahwa** | Roll No: 102303608 | UCS654