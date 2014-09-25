# Open Data ETL Tutorial

## Instructions

### Extract Data

Host Name: mysql.tomschenkjr.net
Database Name: etl_test_database
User Name: etl_tutorial
Password: ak9gos8dild9orc

Next, extract data from database, renaming the columns into a human-readable form.

```sql
SELECT statedata.St AS State, 
	   HSGrad AS HighSchoolGrad, 
	   Lon AS Longitude, 
	   Lat AS Latitude
FROM statedata, statecenter
```

### Installing MySQL Driver
If the test fails, install the [MySQL driver](http://dev.mysql.com/downloads/connector/j/). Move the .jar file to $PENTAHO_HOME/libext/JDBC

### Prepare Socrata environment

Visit [https://communities.socrata.com/catalog/chicago-etl/](https://communities.socrata.com/catalog/chicago-etl/) and create an account.
