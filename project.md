# GumGum Web Engineering - PHP Test
# Snippets

Inspired by http://codekata.com/kata/kata04-data-munging/

Exercise #1 - English Weather App
---------------------------------

In [weather.dat](data/weather.dat) you’ll find daily weather data for the UK in
June 2001.
Build a PHP app that does the following using it:

- First run (or no database available):
  - Ask the user to upload the file, validate and proceed.
  - Build a local sqlite table from it.

- Routes:
  - /
    - Shows **today** min/max/avg, prettier the better.
  - /list
    - Shows a list of all the records, CRUD options.
    - Here add as many routes you need for the CRUD operations.
  - /report
    - Shows a by-day chart with all the data.
    - Shows the same table from /list without CRUD options, sortable is a plus
    - Add filters:
      - Min/Max avg. temperature
      - Table should show/hide rows according to this filter
      - Chart should respond to the filter as well, freedom to choose how.
  - /upload
    - Reupload the data, recreating everything from it.
  - On all routes the whole app style is affected by **today** avg temp:
      - If < 50F, cold/blue-ish colors
      - If 50F-80F, default/gray-ish colors
      - If > 80F, warm/yellow-ish colors

*"Today" means using the day from the actual server date*
*Assume PHP error reporting enabled with E_ALL.*
*Validations are important*


Exercise #2 - English Soccer API
--------------------------------

The file [soccer.dat](data/soccer.dat) contains the results from the English
Premier League for 2001/1.

The columns labeled ‘F’ and ‘A’ contain the total number of goals scored for and
against each team in that season (so Arsenal scored 79 goals against opponents,
and had 36 goals scored against them).

The column labeled LGD is the Last Game Day. Just keep it in mind.

Write an RESTful API that is capable of:
- Upload the file and build a local sqlite table from it.
- List all results
  - Query params: filters (at least 2), sortable, output format
- CRUD operations on each entry Name field.
- /top Outputs each team and their goal difference, in DESC order by the later

*Must work with calls from any domain*
*Front end is a plus*
*JSON ouput is required, HTML is a plus*


Exercise #3 - Refactoring
-------------------------

Take the two programs written previously and factor out as much common code as
possible, leaving you with two smaller programs using shared COMPOSER components

And add an option to the API:
- /restless
  - Shows a list of all the teams that last game was on 75 F Avg or more
