# **Demographic and Health Factors on Sleep Quality**
This project investigates various factors that influence sleep quality through data analysis and visualization techniques.

## **Table of Contents**
- [Introduction](#Introduction)
- [Data](#Data)
- [Installation](#Installation)
- [Usage](#Usage)
- [Results](#Results)

## **Introduction**

Sleep plays a crucial role in our cognitive, physical, and emotional well-being, yet poor sleep health remains a growing global concern. Insufficient sleep is linked to impaired decision-making, mental health challenges, and chronic conditions such as hypertension and type 2 diabetes. This project analyzes the influence of demographic and health factors on sleep quality in an effort to gain insights that could inform effective improvement strategies.

## **Data**

The data was obtained from [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset). It is located in the `/data/sleep-and-lifestyle.csv` file. The dataset consists of 374 observations including variables such as gender, age, occupation, sleep duration, stress levels, BMI, and the presence of sleep disorders.

## **Installation**

To run the analysis, you need to have the following Python libraries installed:
- pandas
- numpy
- seaborn
- matplotlib
- scipy

You can install these libraries using pip:
```bash
pip install pandas numpy seaborn matplotlib scipy
```
## **Usage**
1. Clone the repository:
   ```bash
   git clone https://github.com/jasmineamjadi/sleep-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd sleep-analysis
   ```
3. Open the notebook `sleep-quality-analysis.ipynb` in Jupyter Notebook or Jupyter Lab to view and run the analysis:
   ```bash
   jupyter notebook sleep-quality-analysis.ipynb
   ```

## **Results**
### **Gender and Age Distribution**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/gender-age-distribution.png)
### **Gender vs. Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/gender-sleep.png)
### **Age vs. Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/age-sleep.png)
### **Occupation vs. Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/occupation-sleep.png)
### **Sleep Duration vs. Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/sleep-duration-quality.png)
### **Stress Levels vs. Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/stress-sleep.png)
### **Sleep Disorders, BMI, and Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/bmi-disorder-proportions.png)
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/bmi-disorder-sleep.png)
