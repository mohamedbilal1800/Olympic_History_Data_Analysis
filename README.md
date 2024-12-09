# **Olympic Games Data Analysis Project**

## **Overview**
This project explores the **120 Years of Olympic History: Athletes and Results** dataset, analyzing athlete demographics, country performances, medal achievements, and the evolution of the Olympic Games from **1896 to 2016**. The insights and visualizations generated in this analysis provide a comprehensive understanding of the trends and patterns in Olympic history.

---

## **Dataset Information**
The analysis is based on two datasets:  
1. **`athlete_events.csv`**:
   - Contains detailed information about athletes, events, and medal achievements.
   - **Rows**: 271,116  
   - **Columns**: 15  
   - Key features: Athlete demographics, event details, and medal types.  

2. **`noc_regions.csv`**:
   - Maps National Olympic Committees (NOCs) to corresponding countries/regions.
   - **Columns**: 3 (NOC, region, notes)  

---

## **Key Features of the Project**
### **1. Data Cleaning**
- Merged `athlete_events.csv` and `noc_regions.csv` to create a unified dataset.  
- Handled missing values in columns such as `Medal`, `Age`, `Height`, and `Weight`.  
- Consolidated inconsistent country names (e.g., `Singapore-1`, `Singapore-2`).  
- Removed duplicate rows and irrelevant columns.

### **2. Feature Engineering**
- Created new features:
  - **BMI**: Body Mass Index of athletes.
  - **Age Categories**: Budding Competitor (<20), Rising Competitor (20–25), Seasoned Competitor (26–35), Senior Competitor (>35).  
  - **Event Era**: Foundational Era (≤1950), Growth Era (1951–2000), Modern Era (≥2001).  
  - **Sports Categories**: Team Sports vs. Individual Sports.  

### **3. Exploratory Data Analysis (EDA)**
- Explored variations in athlete **age, height, weight, and BMI** over time.  
- Analyzed the **participation trends** of male and female athletes.  
- Examined the dominance of top-performing countries (USA, Russia, Germany).  
- Investigated the impact of hosting the Olympics on a nation's performance.  

### **4. Visualizations**
- Generated insightful visualizations using Python libraries like **Matplotlib** and **Seaborn** to highlight trends and patterns.

---

## **Key Insights**
1. **Athlete Demographics**:
   - Most athletes are aged between **20 and 30**, with height and weight showing consistent increases over time.  
   - BMI analysis revealed that athletes in strength-based sports have higher BMI due to muscle mass.  

2. **Country Performances**:
   - The **USA**, **Russia**, and **Germany** dominate Olympic history in total medal counts.  
   - Host nations often perform better, benefiting from home-ground advantages and increased athlete participation.

3. **Medal Achievements**:
   - Only **20.76%** of Olympic participants win medals, emphasizing the elite nature of medalists.  
   - **Michael Phelps** holds the record for the most medals (28) and golds (23).  

4. **Gender Trends**:
   - Female participation has significantly increased since the late 20th century, nearing parity with male athletes in recent years.

---

## **Technologies Used**
- **Programming Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn  
- **Data Visualization**: Graphs, plots, and heatmaps for EDA insights.  

---

## **Repository Structure**
```
.
├── data/
│   ├── athlete_events.csv
│   ├── noc_regions.csv
├── notebooks/
│   ├── Olympic_Data_Analysis.ipynb
├── README.md
└── outputs/
    ├── visualizations/
    └── final_report.pdf
```

---

## **How to Use**
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/olympic-data-analysis.git
   ```
2. Navigate to the project directory:  
   ```bash
   cd olympic-data-analysis
   ```
3. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
4. Open the Jupyter Notebook to explore the analysis:  
   ```bash
   jupyter notebook notebooks/Olympic_Data_Analysis.ipynb
   ```

---

## **Future Scope**
- Include analysis of newly added sports in post-2016 Olympics.  
- Explore the impact of technological advancements on athlete performance.  
- Conduct a comparative analysis of underperforming nations to identify areas for growth.  

---

## **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
