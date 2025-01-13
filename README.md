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

While males and females were almost equally represented overall, the age group distributions were distinct. Most participants were middle-aged, primarily in the 31-40 and 41-50 age groups. Younger groups had more males, while older groups, most notably in the 51-60 range, were predominantly female.


### **Gender and Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/gender-sleep.png)

On average, females rated their sleep quality to be slightly higher than males. Women consistently scored one point higher at the 25th, 50th,and 75th percentiles. A Welch's t-test confirmed this difference, meaning it's unlikely due to chance. This suggests better sleep quality among females, aligning with trends from earlier research that have found that women tend to sleep slightly longer and higher sleep efficiency than men.

### **Age and Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/age-sleep.png)

There was quite a bit of variability in sleep quality among the age groups. The 20-30 group had the lowest average, mostly between 6 and 7, while the 51-60 group clustered tightly around 9, indicating the best sleep quality compared to the other groups.A Spearman's rank coefficient of 0.42 shows a moderate positive link between age and sleep quality, suggesting improvement with age. However, this trend contradicts much existing research that has found an increase of sleep disturbances and decreased time spent in deep sleep with age. This highlights the need to investigate potential confounding factors such as the distribution of BMI or sleep durations among these age groups. 

### **Occupation and Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/occupation-sleep.png)

Sleep quality ratings varied across occupations in this dataset with engineers reporting the highest average ratings. Salespeople had the lowest ratings, followed by doctors, and nurses showed the highest variability in ratings among the seven occupations. Higher sleep quality could be linked to a more consistent work schedule while irregular work hours may contribute to lower ratings. Variability among ratings within certain occupations could be indicative of the diverse nature of their fields. It would be interesting to perform a further analysis on stress levels and physical activity between these occupations and how they play into reported sleep quality.

### **Sleep Duration, Stress Level, and Sleep Quality**

<p float="left">
  <img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/sleep-duration-quality.png" width="45%" />
  <img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/stress-sleep.png" width="45%" />
</p>

Sleep quality increases with sleep duration. Conversely, increased stress level correlates with reduced sleep quality. This suggests that an adequate amount of sleep and stress management strategies are essential for improving sleep quality. 

### **Sleep Disorders, BMI, and Sleep Quality**
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/bmi-disorder-proportions.png)
![alt text](https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/bmi-disorder-sleep.png)

Overweight and obese individuals make up a large percentage of those with sleep apnea and insomnia. People without sleep disorders, particularly in the normal BMI range, report higher sleep quality. For sleep apnea, both healthy weight and obese individuals have a similar median sleep quality while overweight individuals report lower and more varied ratings. Insomnia shows lower sleep quality among overweight and obese individuals compared to those with a normal BMI, highlighting the link between BMI, sleep disorders, and reduced sleep quality. 

