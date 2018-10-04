# Technical Assessment Level 1
This is a draft technical assessment for analyst and associate candidates.
The exercises involve using APIs, command line tools, and Excel to download and manipulate data.

Upon completion of the following exercises, email the files below to [training@sagenceconsulting.com](mailto:training@sagenceconsulting.com).
```bash
salaries.sh
ANSWERS.txt
salaries_analysis.xlsx
```

## Data

For these exercises, we will use the Chicago city salaries file.
You can check out information about the data on the [Chicago Data Portal](https://data.cityofchicago.org/Administration-Finance/Current-Employee-Names-Salaries-and-Position-Title/xzkq-xp2w).

To get the complete salaries data, we recommend using this endpoint:
```
https://data.cityofchicago.org/api/views/xzkq-xp2w/rows.csv
```

## Exercises

### Command Line
For the following exercises, store code in shell script called `salaries.sh`.
1. Use the Chicago Data Portal API endpoint to download a CSV file of the salaries using `curl`. Save the data to a file called `salaries.csv`.
2. Using your converted CSV file, write shell scripts to `salaries.sh` in order to answer the following questions:
  * How many paid employees does City of Chicago have?
  * How many salaried employees are there?
  * How many hourly employees are there?
3. Store answers to Q2 in a file called `ANSWERS.txt`.

### Excel
There have been some updates to the salary information because some employees received a raise. The updated salaries for each employee are stored in a GitHub repository. Download the new salaries data from the repository [here](https://github.com/ratulesrar3/assessment_level_one).

4. Merge the new salaries with the salaries data downloaded via the API.
5. Using the merged dataset, answer the following questions:
  * What department has the most employees?
  * Which departments have the highest average salaries?
  * What is the average salary for Chicago police officer?
6. Use an in-line formula to split the names into first names, last names, and middle initials. Then answer the following questions:
  * What is the most common last name?
  * What percentage of employees have no middle initial?
7. Write a simple macro to create a new sheet with only police and fire department employees. How many emergency responders does the city employ?
8. Save your edited spreadsheet as a file called `salaries_analysis.xlsx`.
