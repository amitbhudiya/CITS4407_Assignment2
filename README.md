# CITS4407_Assignment2
## Board Games Data Analysis Suite
This project consists of three shell scripts that process and analyze board game data from BoardGameGeek:

1. `empty_cells` - Identifies empty cells in each column
2. `preprocess` - Cleans the data
3. `analysis` - Analyzes the cleaned data to answer research questions

### Script Details
### empty_cells
**Usage:** `./empty_cells <filename> <separator>`

This script analyzes a CSV/TSV file to find the number of empty cells in each column. It takes two arguments:

- `filename:` The input data file to analyze
- `separator`: The character used as a separator in the file (e.g., ';', or ','  or '\t')

**Output:** A list of column names and the number of empty cells found in each column.

### preprocess
**Usage:** `./preprocess <input_file>`

This script cleans the input data file by:

- Converting semicolon separators to tab characters
- Converting DOS/Windows line endings to Unix line endings
- Changing decimal commas to decimal points
- Removing non-ASCII characters
- Generating new IDs for rows with empty ID fields

**Output:** The cleaned data is written to standard output and can be redirected to a file.

### analysis
**Usage:** `./analysis <cleaned_input_file>`

This script analyzes the cleaned data to answer four research questions:

- What is the most popular game mechanics?
- What is the most popular game domain?
- What is the correlation between publication year and average rating?
- What is the correlation between game complexity and average rating?

**Output:** The answers to the research questions.
