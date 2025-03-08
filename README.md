# GitHub Most Popular Repos - Data Engineering Project

## Project Overview

This project focuses on extracting, transforming, and loading (ETL) data from JSON files containing information about the top-starred GitHub repositories. The goal is to analyze these repositories based on programming languages, organization accounts, and search term relevance, then store the results in a PostgreSQL database using Apache Spark.

## Data Source

We were provided with 30 JSON files [Source Data](https://www.kaggle.com/datasets/anshulmehtakaggl/top-1000-github-repositories-for-multiple-domains?select=Spark.json), each containing repositories matching different search terms.These files include details such as:


(![These files include details such as: ](https://github.com/user-attachments/assets/534b2d42-9b90-43ed-a237-f9a39b493d93)
)

## Key Objectives

Create a table for programming languages (programming_lang)

Stores the count of repositories using each programming language.

Create a table for organization-type accounts (organizations_stars)

Stores the total number of stars received by repositories belonging to each organization.

Create a table for search terms (search_terms_relevance)

Stores the relevance score for each search term, calculated using:



## Technologies Used

Apache Spark (for data processing)

PostgreSQL (for data storage)

Google Colab (for running the notebook)

PySpark (for Spark operations)

## ----------------------------------------------------------------------------------------
## Implementation

 ### 1️)Extract Data

The JSON files were loaded into a Spark DataFrame.

 ### 2️)Transform Data

Programming Languages Table (programming_lang)

Organizations Stars Table (organizations_stars****)

Search Terms Relevance Table (search_terms_relevance****)

 ### 3️)Load Data into PostgreSQL

We installed PostgreSQL on Google Colab and wrote the transformed DataFrames into three separate tables.

### 4️)Read Data from PostgreSQL

To verify the data was loaded correctly, we read the tables back into Spark.

## -----------------------------------------------------------------------------------------------

## Results & Insights

Identified the most popular programming languages based on GitHub repository counts.

Calculated which organizations have the most stars across their repositories.

Determined the most relevant search terms based on our custom relevance formula.

