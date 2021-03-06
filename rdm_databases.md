<style>
.footer {
    color: #434343;
    background: #ffffffff;
    position: fixed;
    top: 90%;
    text-align: left;
    width: 100%;
}
.header {
    color: black;
    background: #E8E8E8;
    position: fixed;
    bottom: 90%;
    text-align:center;
    width:100%;
}
.small-code pre code {
  font-size: 0.9em;
}
</style>

databases
========================================================
author: 
autosize: true
font-family: 'Arial'

terminology
========================================================

* A database (DB) is an organized collection of data
* A database management system (DBMS) is a software that allows interacting with the database (e.g., storing, retrieving, updating data)

<div class="footer" style=font-size:50%;">Attribution: Introduction to Data Science: BIO 260 and CSCI E107, Harvard T.H. Chan School of Public Health</div>


relational database
========================================================
* Many types/flavors of databases: document, key-value
* Relational model (RM):
  + built atop a set-theory branch called relational algebra: a combination of selections ( WHERE ... ), projections ( SELECT ... ), Cartesian products ( JOIN ... ), and more
* RDBMS = DBMS + RM
* SQL (Structured Query Language): language designed to interact with RDBMS

<div class="footer" style=font-size:50%;">Attribution: Introduction to Data Science: BIO 260 and CSCI E107, Harvard T.H. Chan School of Public Health</div>


why use a RDBMS?
========================================================

* Data size, typically when the data fits on drive but not in memory
* One DB vs (too) many CSV files - **complexity!**
* Harness the power of SQL
* Data already live in a DB
* DB provides extra tools, for example a GIS toolbox to deal with spatial data

<div class="footer" style=font-size:50%;">attribution: introduction to data science: bio 260 and csci e107, harvard t.h. chan school of public health</div>


RDBMS software solutions
========================================================

* commercial
  + Oracle
  + Microsoft SQL Server
  + ...
* open-source
  + MySQL
  + PostgreSQL
  + SQLite
  + ...
  
<div class="footer" style=font-size:50%;">attribution: introduction to data science: bio 260 and csci e107, harvard t.h. chan school of public health</div>

  
SQLite
========================================================
  
* SQLite is the easiest way to start: unlike others, it is not a client-server DB. The whole DB can live in a (portable) folder. All the required tools are included in dplyr.
* Light but still powerful. It barely requires configuration but can still store and process large amounts of data. It is used in most web browsers and mail clients.

<div class="footer" style=font-size:50%;">attribution: introduction to data science: bio 260 and csci e107, harvard t.h. chan school of public health</div>

Structure
========================================================
title: false

table structure
<p style="font-size:0.5em; color:grey;"><img src="./images/tableStructure.png" style="margin-bottom=10px"><br>attribution: introduction to data science: BIO 260 and CSCI E107 Harvard T.H. Chan School of Public Health</p>
***
database structure (schema)
<p style="font-size:0.5em; color:grey;"><img src="./images/entity-relationship-diagram.png" style="margin-bottom=10px"><br>attribution: Hand-crafted relational databases for fun and science, Naupaka Zimmerman, Data Carpentry, 2016-12-05</p>
