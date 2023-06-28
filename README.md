# berkeley-db-cpp-framework
C++ framework to improve Berkeley DB developer efficiency and reduce programming errors.

# Table of Contents
- [Background](#background)
    - [The purpose of Databases](#database-purpose)
    - [Advantages of Berekley DB](#berekley-db-advantages)
    - [Berekley DB resources](#berekley-db-resources)

## Background
[Oracle Berkeley DB](https://www.oracle.com/database/technologies/related/berkeleydb.html)  provides highly efficient 
storing, managaging, and accessing of large sets of data.  


The ` berkeley-db-cpp-framework` are C++ classes and functions created to 
hide some of the complexity of using Berkeley DB.
Berkeley DB is simpler and requires less resources than common Relational Database 
Systems (RDBMS) such as that provided by Oracle.
As a result, it is much faster and easier to use.
It is an embedded database, used as a library in programs 
at the cost of not having an interactive user facility 
such as Structured Query Language (SQL) that makes
databases available to non-programmers.

### The purpose of Databases <a name="database-purpose"/>

A significant feature of databases is using *indexes* that greatly speed data access.
Assuming each data item is identified by a *key*, such a an account, order, part, or social 
security number, an index allows finding a given item in time almost
independent of the amount of data stored. Indexed databases have been used by the 
earliest data processing systems, and RDBMS incorporate indexes to be more 
efficient. Ironically, though, because of the extensive features they provide,
RDBMS are still substantially slower than the earlier simple indexed databases.

RDBMS allow allow flexible data access to exploring developing database applications,
and this makes them the most popular databases.
However, when data applications are put into production, as data processing or web
data access applications, the patterns of data access are generally fixed
and the flexibility of a RDBMS is not required. Hence, a much simpler indexed
 database can be substituted to greatly enhance performance at the
cost reimplementing the application to use the new database.

Berkeley DB is an example of such simpler indexed database systems.
Because it requires programming, changes take more time,
but for commercial applications the time is repaid by the cost saved
such as charges from a cloud service such as AWS. 
As a result, it is available for use by technical IT personnel rather than general users. 

### Berekley DB advantages<a name="berekley-db-advantages"/>

RDBMS provide other capabilities such as allowing users to concurrently access
a database, ensuring data is always valid (such as an account referenced
in an order always exists in the system), and that databases recover properly
when systems fail. 
Berkeley DB, however, also provides those capabilities as well as
much higher efficiency. 
While Berkeley DB is simpler, bacause it is programmed 
there is necessarily some complexity using it.
The Berkeley DB C++ Framework was created to simplify some of those
programming tasks to make developing and maintaining applications
using Berkeley DB easier.

### Berekley DB resources<a name="berekley-db-resources"/>

The rest of this description is intended for programmers.
Before continuing, a basic understanding of Berkeley DB is needed.
The following resources should be used to understand the 
how the Berkeley DB works and have an introduction to how
the Berkeley DB is programmed. 
While it is not essential to know all details of how
the original libraries work to use this framework,
it is necessary to know the primary C++ classes
to understand how the framework works 'under the hood'.

- [Berkeley DB Overview and software downloads](https://www.oracle.com/database/technologies/related/berkeleydb.html) (Oracle provides free access to Berkeley DB).
- [Berkeley DB Programmer's Reference Guide](https://docs.oracle.com/cd/E17276_01/html/programmer_reference/index.html)
  (as HTML, also as [PDF](https://docs.oracle.com/cd/E17076_05/html/programmer_reference/BDB_Prog_Reference.pdf)).
- [Berkeley DB book by Sleepycat Software](https://www.amazon.com/Berkeley-DB-SLEEPYCAT-Sleepycat-Software/dp/0735710643)
- [The Berkeley DB Book by Himanshu Yadava](https://www.amazon.com/Berkeley-DB-Book-Himanshu-Yadava/dp/1430211954)

