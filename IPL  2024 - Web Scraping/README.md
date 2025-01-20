# IPL 2024 Data Extraction, Cleaning, and Analysis

## Project Description
This project involves extracting match schedule and result details for the **IPL 2024** season from [ESPN Cricinfo](https://www.espncricinfo.com/series/indian-premier-league-2024-1410320/match-schedule-fixtures-and-results). The data is cleaned using **Power Query** and stored in a **MySQL database** for further analysis.

The project demonstrates web scraping, data cleaning, and database management using Python and other tools.

## Features
- **Web Scraping:** Extract match details such as teams, scores, results, and locations using Python.
- **Data Cleaning:** Perform transformations and ensure data accuracy using **Power Query**.
- **Database Integration:** Store cleaned data in a structured MySQL database for easy querying and analysis.

## Tools and Technologies

### Programming Language:
- Python

### Python Libraries:
- `bs4` (BeautifulSoup) - for web scraping
- `requests` - for fetching web pages
- `openpyxl` - for handling Excel files
- `mysql-connector-python` - for connecting to MySQL

### Data Cleaning:
- **Power Query** in Microsoft Excel or Power BI

### Database:
- **MySQL**

## Setup and Usage

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/ipl-2024-data.git
cd ipl-2024-data


### 2. Install Required Libraries
Ensure you have Python installed. Then, install the required libraries:
```bash
pip install beautifulsoup4 requests openpyxl mysql-connector-python
```

### 3. Web Scraping Script
Run the `scrape.py` script to fetch IPL 2024 match details:
```bash
python scrape.py
```
This will generate an Excel file named `ipl_2024_schedule.xlsx`.

### 4. Data Cleaning
- Open the `ipl_2024_schedule.xlsx` file in **Power Query** using Excel or Power BI.
- Perform cleaning tasks such as:
  - Removing duplicates
  - Standardizing date and time formats
  - Correcting team names, locations, and scores
- Export the cleaned data as a new Excel file (`ipl_2024_cleaned.xlsx`).

### 5. Upload to MySQL Database
Run the `upload_to_mysql.py` script to upload the cleaned data into your MySQL database:
```bash
python upload_to_mysql.py
```

## Database Schema
| Column Name    | Data Type       | Description                          |
|----------------|-----------------|--------------------------------------|
| `team_1`       | VARCHAR(100)    | Name of the first team               |
| `team_1_score` | INT             | Score of the first team              |
| `team_2`       | VARCHAR(100)    | Name of the second team              |
| `team_2_score` | INT             | Score of the second team             |
| `result`       | VARCHAR(200)    | Match result                         |
| `location`     | VARCHAR(150)    | Match location                       |

## Learning Outcomes
- How to scrape web data using Python libraries like `BeautifulSoup` and `requests`.
- Cleaning and transforming raw data into structured formats using Power Query.
- Storing and managing data in a MySQL database for analysis.
- Building a complete data pipeline for sports analytics projects.

## Future Enhancements
- Automating regular updates for match schedules and results.
- Integrating visualization tools like Power BI or Tableau for insights.
- Performing detailed statistical analysis on team performance and match trends.

## Acknowledgments
- Data Source: [ESPN Cricinfo](https://www.espncricinfo.com/series/indian-premier-league-2024-1410320/match-schedule-fixtures-and-results)
- Special thanks to the Python and data community for guidance.
```

