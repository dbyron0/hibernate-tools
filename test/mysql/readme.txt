The tests in this project will run when the 'all' profile is used and when the database is online.

The project was developed against the MySQL database running on localhost in a Docker container.

To do this on your own machine execute the following steps:

1. Install Docker.

2. Pull the Docker image of SQL Server: 'docker pull mysql'

3. Start the database: 'docker run -p3306:3306 --name MySql -e MYSQL_ROOT_PASSWORD=P@55w0rd -d mysql'. 

4. Connect to the database using your favorite client (e.g. DBeaver: http://dbeaver.jkiss.org)
hostname: localhost
port: 3306
username: root
password: P@55w0rd
The complete JDBC URL is: jdbc:mysql://localhost:3306

5. Create the 'HTT' schema. You can do this by executing the following SQL: 

create schema HTT;

6. You are now ready to run the tests. Use the following URL to connect: 'jdbc:mysql://localhost:3306/htt' 