### Description of the project
The aim of the following project is to calculate the overall crude and the age-standardized chronic obstructive pulmonary disease (COPD) death rates in both the United States and Uganda in 2019.

The crude death rate (CDR) is a demographic measure that represents the number of deaths occurring in a given population over a specific period, usually per 1,000 or 100,000 individuals.

The CDR is calculated as followed:

    CDR = (Number of deaths / Population) * multiplier

We will work with the multiplier 100000.

To calculate the overall age standardized crude death rate we will apply the average standardized population rates from 2000 to 2025.


### Installation instructions
The project was done with Jupyter notebook 6.5.4. using the Anaconda navigator

Python 3 was used for the project.

The following python libraries have been used in he project:
 - pandas
 - numpy
 - matplotlib


### Data sources
1. UN World Population Prospects (2022) — Population Estimates 1950-2021: WPP2022_POP_F01_1_POPULATION_SINGLE_AGE_BOTH_SEXES.xlsx
  https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/EXCEL_FILES/2_Population/WPP2022_POP_F01_1_POPULATION_SINGLE_AGE_BOTH_SEXES.xlsx
   
2. WHO Standard Population — Table 1 in 'Ahmad OB, Boschi-Pinto C, Lopez AD, Murray CJ, Lozano R, Inoue M (2001). Age standardization of rates: a new WHO standard.'
   https://cdn.who.int/media/docs/default-source/gho-documents/global-health-estimates/gpe_discussion_paper_series_paper31_2001_age_standardization_rates.pdf
  
3. A table of COPD death rates for the USA and Uganda in 2019 provided by the company Our World in Data
   https://owid.notion.site/Data-analysis-exercise-Our-World-in-Data-Junior-Data-Scientist-application-ab287a3c07264b4d91aadc436021b8c0


### Processing of Data Sources
All the CSV files imported and used in the COPD_Death_Rates.ipynb notebook are based on the data sources mentioned above.

1. The UN_Pop_estimates_USA_UGA_WORLD_2019.csv is based on estimates of the first sheet in the WPP2022_POP_F01_1_POPULATION_SINGLE_AGE_BOTH_SEXES.xlsx from the UN World Population Prospects. It contains     only the estimated population for Uganda, the US, and the World in 2019 from age 0 to 100+.
   
2. The WHO_World_Standard_Population_Distribution.csv contains a copy of the column "WHO World Standard" of the WHO Standard Population Table (Table 1) in 'Ahmad OB, Boschi-Pinto C, Lopez AD, Murray CJ,     Lozano R, Inoue M (2001). Age standardization of rates: a new WHO standard.'
  
3. The Age_specific_death_rates_COPD.csv contains a copy of the table called "Table of age-specific death rates of COPD"

The rest of the data processing is done in the COPD_Death_Rates.ipynb notebook.


### Code structure
Since the project is small there is only a folder called db containing all the data sources for the project. Furthermore there is the notebook COPD_Death_Rates.ipynb containing all the code linked to the analysis of the data, a file called LICENSE giving information of the license used, a README.md giving general and technical information on the project. 
``` bash
 ├── db
 │   ├── Age_specific_death_rates_COPD.csv
 │   ├── UN_Pop_estimates_USA_UGA_WORLD_2019.csv
 │   ├── WHO_World_Standard_Population_Distribution.csv
 ├── COPD_Death_Rates.ipynb
 ├── LICENSE
 └── README.md
```

### Results and evaluation
Overall COPD crude death rates: The total COPD crude death rate per 100,000 individuals for Uganda in 2019 is 5.8. The total COPD crude death rate per 100,000 individuals for the United States in 2019 is 57.2.

The high COPD crude death rate for the US compared to Uganda can be explained by the fact that the two countries have very different age distributions. In Uganda, there is a high percentage of young people that have a quite low COPD death rate. Older people generally have a higher death rate, and the US has a lot more older people than Uganda.

To be able to compare the results of the two countries more easily, we use the average standardized world population rates to get a similar age distribution for Uganda and the US. Applying these rates, we get: The overall COPD crude death rate per 100,000 individuals for Uganda is 28.7. The overall COPD crude death rate per 100,000 individuals for the United States is 28.4.


### Future work
For future research on COPD crude death rates, we could include some other countries and regions. For example, we could compare the US COPD death rates to those of European countries. Additionally, we could include more Sub-Saharan countries to compare the death rates with those of Uganda.


### License
MIT License
