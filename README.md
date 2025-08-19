# NYC_Exams_Results_Analysis
Exploring NYC Public Schools Test Result scores

## Context
Every year american high-school students take SATs, an exam which measures
  - literacy: reading section
  - numeracy: math section
  - writing: writing section

**Each has a maximum score of 800**

This test are very important because the result defines the admission process. This analysis could mean very important information, for example parents would use it to have more information about the school performance. 

## Project Description
This project was taken from an online learning plataform called Datacamp. The main objetive is to demonstrate basic python skills, focusing on data analysis with pandas library.
Guiding questions are raised:
1. Which NYC schools have the best math results?
2. What are the top 10 performing schools based on the combined SAT scores?
3. Which single borough has the largest standard deviation in the combined SAT score?

## Data Origin and structure
The data was provided by DataCamp. It´s a csv file, with tabular structure. 

- Fuente: https://app.datacamp.com/learn/projects/exploring_nyc_public_school_test_result_scores/guided/Python
- Formato: CSV
 
 **_*Data Dictionary*_**

| Column Name                     | Data Type | Description                         |
|---------------------------------|-----------|-------------------------------------|
| school_name                     | string    | Name of the school                  |
| borough                         | string    | district or administrative unit     |
| builiding_code                  | sting     | building identifier                 |
| average_math                    | integer   | Average math score (0-800)          |
| average_reading                 | integer   | Average reading score (0-800)       |
| average_writing                 | integer   | Average writing score (0-800)       |
| percent_tested                  | float     | percentage of students tested       |

## Analysis objetives
Obtain insights about NYC public school SAT performance. There are three basic questions. The first one is about which are the schools that have the best math results. This same question could be made about the other results. This gives information about the best schools on each area, and which are the best scores ranges. The second question also looks for the bests schools, but this time combining the three SAT scores. It requires adding another column to the database, which has de summatory of the three scores. The third question answers which district has the largest standard deviation in the combined SAT score, grouping by borough. This value gives us an idea of which borough has the biggest dispersion, which implies boths schools with top results, and schools with low results.  


## Tools & How to Run

This project is designed to be run online, without any local installation.

- **Google Colab:**  
  You can open and run the analysis notebooks directly in your browser using [Google Colab](https://colab.research.google.com/).  
  [Open the main notebook in Colab](link-to-your-colab-notebook)

- **GitHub:**  
  All code and data are available in this repository. You can view notebooks and scripts directly on GitHub.

- **Python:**  
  The project is compatible with cloud-based Jupyter environments and GitHub Codespaces.

- **Pandas**

No need to install anything locally—just click and run!

## Key Findings

- Based on the analysis performed, the borough with the largest standard deviation in total SAT scores is Manhattan. The standard deviation for Manhattan is 230.29. This borough has 89 schools included in this calculation, with an average SAT score of 1340.13. This suggests that there is a greater spread or variability in total SAT scores among schools in Manhattan compared to other boroughs. In other words, there are schools with very high scores and schools with lower scores, leading to more diverse results in that borough.
- Based on the analysis, the top 10 schools by total SAT score are:

1. Stuyvesant High School (Total SAT: 2144)
2. Bronx High School of Science (Total SAT: 2041)
3. Staten Island Technical High School (Total SAT: 2041)
4. High School of American Studies at Lehman College (Total SAT: 2013)
5. Townsend Harris High School (Total SAT: 1981)
6. Queens High School for the Sciences at York College (Total SAT: 1947)
7. Bard High School Early College (Total SAT: 1914)
8. Brooklyn Technical High School (Total SAT: 1896)
9. Eleanor Roosevelt High School (Total SAT: 1889)
10. High School for Mathematics, Science, and Engineering at City College (Total SAT: 1889)

    These are the schools with the highest combined scores from the math, reading, and writing sections of the SAT.
 
- Based on the output from top_10_count_borough (Series that shows how many of the top 10 schools (by total SAT score) are located in each borough):

  According to this analysis, the distribution of the top 10 schools across boroughs is:

  Manhattan: 4 schools
  Bronx: 2 schools
  Queens: 2 schools
  Brooklyn: 1 school
  Staten Island: 1 school

  ![Pie Chart: Distribution of Top 10 Schools by Borough](images/top_10_schools_by_borough.png)

  *Figure: Distribution of Top 10 Schools by Borough.*
  
This indicates that Manhattan has the highest number of schools represented in the top 10 list based on total SAT scores in the dataset.

## Insights and conclusions
First, we could determinate with the top_10 schools which are the schools with the best SAT scores. Names like Stuyvesant High School or Bronx High School of Science stand out. Another conclusion we could take for this analysis is that the schools with top scores are not evenly distributed across the city. Manhattan has 40% of the top 10, followed by Bronx 20%. On the other hand, we have districts like Brooklyn which only has one. This suggests that there are district factor´s which could be associated to the high academic performance. Finally, The standard deviation analysis (largest_std_dev) shows that Manhattan not only has the highest number of schools in the top 10, but also the greatest variability in SAT scores among all its schools. This is an interesting insight: despite having many elite schools, there is also a wide range of scores within the borough. This could be due to greater diversity in the types of schools or student populations within Manhattan, or perhaps reflect significant differences in resources or educational approaches between schools in the same borough. Other boroughs may have lower average SAT scores, but perhaps a more homogeneous distribution of scores among their schools.


Fina
