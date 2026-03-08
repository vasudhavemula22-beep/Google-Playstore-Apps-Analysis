
Google Play Store Data Analysis
 Project Overview

This project involves the Exploratory Data Analysis (EDA) of the Google Play Store apps dataset using Python and the Pandas library. The goal is to analyze various metrics such as app ratings, reviews, categories, and installation numbers to derive meaningful insights about the app market.

 Technologies Used:

Python 3.x

Pandas (Data manipulation and analysis)

 Dataset:

The dataset used for this analysis is included in this repository (googleplaystore.csv).

Source: Google Play Store

Content: Contains ~10,800 rows with details on App Ratings, Reviews, Size, Installs, and Pricing.


 Important Configuration (Before Running):

The Python script currently contains a specific file path pointing to a local directory:

data = pd.read_csv(r"D:/vasudha datasets and projects/google_playstore/googleplaystore.csv")

You must update this line before running the code:

Download the googleplaystore.csv file from this repository.

Open the Python script.

Change the path inside pd.read_csv("...") to the location where you saved the CSV file on your own computer.


 Key Analysis & Insights:

The script performs the following specific operations:

1. Data Exploration

Displays the first 5 and last 3 rows of the dataset.

Calculates the shape (number of rows and columns).

Provides technical summaries (info()) and statistical summaries (describe()).

2. Analytical Questions Answered

Astrology Apps: Counts how many apps contain "Astrology" in their title.

Average Rating: Calculates the mean rating across all apps.

Unique Categories: Counts the total number of unique app categories.

Best Categories: Identifies which app category has the highest average rating.

5-Star Apps: Counts the number of apps that have a perfect 5.0 rating.

Free vs. Paid: Counts the distribution of Free vs. Paid applications.

3. Data Cleaning & Advanced Analysis
   

Review Analysis:

Converts the Reviews column to a numeric data type (handling specific formatting issues like '3.0M').

Calculates the average number of reviews.

Identifies the app with the maximum number of reviews.

Lists the Top 5 apps with the highest reviews.

Rating by Type: Compares the average rating of Free apps vs. Paid apps.


Installation Analysis:

Cleans the Installs column by removing characters (,, +) and handling corrupt data ('Free').

Converts Installs to integer type.

Identifies the Top 5 apps with the maximum number of installations.


 How to Run

Install Dependencies:
Ensure you have pandas installed:

pip install pandas

Update Path:
As mentioned in the configuration section, update the read_csv path in the code.

Run the Script:
Execute the Python file in your preferred environment (Jupyter Notebook, VS Code, PyCharm, or Spyder).

