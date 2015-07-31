# GumGum Web Engineering - PHP Test
# Snippets

Inspired by http://codekata.com/kata/kata04-data-munging/

Exercise #1
-----------

Build a PHP app that does the following using [weather.dat](data/weather.dat)

- First run (or no database available):
 - Ask the user to upload the file, validate type and proceed
 - Mine the data: Day, Max Temp, Min Temp, Avg Temp
 - Dump the data in rows into a local sqlite database

- Routes:
 - All routes
  - The whole site stylesheet is affected by today avg temp"
   - If < 50F, cold/blue-ish theme
   - If 50F-80F, default/gray-ish theme
   - If > 80F, warm/yellow-ish theme
 - /
  - Shows today min/max/avg, prettier the better
 - /list
  - Shows a list of all the records, CRUD options
  - Here add as many routes you need for the CRUD operations
 - /report
  - Shows a chart with all the data by day
  - Shows a table (like /list)
  - Add filters like:
   - Min/Max temperature, which could apply to MinT,MaxT or AvgT
   - Table should show only the rows allowed by the filter
   - Chart should indicate however you want the filtered data

Assume PHP error reporting enabled with E_ALL.
