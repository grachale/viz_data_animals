# Exploratory Data Analysis (EDA)

## Data
In the files `intakes.csv` and `outcomes.csv`, you will find data from an animal shelter in Austin, Texas, USA. The data is sourced from the official open data repository of the city of Austin.

The `intakes` dataset contains information about animals admitted from October 1, 2013, to April 27, 2022. The `outcomes` dataset includes information about animals that left the shelter (e.g., through adoption, return to owners) during the same time frame. Note that animals admitted before October 1, 2013, may not appear in `intakes.csv` (as data was not collected yet) but will have a record in `outcomes.csv` if they left the shelter after that date.

**Important:** The same animal may appear multiple times in each dataset. Some animals return to the shelter, and there may be duplicate records.

## Task
Use markdown cells for documentation. Explain all significant steps, describe visualizations, and discuss observations.

### ✨ Preparing data
1. Import necessary packages.
2. Load the `intakes` and `outcomes` datasets from the respective CSV files.
3. Familiarize yourself with both datasets, and comment on your findings (e.g., number of rows, number and meaning of features, data types, unique values).
4. Clean and convert the data:
   - Identify and handle missing values, replacing them with NaN if necessary.
   - Convert categorical features to the category type.
   - Convert the `Age upon Intake/Outcome` feature to a numerical type.
   - Convert the `DateTime` feature to `datetime64` type.
   - Perform any other meaningful data adjustments (e.g., conversions, removal of duplicate records, adding new features).

### Descriptive statistics
1. Comment on the selection of appropriate statistics for the given data type. Use visualizations whenever possible.
2. Describe the features `Age upon Intake` and `DateTime` (originally from the `intakes` dataset) using univariate descriptive statistics.
3. Select three additional features and describe them using appropriate univariate descriptive statistics.
4. Choose two features that might have a relationship (e.g., correlation) and describe this relationship using bivariate descriptive statistics. Pairs like `Age upon Intake` and `Age upon Outcome` are not accepted.

### ❓ Questions
Using suitable visualizations, answer the following questions:
1. Does the type of animal outcome depend on the type of intake? Simplify by considering only animals that appear exactly once in each dataset.
2. Does the age of the animal play a role in adoption?
3. Is the intake of animals constant throughout the year, or are there periods of higher/lower activity?

### ❓ Own questions
Create at least three custom questions and answer them with appropriate visualizations. You can base your questions on the mentioned datasets or use the `locations` dataset found in the `locations.csv` file. Feel free to explore additional interesting data related to this topic.

The `locations` dataset provides information about all stray cats and dogs in the shelter for less than a week. Most are in the shelter, but some are with volunteers, indicated in the `At AAC (AAC – Austin Animal Center)` column.
