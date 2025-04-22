Explore this data https://lite.datasette.io/?url=https%3A%2F%2Fraw.githubusercontent.com%2FSMUsamaShah%2FImdbParentsGuideSqlite%2Frefs%2Fheads%2Fmain%2Fimdb_parents_guide.sqlite#/imdb_parents_guide/imdb_pg

# ImdbParentsGuideSqlite
IMDB Parents Guide SQLite Database

Data taken from https://www.kaggle.com/datasets/barryhaworth/imdb-parental-guide

Contains data of movies with more than 1000 votes upto 16 January 2023 


# Convert CSV to SQLite
Source: https://stackoverflow.com/a/43786285/342095

```
$ sqlite3 newdbfilename.sqlite
sqlite>  .mode csv
sqlite>  .import yourdata.csv yourtable
sqlite>  .exit
```
