Table of Content
================
* [Age Guess](#age-guess)
  * [Description](#description)
  * [Planning by day](#planning-by-day)
  * [Results](#results)
  * [Installation guide](#installation-guide)
  * [Credits](#credits)
  * [Licensing](#licensing)


# Age Guess

## Description
This is an age analysis project of some photographs in which some people are, these photographs are presented to the players, who must guess the age of the person at the time of the photograph.
In the project, five files are delivered that have different types of information about the participants, the photographs and the access to them, in addition a number of points is included for each of the people who try to guess the ages of the people.
The data analysis was done in a period of four days and that is why in the code to be presented it can be seen that each of the calculations carried out corresponds to a day that is duly marked with a title so that the sequence of the analysis is understood.

## Planning by day

1. Day 1 
Read the Document "The AgeGuess database, an open online resource on chronological and perceived ages of people aged 5–100" and Explore the data of the five files
2. Day 2 
Basic Analysis of the five files and basic Visualizations of the data
3. Day 3 
Searching Errors in the tables and building a new column to compare the Age Guessing to Real Age 
4. Day 4 
Join some of the tables to create queries and create Rankings by points, gender, country 

## Results
1. Day 1 
* Exploration of files: ag_gamers.csv, ag_guess.csv, ag_photos.csv, ag_report.csv, ag_quality.csv
* functions: shape, columns, dtypes, isnull().sum()  
* Graphs: Type of Gender(gamers), Type of Gender(photos), Distribution of Age (photos)    
2. Day 2 
* functions: value_counts, replace, groupby, sum, describe, query
* New columns: "qualiyty_category"(change number to categories), "outG_category"(absolute value of the out guess)   
* Graphs: Type of Quality(quality), Type of Ethnicity(gamers), Type of Ethnicity(photos), Measure of Difference with Real age(guess) 
Top 20 gamers by Total Points(gamers), Top 20 g by Total correct guess(gamers) 
3. Day 3 
* functions: query, round, value_counts
* New columns: "real age"(calculation of the age guess plus out of year guess), 
* Graphs: Real age vs Perceived age(guess), Histogram of Accuracy(guess), Histogram of Real Age(guess), Histogram of Real Age > 0(guess)
* Histogram of Guess Age > 0(guess), Measure of Difference with Real age(guess), Real Age == Guess Age(guess) 
4. Day 4 
* functions: query, merge, dtypes, isnull().sum(), .loc, .notnull(), .str.split(), fillna(). pd.cut()
* Merge tables: gamers+photos(uid), gamers+photos(uid), photos+guess(photo_id), 
* New columns: poss_age_gamer_in_moment, age_gamer_in_moment, year_in_moment, Ranking_by_Points(Total Points), Ranking_g(Gender), 
Ranking_C(Country), year_created, year_photo_uploaded  
* Graphs: Real Age == Distribution of Birth_year by Decades(gamers), Total New Gamers per Year(gamers), Total New Photos per Year(photos),
Birth decades by Gender(photos), Mean points by Country(gamers), Max points by Country(gamers), Performance by Countries(gamers)

## Installation guide

If you use conda, you can install: 

   * conda install pandas

   * conda install seaborn

   * conda install numpy

If you use pip, you can install: 

   * pip install pandas

   * pip install seaborn

   * pip install numpy

## Credits
The analysis of the database was carried out by Eliseo B.
the file is in notebook format "Age_Guess_Analysis.pynb"

The study was developed by a group of scientists and
the information of it is available at:
 * Review: SCIENTIFIC DATA
 * https://doi.org/10.1038/s41597-019-0245-9

## Licensing

GNU LESSER GENERAL PUBLIC LICENSE
                       
Version 2.1, February 1999

