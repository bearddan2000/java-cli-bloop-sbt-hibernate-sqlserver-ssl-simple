# java-cli-bloop-sbt-hibernate-sqlserver-ssl-simple

## Description
Creates a small database table
called `dog` and populates with
hql.

Sql server uses self-signed ssl.

Compiled and ran from build server `bloop`.

# Build note
Dependencies must be compatable with jdk8 or less.

## Tech stack
- bloop
- java
- bloop-sbt
  - hibernate
  - hql
  - log4j
  - sqlserver driver

## Docker stack
- alpine:edge
- hseeberger/scala-bloop-sbt:11.0.2-oraclelinux7_1.3.5_2.12.10
- mcr.microsoft.com/mssql/server:2017-latest-ubuntu

## To run
`sudo ./install.sh -u`

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- [HQL code based on](https://www.journaldev.com/2954/hibernate-query-language-hql-example-tutorial)
- [Hibernate config based on](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/An-example-hibernatecfgxml-for-MySQL-8-and-Hibernate-5)
- [Hibernate code based on](https://github.com/lokeshgupta1981/hibernate/tree/master/hibernate-hello-world)
