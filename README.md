# SQL Server

    docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Password!' --network sbe16 -p 1433:1433 -d mcr.microsoft.com/mssql/server:2017-CU8-ubuntu

## Access the database

    docker exec -it <containerID> bash  

## SQLcmd

    /opt/mssql-tools/bin/sqlcmd -S localhost -U SA -P "Password!"

    1> CREATE DATABASE TestDB
    2> GO
    1> SELECT Name from sys.Databases
    2> GO

    CREATE TABLE ctd_sbe16plus_data (instrument_id VARCHAR(5),time DATETIME,cond FLOAT,press FLOAT,sal FLOAT,soundv FLOAT,temp FLOAT,dissolved_oxygen_ppm FLOAT,dissolved_oxygen_sat FLOAT,ttime DATETIME,created DATETIME,modified DATETIME,crby VARCHAR(50),modby VARCHAR(50))
    GO

