# SQL Wars: Comparing Relational Databases

## Introduction
Coming from a computational science/applied mathematics background many of the ideas of data science/machine learning are second nature to me. One thing that was very new to me was creating and manipulating databases. In computational science we don't really deal with databases and I/O is something to avoid as much as possible because it limits performance. Therefore, in this blog post I'll be going what I have learend about SQL databases, i.e. what they are, how to set them up, and how to use them.

### SQL And What I'll Cover:
SQL stands for Structured Query Language. It is a domain specific language used in programming to deal with data that is stored in a relational database. SQL is designed for a specific purpose: to query data contained in a relational database. There are plently of good references on how to learn SQL query commands, two that I used are,

1. <a href="http://sqlzoo.net/">SQLZOO</a>
2. <a href="https://www.w3schools.com/sql/">w3schools.com</a>

However, this is not what I intend to cover here.  Instead, I would like to look at how one can create and interact with different implementations of SQL databases.  And specifically how to do this using Python.  There are many different implementations of SQL: SQLite, Oracle, MySQL, PostgreSQL, etc.  The basic operations on SQL databases that are common to all the implementations are described in the acronym, C.R.U.D.:

- **C**reate: How to create a database and tables.
- **R**ead: How read from a table in a database.
- **U**pdate: How to update the values in a table in the database.
- **D**elete: How to delete rows from a table in the database.


For now the SQL implementations I'll be focusing on are,

* <a href="https://www.sqlite.org/">SQLite</a> and Python's interface to it <a href="https://docs.python.org/2/library/sqlite3.html">sqlite3</a>.

and 

* <a href="https://www.postgresql.org/">PostgreSQL</a> and Python's interface to it <a href="https://www.sqlalchemy.org/">sqlalchemy</a> and <a href="http://initd.org/psycopg/">psycopg2</a>.

As we'll see most of the differences between working with the two implementations will be in how we create the databases.  The queries will be relatively the same, but the libaries we use to interact with the databases will be different depending on the SQL implementation. I'll be updating this blog post as a time goes on, so check back later for new additions.

## Requirements
1. <a href="https://www.python.org/"> Python</a> 2.7
2. <a href="http://jupyter.org/">Jupyter Notebook</a>
3. <a href="https://www.sqlalchemy.org/">SQLAlchemy</a>
4. <a href="https://sqlalchemy-utils.readthedocs.io/en/latest/">SQLAlchemy-Utils</a>
5. <a href="http://initd.org/psycopg/">psycopg2</a>

To install the requirements with pip (except for Python), type in the main directory:

<code> pip install -r requirements.txt </code>
