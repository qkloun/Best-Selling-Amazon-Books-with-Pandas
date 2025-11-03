# Bestsellers Data Analysis

A Python data analysis project that cleans and analyzes book bestseller data, generating insights about top authors and genre ratings.

## Overview

This project processes a dataset of bestselling books to identify trends and patterns. It performs data cleaning, transformation, and aggregation to produce actionable insights about the most prolific authors and average ratings across different genres.

## Features

- **Data Cleaning**: Removes duplicate entries to ensure data integrity
- **Column Renaming**: Standardizes column names for better readability
- **Data Type Conversion**: Ensures price data is properly formatted as float
- **Author Analysis**: Identifies the top 10 most frequently appearing authors
- **Genre Analysis**: Calculates average user ratings by genre
- **CSV Export**: Automatically generates two output files with analysis results

## Requirements

```
pandas
```

Install dependencies using:
```
pip install pandas
```

## Usage

1. Ensure you have a `bestsellers.csv` file in the same directory as the script
2. Run the analysis script:
```
python analysis.py
```

3. The script will generate two CSV files:
   - `top_authors.csv` - Top 10 authors by number of bestselling books
   - `avg_rating_by_genre.csv` - Average user ratings grouped by genre

## Input Data Format

The input CSV file (`bestsellers.csv`) should contain the following columns:
- `Name` - Book title
- `Author` - Book author
- `Year` - Publication year
- `User Rating` - Rating score
- `Price` - Book price
- `Genre` - Book genre

## Output Files

### top_authors.csv
Contains the 10 authors with the most bestselling books in the dataset.

### avg_rating_by_genre.csv
Shows the average user rating for each genre, rounded to 2 decimal places.

## Data Transformations

The script performs the following transformations:
1. Removes duplicate records
2. Renames columns:
   - `Name` → `Title`
   - `Year` → `Publication Year`
   - `User Rating` → `Rating`
3. Converts `Price` column to float data type
4. Aggregates author frequency counts
5. Calculates mean ratings by genre

## License

This project is open source and available for educational purposes.

## Contributing

Feel free to fork this repository and submit pull requests for any improvements.
