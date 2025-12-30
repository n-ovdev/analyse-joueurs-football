# ⚽ Football Players Data Analysis

## 📋 Description

Football players data analysis project created as part of my Data Analysis learning journey. This project demonstrates my skills in SQL, Python, Pandas, and data visualization.

## 🎯 Objectives

- Analyze professional football players' characteristics
- Clean and prepare data
- Create relevant statistical analyses
- Produce clear visualizations
- Calculate a composite performance score

## 🔧 Technologies Used

- **Python 3.x**
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Chart creation
- **Jupyter Notebook**: Development environment
- **SQL**: Query extraction (pandas equivalent)

## 📊 Dataset

- **Source**: Professional football players data
- **Main columns**:
  - `name`: Player name
  - `age`: Age
  - `overall`: Overall rating
  - `vitesse`: Speed
  - `potentiel`: Player potential
  - `club_name`: Club
  - `pays`: Country
  - `salaire`: Salary

## 🧹 Cleaning Process

1. ✅ Missing values check
2. ✅ Duplicates check
3. ✅ Data types correction
4. ✅ Addition of calculated `potentiel` column
5. ✅ Format standardization

## 📈 Analyses Performed

### 1. Descriptive analyses
- Top 3 fastest players
- Average overall by club
- Total salary by country
- Explosive players (speed >= 90)

### 2. Composite score
Performance score calculation based on:
- Overall (50%)
- Speed (30%)
- Potential (20%)

### 3. Visualizations
- Top 5 players by overall (bar chart)
- Total salary by country (bar chart)
- Speed vs overall relationship (scatter plot)
- Composite score by player

## 📂 Project Structure
```
football-project/
│
├── projet_foot.ipynb          # Main notebook
├── joueurs.csv                # Dataset
├── joueurs_clean.csv          # Clean data
├── top5_overall.png           # Top 5 chart
├── salaire_par_pays.png       # Salary chart
├── scatter_vitesse_overall.png # Scatter plot
├── score_composite.png        # Composite score
└── README.md                  # Documentation
```

## 🚀 Installation and Usage

### Prerequisites
```bash
pip install pandas matplotlib jupyter
```

### Execution
```bash
jupyter notebook projet_foot.ipynb
```

## 📊 Key Results

- **Number of players analyzed**: [Your number]
- **Player with best overall**: [Name]
- **Country with highest wage bill**: [Country]
- **Speed/overall correlation**: Positive

## 🎓 Skills Demonstrated

- Data manipulation with Pandas
- Statistical analysis (averages, groupby, aggregations)
- Custom metrics creation (composite score)
- Data visualization
- Data cleaning and preparation
- Technical documentation

## 🔄 SQL Equivalent

The pandas analyses in this project can be performed in SQL:
```sql
-- Top 3 fastest players
SELECT name, vitesse 
FROM joueurs 
ORDER BY vitesse DESC 
LIMIT 3;

-- Average overall by club
SELECT club_name, AVG(overall) as overall_moyen
FROM joueurs 
GROUP BY club_name;

-- Total salary by country
SELECT pays, SUM(salaire) as salaire_total
FROM joueurs 
GROUP BY pays 
ORDER BY salaire_total DESC;
```

## 📧 Contact

**NOAH TONTOLO**
- LinkedIn: NOAH TONTOLO
- Email: noahtontolo@gmail.com
- Portfolio: ComeUp, FIverr, Malt.

## 📝 License

This project is open-source and for educational purposes.

---

## 🔗 Other Projects

- [E-commerce Data Cleaning](link-to-your-other-repo)
