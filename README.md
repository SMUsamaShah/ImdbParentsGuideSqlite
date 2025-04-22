Explore this data https://lite.datasette.io/?url=https%3A%2F%2Fraw.githubusercontent.com%2FSMUsamaShah%2FImdbParentsGuideSqlite%2Frefs%2Fheads%2Fmain%2Fimdb_parents_guide.sqlite#/imdb_parents_guide/imdb_pg

All safe animated movies for a kid:

https://lite.datasette.io/?url=https%3A%2F%2Fraw.githubusercontent.com%2FSMUsamaShah%2FImdbParentsGuideSqlite%2Frefs%2Fheads%2Fmain%2Fimdb_parents_guide.sqlite#/imdb_parents_guide?sql=select+%27https%3A%2F%2Fwww.imdb.com%2Ftitle%2F%27+%7C%7C+tconst+%7C%7C+%27%2F%27+AS+imdb_url%2C+titleType%2C+primaryTitle%2C+startYear%2C+runtimeMinutes%2C+genres%2C+averageRating%2C+numVotes%2C+sex%2C+violence%2C+profanity%2C+drugs%2C+intense+from+imdb_pg+where+%22isAdult%22+%3D+0+and+%28%22sex%22+%3D+%22None%22+or+%22sex%22+%3D+%22%22%29+and+%28%22violence%22+%3D+%22None%22+or+%22violence%22+%3D+%22%22%29+and+%28%22drugs%22+%3D+%22None%22+or+%22drugs%22+%3D+%22%22%29+and+%28%22profanity%22+%3D+%22None%22+or+%22profanity%22+%3D+%22%22%29+and+titleType+LIKE+%27%25movie%25%27+and+runtimeMinutes+%3E+60+and+numVotes+%3E+3000+and+%22genres%22+LIKE+%27%25anim%25%27+order+by+averageRating+desc&_hide_sql=1

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
