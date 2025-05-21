# CrossFit Games Analysis

## The Situation
You've recently joined Maven CrossFit, a local CrossFit gym based in Boston.

## The Assignment
To prep for the upcoming CrossFit Games, you've decided to explore public data containing results and athlete information from the 2019 Games.
Your goal is to collect, clean and transform the raw data and produce extracts that your gym can analyze for competitive insights.

## The Objectives
1. Profile and QA the data
2. Transform the data
3. Clean and summarize the data for further analysis

## The Data Set

#### CrossFit Games
Scraped data on athletes and scores from the 2019 CrossFit Games, including information on each athlete's height, weight, affiliated gym, and nationality, as well as their overall rank and their performance on each workout.

#### Recommended Analysis
1. Which country do most athletes come from? Is it also the most successful country?
2. What is the age range of CrossFit competitors? At which age do they show peak performance?
3. Is any gym more successful than the rest?
4. How many workouts do the overall winners typically win?

#### Objective 1: Profile & QA the data
Your first objective is to explore and profile the data while optimizing it for visualization, including connecting to the data, removing null rows, eliminating duplicate fields, and exploring the fields/values.

* Connect to the three Excel workbooks and CSV file provided and take a moment to familiarize yourself with the file structure and metadata.
* Remove empty rows and identify field names from each input file.
* Remove the duplicative rank field from the 2019_games_scores file.
* Take a moment to explore and profile the data. Which country do most athletes come from? What’s the age range of CrossFit competitors?

#### Objective 2: Transform the data
Your second objective is to transform and shape the data into a usable format for analysis, including leveraging unions, joins, and field manipulation.

* Combine the 2019_games_athletes_men and 2019_games_athletes_women tables into a single view.
* Join the combined athletes table with the Country_Metadata table, keeping only records which match on country.
* Join the 2019_games_scores with the combined athletes table, and keep all score records regardless if they have a match.
* Remove the competitor_id field coming from the combined athletes table.

#### Objective 3: Clean and summarize the data
Your final objective is to clean and summarize the data by creating new fields to support your final analysis and aggregating data for final output.

* Create new fields for height (measured in inches) and weight (measured in pounds).
* Create a new field to calculate the number of minutes (as a numerical value) based on the existing time field.
* Aggregate the average weight (lbs), average height (ft), average age, and count of competitors by division and output the result as a local csv file.
* Aggregate the average points (lbs) and count of competitors by country of origin and output the result as a local xlxs file.

#### [Project Link]()