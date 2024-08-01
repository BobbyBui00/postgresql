## LEARN POSTGRESQL

postgres.exe -h <servername> -d <databasename> -U <username>

## PSQL COMMANDS

\d <table_name> 		: show table creation information
\d+ 				: get detailed information on a table
\dn 				: list schemas
\c <database_name> 		: switch database
\dt 				: list databases
\dt+ 				: get more information on tables in current database
\dt <schema>.* 			: list databases in specific schema
\i <path_to_sql> 		: import data into postgres
\l  				: display databases
\q 				: quit
\df 				: list all stored procedures
\df+ <function_name>		: show a stored procedure or a function code
\dv 				: list all views
\x				: show query output in the pretty format
\du				: list all users

SHOW search_path;
SET search_path TO <schema/database/>;

CREATE ROLE <role_name>;
CREATE ROLE <username> NOINHERIT LOGIN PASSWORD <password>;
SET ROLE <role_name>;
GRANT <role_1> TO <role_2>;
