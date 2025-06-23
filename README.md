# Task---1-Data-cleaning-and-preprocessing

Identified and handled missing values using isnull() in Python.

Removed duplicate rows using drop duplicates().

Standardized text values like country names, etc.

Converted date formats to a consistent type (e.g., dd-mm-yyyy).

Renamed column headers to be clean and uniform (e.g., lowercase, no spaces).

Checked and fixed data types (e.g., age should be int, date as datetime).

CODE EXPLANATION! 

* Imports the `pandas` library, which is used for data manipulation and analysis.

---

* Loads the dataset from a specific path on your computer.

---

* Removes any completely duplicate rows from the dataset.
* Prints a confirmation message.

---

* Displays the count of missing values in each column.

---


* Removes entire columns that contain **any** missing values.
* `axis=1` targets columns, and `inplace=True` modifies the dataframe directly.

---

* Checks if the column `'COUNTRY'` exists.
* Converts all values in that column to lowercase and strips leading/trailing whitespace (for consistency).

---

* Converts the `'ORDERDATE'` column to proper `datetime` format.
* Invalid date entries are turned into `NaT` (`Not a Time`) using `errors='coerce'`.

---

* Changes all column names to lowercase.
* Replaces spaces with underscores to make column names easier to work with programmatically.

---

* Prints the data types of each column after all transformations.

---

* Saves the cleaned dataset to a new CSV file named `cleaned_data.csv` in the current working directory.
* `index=False` prevents the row index from being written to the file.

---

* Confirms the completion of the preprocessing steps.
