# Rakenne

(means _structure_ in Finish)

Rakenne is a database modeling tool.

Its goal is:

* to provide a DSL for modeling database
  * to describe entity-relationship diagrams (ERD) using MERISE notation
  * to describe physical diagrams (PD)
* to provide a command-line tool for all operations
* to render models into diagrams
  * ERD to MERISE MCD diagrams
  * ERD to Chen notation diagrams
  * PD to MERISE MLD diagrams
* to validate model
* to convert across different database reprentations
  * to convert ERD to PD
  * to convert PD to database specific SQL
  * to reverse-engineer database-specific SQL to PD
  * to reverse-engineer PD to ERD
* to support multiple physical models
  * sql
  * nosql
* to support multiple SQL and NoSQL languages
  * SQL: postgresql
  * SQL: mariadb
  * NoSQL: redis
  * NoSQL: mongodb
  * NoSQL: cassandra CQL


## References

* https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model
* https://www.lucidchart.com/pages/er-diagrams
* https://www.youtube.com/watch?v=LR0Ip5Jenbk
