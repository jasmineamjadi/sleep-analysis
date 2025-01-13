# **Demographic and Health Factors on Sleep Quality**
This project investigates various factors that influence sleep quality through data analysis and visualization techniques.

## **Table of Contents**
- [Introduction](#Introduction)
- [Data](#Data)
- [Installation](#Installation)
- [Usage](#Usage)
- [Results](#Results)

## **Introduction**

Sleep plays a crucial role in our cognitive, physical, and emotional well-being, yet poor sleep health remains a growing global concern. Insufficient sleep is linked to impaired decision-making, mental health challenges, and chronic conditions such as hypertension and type 2 diabetes.<a href="#References"><sup>[1]</sup></a><a href="#References"><sup>[2]</sup></a><a href="#References"><sup>[3]</sup></a><a href="#References"><sup>[4]</sup></a>

<sup>[1]</sup><sup>[2]</sup><sup>[3]</sup><sup>[4]</sup>  

This project analyzes the influence of demographic and health factors on sleep quality in an effort to gain insights that could inform effective improvement strategies.

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
<img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/gender-age-distribution.png" alt="isolated" width="80%"/>

While males and females were almost equally represented overall, the age group distributions were distinct. Most participants were middle-aged, primarily in the 31-40 and 41-50 age groups. Younger groups had more males, while older groups, most notably in the 51-60 range, were predominantly female.

### **Gender and Sleep Quality**
<img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/gender-sleep.png" alt="isolated" width="80%"/>

On average, females rated their sleep quality slightly higher than males. Women consistently scored one point higher at the 25th, 50th,and 75th percentiles. A Welch's t-test confirmed this difference, meaning it's unlikely due to chance. This suggests better sleep quality among females, aligning with trends from earlier research that found women tend to sleep slightly longer and have higher sleep efficiency than men.

### **Age and Sleep Quality**
<img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/age-sleep.png" alt="isolated" width="80%"/>

There was quite a bit of variability in sleep quality among the age groups. The 20-30 group had the lowest average, mostly between 6 and 7, while the 51-60 group clustered tightly around 9, indicating the best sleep quality compared to the other groups.A Spearman's rank coefficient of 0.42 shows a moderate positive link between age and sleep quality, suggesting improvement with age. However, this trend contradicts much existing research that has found an increase of sleep disturbances and decreased time spent in deep sleep with age. This highlights the need to investigate potential confounding factors such as the distribution of BMI or sleep durations among these age groups. 

### **Occupation and Sleep Quality**
<img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/occupation-sleep.png" alt="isolated" width="80%"/>

Sleep quality ratings varied across occupations in this dataset with engineers reporting the highest average ratings. Salespeople had the lowest ratings, followed by doctors, and nurses showed the highest variability in ratings among the seven occupations. Higher sleep quality could be linked to a more consistent work schedule while irregular work hours may contribute to lower ratings. Variability among ratings within certain occupations could be indicative of the diverse nature of their fields. It would be interesting to perform a further analysis on stress levels and physical activity between these occupations and how they play into reported sleep quality.

### **Sleep Duration, Stress Level, and Sleep Quality**

<p float="left">
  <img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/sleep-duration-quality.png" width="45%" />
  <img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/stress-sleep.png" width="45%" />
</p>

Sleep quality increases with sleep duration. Conversely, increased stress level correlates with reduced sleep quality. This suggests that an adequate amount of sleep and stress management strategies are essential for improving sleep quality. 

### **Sleep Disorders, BMI, and Sleep Quality**

<img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/bmi-disorder-proportions.png" alt="isolated" width="80%"/>

<img src="https://github.com/jasmineamjadi/sleep-analysis/blob/main/visualizations/bmi-disorder-sleep.png" alt="isolated" width="80%"/>

Overweight and obese individuals make up a large percentage of those with sleep apnea and insomnia. People without sleep disorders, particularly in the normal BMI range, report higher sleep quality. For sleep apnea, both healthy weight and obese individuals have a similar median sleep quality while overweight individuals report lower and more varied ratings. Insomnia shows lower sleep quality among overweight and obese individuals compared to those with a normal BMI, highlighting the link between BMI, sleep disorders, and reduced sleep quality. 

## References

1. Salfi F, Lauriola M, Tempesta D, Calanna P, Socci V, De Gennaro L, Ferrara M. Effects of Total and Partial Sleep Deprivation on Reflection Impulsivity and Risk-Taking in Deliberative Decision-Making. Nat Sci Sleep. 2020    May 27;12:309-324. doi: 10.2147/NSS.S250586. PMID: 32547280; PMCID: PMC7261660.
2. Neckelmann D, Mykletun A, Dahl AA. Chronic insomnia as a risk factor for developing anxiety and depression. Sleep. 2007 Jul;30(7):873-80. doi: 10.1093/sleep/30.7.873. PMID: 17682658; PMCID: PMC1978360.
3. Mansukhani MP, Covassin N, Somers VK. Apneic Sleep, Insufficient Sleep, and Hypertension. Hypertension. 2019 Apr;73(4):744-756. doi: 10.1161/HYPERTENSIONAHA.118.11780. PMID: 30776972; PMCID: PMC6513351.
4. Knutson KL. Impact of sleep and sleep loss on glucose homeostasis and appetite regulation. Sleep Med Clin. 2007 Jun;2(2):187-197. doi: 10.1016/j.jsmc.2007.03.004. PMID: 18516218; PMCID: PMC2084401.
5. Krishnan V, Collop NA. Gender differences in sleep disorders. Curr Opin Pulm Med. 2006 Nov;12(6):383-9. doi: 10.1097/01.mcp.0000245705.69440.6a. PMID: 17053485.
6. Ehlers C, Kupfer D. Slow-wave sleep: do young adult men and women age differently?. Journal of Sleep Research. 1997;6:211-215. doi: 10.1046/j.1365-2869.1997.00041.x.
7. Li J, Vitiello MV, Gooneratne NS. Sleep in Normal Aging. Sleep Med Clin. 2018 Mar;13(1):1-11. doi: 10.1016/j.jsmc.2017.09.001. Epub 2017 Nov 21. PMID: 29412976; PMCID: PMC5841578.

