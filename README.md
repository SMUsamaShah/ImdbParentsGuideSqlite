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
