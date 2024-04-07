# Continuity_of_absence Project


## Description
This Python script, written in Jupyter Notebook format, combines and cleans data from .xlsx files located in a specified raw data directory.


## Requirements
- Python 3.x
- Python libraries:
  - pandas
  - openpyxl
- os library
- glob library


## Key Functionalities
Combines rows: When consecutive rows share the same key values (Numer osobowy, Rodz. nieob./obecn.) and represent a contiguous period of time (Data do for the first row is one day before Data od of the second row), their data is combined into a single row.
![image](https://github.com/G-P-Rod/continuity_of_absence/assets/143654189/da956023-d928-4028-8287-29ca8ad58221)


Adds a 'Dokonano_złączenia' column: This column indicates whether a row has been combined with others.
Counts Changes: The script tracks the number of rows merged during the process. There may still be rows left to merge after the first loop. 
The loop will stop when the number of connected rows is zero.
![image](https://github.com/G-P-Rod/continuity_of_absence/assets/143654189/4c3c24e1-a7d2-40bb-8a32-241ee3e664df)


## File Structure
Source Data: .xlsx files are expected to be located in the data/raw directory.
Destination File: The combined and processed data is saved as combine.xlsx in the data/processed directory.

## Usage
Open the Jupyter Notebook file (main.ipynb).
Run the cells in sequential order.


## Output
The processed data is saved as combine.xlsx in the data/processed directory.


## Result:
The program informs us how many lines have been combined into one.

![image](https://github.com/G-P-Rod/continuity_of_absence/assets/143654189/cba47747-7098-4dfd-a2df-2daa42b00f70)

