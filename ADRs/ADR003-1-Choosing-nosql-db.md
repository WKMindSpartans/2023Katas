# Architectural Decision Record
## Date
9/13/23 

## Title
Choosing the right NoSQL DB

## Status
Accepted

## Context

No SQL Databases offer high flexibility in schema and scale. Hence NoSQL is a better choice over traditional SQL databases.

NoSQL databases are classified into 4 types.

* Document stores
* Graph databases
* Key-value store 
* Wide column store

credits : https://www.researchgate.net/figure/CAP-theorem-with-databases-that-choose-CA-CP-and-AP_fig1_282519669

## Decision

- As there would be too many writes, a document-based store would be a better choice. 
- the document data stores offer data partitioning, which would help as the platform expands toward different regions.
- Key-value store would be helpful in use cases of caches, where aggregate queries are not required.
