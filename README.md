**eBay Men's Perfume Data Analysis**

**Project Overview**

This project explores an eBay men's perfume listings dataset using Python, Pandas, NumPy, and Matplotlib.

The objective is to understand the dataset, examine perfume listing prices, compare brands, identify data quality issues, and visualize key patterns through charts.

**Project Objectives**

Explore the dataset's structure and data types.

Analyze missing values and duplicate records.

Examine perfume price distributions and summary statistics.

Identify the highest-priced and lowest-priced listings.

Compare brands using average, minimum, and maximum prices.

Calculate brand-wise listing counts and total listed prices.

Create charts to communicate findings clearly.

**Dataset Description**

Dataset: eBay Men's Perfume Listings

Records: 1,000 rows

Columns: 10

**The dataset contains the following columns:**

Column

Description

brand

Perfume brand name

title

Product listing title

type

Perfume or fragrance type

price

Numeric listing price

priceWithCurrency

Price displayed with currency information

available

Available quantity, where provided

availableText

Listing availability and sales text

sold

Sold count, where provided

lastUpdated

Listing update information

itemLocation

Listing location

**Tools and Technologies**

Python

Jupyter Notebook

NumPy

Pandas

Matplotlib

**Project Workflow**

**1. Data Loading**

Imported the CSV dataset using pandas.read_csv().

Loaded the dataset into a Pandas DataFrame.

**2. Data Exploration**

Used the following operations to understand the dataset:

shape

columns

info()

head()

describe()

unique()

nunique()

value_counts()

**3. Data Quality Checks**

Checked missing values in each column using isnull().sum().

Calculated missing-value percentages.

Counted exact duplicate rows using duplicated().

Identified repeated product titles and examined matching records.

Note: These checks identify data quality issues. Missing values and repeated titles were not systematically cleaned or removed in the current notebook.

**4. Price Analysis**

Calculated mean, median, minimum, maximum, and other descriptive statistics.

Identified the top 10 highest-priced listings.

Identified the lowest-priced listings.

Compared average prices across brands.

**5. Brand-Wise Analysis**

Used groupby() and agg() to calculate:

Average listing price

Minimum listing price

Maximum listing price

Listing count

Total listed price

Also sorted and filtered brands to compare their listing activity and price patterns.

**6. Data Visualization**

Created the following visualizations using Matplotlib:

Bar Chart: Top 10 brands by listing count.

Pie Chart: Distribution of listings among the top 5 brands.

**Key Findings**

Based on the current notebook outputs:

Giorgio Armani has 60 listings, the highest count among the brands shown in the top 10 listing-count results.

Paco Rabanne has 45 listings.

Ralph Lauren has 41 listings.

The average listing price is approximately 46.48 in the dataset's price units.

The median listing price is 35.71.

The minimum listed price is 3.00.

The maximum listed price is 259.09.

The dataset contains 177 missing cells.

No exact duplicate rows were found, although 34 repeated titles were identified by the title-based duplicate check.

**Important Limitations**

The dataset contains missing values that require further investigation.

Repeated titles do not necessarily mean that two listings are identical.

Brand names may contain spelling or capitalization variations.

The sum of listing prices does not represent actual revenue or profit.

The relationship between price and sold count has not yet been analyzed in the current notebook.

Results describe the provided dataset and may not represent all eBay perfume listings.
