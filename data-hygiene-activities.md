data-hygiene-activities
================
Rick Gilmore
2017-07-30 14:55:05

Data file formats
-----------------

-   Find a raw data file from your lab group that does *not* have identifiers. Describe how the file does or does not follow best practices. Describe the sequence of steps you would need to take to transform it into a file that followed these practices.

Naming conventions
------------------

Data directories
----------------

-   Describe the data directory/file organizational scheme for a project in your laboratory. What are the strengths and weaknesses of this organizational scheme for the workflows in your laboratory? How does the scheme reflect data collection? How does the scheme help or hinder data analysis or sharing?

Data dictionaries
-----------------

Take a data file from your lab group and produce a data dictionary that has the components recommended by ([Broman & Lee, 2017](https://github.com/kbroman/Paper_DataOrg/blob/master/manuscript.md#create-a-data-dictionary)): - The exact variable name as in the data file - A version of the variable name that might be used in data visualizations, e.g. a `short_name` - A longer explanation of what the variable means - The measurement units, e.g. cm or reaction time in milliseconds (ms). - Expected minimum and maximum values (if appropriate)

What name would you give this data dictionary and why? What format would it take and why?

Making data 'tidy'
------------------

-   Use the `dplyr::gather` function to make `untidy-wide-data.csv` tidy.
