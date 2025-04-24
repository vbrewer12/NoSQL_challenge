# Food Hygiene Ratings ETL & Analysis

## Project Overview
This project involves extracting, transforming, and analyzing food hygiene ratings from the **UK Food Standards Agency** using **MongoDB**. The goal is to clean, update, and analyze the data to identify trends and provide insights for food safety journalism.

## Technologies Used
- **MongoDB**: NoSQL database for data storage and queries
- **Python**: Data processing and analysis
- **Jupyter Notebook**: Interactive environment for ETL and analysis
- **Pandas**: Data manipulation and transformation
- **PyMongo**: MongoDB driver for Python

## Installation & Usage
### Prerequisites
- Python 
- MongoDB 
- Required Python Libraries:
  ```python
  import pymongo
  import pandas as pd
  import json
  from pprint import pprint
  ```

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/dagimg16/nosql-challenge.git
   ```
2. Navigate to the project directory:
   ```bash
   cd nosql-challenge
   ```
3. Install dependencies:
   ```bash
   pip install pymongo pandas
   ```
4. Import data into MongoDB:
   ```bash
   mongoimport --type json -d uk_food -c establishments --jsonArray --file resources/establishments.json
   ```
5. Run Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Project Scope
### Data Preparation & Cleaning
- **Importing Data**: Load raw food hygiene data into MongoDB.
- **Database Updates**:
  - Add a new restaurant entry.
  - Remove establishments in a specified region.
  - Standardize numerical fields.

### Data Analysis
- Identify establishments with the **worst hygiene scores**.
- Find **highly-rated restaurants**.
- Locate **top-rated establishments** near a specific location.
- Rank **local authorities** based on food safety compliance.

## Conclusion
This project demonstrates the power of **MongoDB and Python** in managing and analyzing food safety data. By structuring and cleaning the dataset, we provide valuable insights into food hygiene trends across the UK.

## Acknowledgments
  - Thanks to SMU and my instructors for guiding me through this learning journey!
  - And a big thank you to everyone checking out this project.

## License
  - Feel free to use and modify this script for your own learning.

