# Documentation: Automating University Data Collection and Storage


### Introduction
This documentation outlines the process and functionality of a Python project developed to retrieve data about universities in a given country and city. The project utilizes the requests package to interact with an API, processes the obtained JSON data using the pandas library, and stores the processed data in an SQLite database. This documentation will guide you through the project's components, setup, and usage.


### Project Overview
The primary objective of the project is to automate the collection, transformation, and storage of university data for a specified country and city. The following steps are involved in achieving this:

-   Sending a request to the API to obtain university data in JSON format.
-   Parsing the JSON data into a pandas DataFrame for data manipulation.
-   Extracting relevant information from the DataFrame and exporting it.
-   Storing the extracted data into an SQLite database table.

### Setup
**Prerequisites**

Before using the project, ensure you have the following installed:

- Python 3.x
- Requests package (pip install requests)
- Pandas package (pip install pandas)
- SQLite3 package (usually comes with Python)

![Alt text](<Code Snippets/packages.png>)

### Files and Directory Structure
- **ETL-API-Call.ipynb:** The main Python script containing the code for the entire project.

- **universities.db:** The SQLite database file where the data will be stored.


## Project Usage
Follow these steps to use the project effectively:

1. **Open ETL-API-Call.ipynb:** This is the main script where all the project functionality is implemented.

2. **Input Parameters:** Modify the following parameters in the script according to your requirements:

- **API_URL:** The URL of the API to retrieve university data.
- **Country:** The name of the country for which you want to retrieve university data.
- **City:** The name of the city within the specified country.
- **Exported Coloumns:** A list of columns from the DataFrame that you want to export to the database.

![Alt text](<Code Snippets/extract.png>)

![Alt text](<Code Snippets/transform.png>)

![Alt text](<Code Snippets/load.png>)

![Alt text](<Code Snippets/call.png>)

The script will perform the following steps:

- Send a request to the API and retrieve data in JSON format.
- Parse the JSON data into a pandas DataFrame.
- Filter and transform the DataFrame as needed.
- Export the selected columns to an SQLite database table named uni_table.

**Check the Database:** After running the script, you should find a new SQLite database file named universities.db. This database contains a table named uni_table with the extracted university data.

## Conclusion
The Python project effectively automates the process of collecting university data for a specific country and city, processing it using pandas, and storing it in an SQLite database. This project streamlines the entire process, making it easier to obtain and manage university information for various purposes.

Feel free to customize the script further to meet your specific needs or integrate it into larger workflows as required. If you encounter any issues or need further assistance, refer to the code comments, and feel free to reach out for support.


**Source Code** - [Click here..](<Code Snippets/Code.pdf>)