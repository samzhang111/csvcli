# Extremely simple command line CSV tools (using basic unix tools)

Some tools that wrap basic unix tools for stream filtering CSV files.

This is not meant as a replacement for a package like csvkit. Rather, it allows a simple stream filter based approach using linux tools existing on most computers.

* `csv-cat <csv1> [csv2 [csv3 ...]]`: concatenates csv files. Like `cat`, except it excludes the first line (assumed to be a csv header) on all files except the first one.
* `csv-dedup <csv-file>`: performs sort | uniq on a csv file, keeping the header in place.
* `csv <csv-file>`: opens an ipython terminal with the csv file loaded as a dataframe in the variable `df`, printing out the head of the dataframe showing up to 50 columns. (Requires ipython to be installed and available on the path)
