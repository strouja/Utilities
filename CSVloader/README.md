This provides IBM Db2 Event Store CSV loader wrapper, which will allow users to insert rows from a CSV file into a table on a Db2 Event Store system. 

Prerequisites:

The table and database must exist before execution.



Steps to running the csvloader . 

1. Download the csvloader wrapper script. 'csvloader' from Github <br />
  https://raw.githubusercontent.com/IBMProjectEventStore/Utilities/master/CSVloader/csvloader <br />
2. Download the csvloader jar from maven <br />
3. Run the csvloader wrapper script './csvloader' <br />
Required Arguments:  <br />
--user (The IBM Db2 Event Store User) <br />
--connstring (The connection string to connect to your IBM Db2 Event Store system where the syntax is: \"\<ip\>:\<port\>,\<ip\>:\<port\>,…\", i.e. one or more IPs with ports corresponding to you Event Store system) <br />
--filename (The name of the .csv file you want to load into your IBM Db2 Event Store table) <br />
--dbname (The name of the database that exists on your IBM Db2 Event Store system) <br />
--tablename (The name of the table that exists in the database used in --dbname) <br />

Example:  <br />
  ./csvloader --user admin --connstring localhost:5555 --filename example.csv --dbname TESTDB --tablename TEST_TABLE <br />
