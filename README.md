# Data modeling techniques - Example with Postgres

# Learning objectives
1. Apply [A database normalization technique](https://en.wikipedia.org/wiki/Database_normalization) for databases practice.
2. Apply [A star schema](https://en.wikipedia.org/wiki/Star_schema) for data warehousesing practice.
3. Apply best practices mentioned in [A Beginner’s Guide to Data Engineering](https://medium.com/@rchang/a-beginners-guide-to-data-engineering-part-ii-47c4e7cbda71) to the projetct.
4. Practice the usage of RDBMS database. We select `PostgresSQL` for this project.
5. Orchestrate the data pipeline with `airflow`
6. Make it reproduciable with `docker`

# Data
 The example data for this project is [Trending YouTube Video Statistics
Daily statistics for trending YouTube videos](https://www.kaggle.com/datasnaek/youtube-new?select=CA_category_id.json). You can find the brief information of the data set in the kaggle link itself. We select only the `CA` dataset for practicing in this project.

## Reasons
- Compatible sizing, and contains both `csv` and `json` formats.
- We can model the data for both `database` and `datawarehosue` purposes.
- The data contains different timestamp, which we can practice ingesting data with a different period.


