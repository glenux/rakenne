
# <img src="doc/logo-display-only.svg" width="50%" style="display: block; margin: 0 auto;" alt="Rakenne" />

Rakenne is a database modeling tool for command line written in Crystal.

For now, It is a toy project to improve author's skills with the language and its various libraries. **It is not supposed to work (yet). Please don't use it in production.** :warning:

Note: _rakenne_ means _structure_ in Finnish.

## Roadmap

* provide a DSL for modeling database
  * describe entity-relationship diagrams (ERD) using MERISE notation
  * describe physical diagrams (PD)
* provide a command-line tool for all operations
* render models into diagrams
  * ERD to MERISE MCD diagrams
  * ERD to Chen notation diagrams
  * PD to MERISE MLD diagrams
* validate model
* convert across different database reprentations
  * to convert ERD to PD
  * to convert PD to database specific SQL
  * to reverse-engineer database-specific SQL to PD
  * to reverse-engineer PD to ERD
* support multiple physical models
  * sql
  * nosql
* support multiple SQL and NoSQL languages
  * SQL: postgresql
  * SQL: mariadb
  * NoSQL: redis
  * NoSQL: mongodb
  * NoSQL: cassandra CQL


## References

* https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model
* https://www.lucidchart.com/pages/er-diagrams
* https://www.youtube.com/watch?v=LR0Ip5Jenbk
