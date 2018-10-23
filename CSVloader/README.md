Steps to running the csvloader . 

1. Download the csvloader wrapper script. 'csvloader' from Github <br />
  https://raw.githubusercontent.com/IBMProjectEventStore/Utilities/master/CSVloader/csvloader <br />
2. Download the csvloader jar from maven <br />
3. Run the csvloader wrapper script './csvloader' <br />
Required Arguments:  <br />
--user <DB2 Eventstore User> <br />
--connstring <Connection String to eventstore> <br />
--filename <CSV file> <br />
--dbname <DB2 Eventstore Database Name> <br />
--tablename <DB2 Eventstore Table Name> <br />

Example:  <br />
  ./csvloader --user admin --connstring localhost:5555 --filename example.csv --dbname TESTDB --tablename TEST_TABLE <br />
