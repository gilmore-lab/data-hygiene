data-hygiene
================
Rick Gilmore
2017-07-30 14:15:44

Goals
-----

1.  Reduce time spent on data cleaning/munging.
2.  Produce 'tidy' data sets that can be easily updated, shared, re-used.

Best practices
--------------

### Data file formats

-   Store and save data files as text, preferably in comma-separated value (CSV) format.

<!-- -->

    variable_1,"variable 2",variable_3,variable_4
    1, "A",TRUE,2017-07-04
    2, "Z",FALSE,2017-07-04

*Note*: First row contains variable/column names. There are no spaces between variables. Each row of the data file ends with an (invisible) line feed/return character. If your variable name has spaces in it, you must surround the name with quotation marks, e.g., `"variable 2"`.

-   Save data files in the rawest, most 'micro' state possible
    -   trial-by-trial, response-by-response
    -   separate files for each participant & measure
-   Write scripts/syntax to aggregate files across participants & measures

-   Adopt a 'tidy' data ([Wickham, 2014](http://dx.doi.org/10.18637/jss.v059.i10)) format
    -   Each row is an observation
    -   Each column is a variable
    -   Files are 'rectangular'
    -   Each cell is filled, even with `NA` if needed.
-   Avoid spaces in file names (& variable names); use hyphens "-" or underscores "\_" to make file names human readable.
    -   This makes file names "parsable"
    -   If important metadata (e.g., participant ID, condition, or test date) aren't in the file, put them in the file name: `<participant-id>-<YYYY-MM-DD>-condA.csv`
-   When using dates, use the YYYY-MM-DD format.

### Data directories

-
