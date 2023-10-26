# ASSIGNMENT OF RELATIONAL DESIGN AND NORMALISATION

                                                             **RELATIONAL DESIGN**
Relational database design (RDD) models information and data into a set of tables with rows and columns. Each row of a relation/table represents a record, and each column represents an attribute of data. The Structured Query Language (SQL) is used to manipulate relational databases. The design of a relational database is composed of four stages, where the data are modeled into a set of related tables. The stages are:

* Relations/attributes - Relation is sometimes used to refer to a table in a relational database but is more commonly used to describe the relationships that can be created between those tables in a relational database.

* Primary keys - A primary key is the column or columns that contain values that uniquely identify each row in a table. A database table must have a primary key for Optim to insert, update, restore, or delete data from a database table. Optim uses primary keys that are defined to the database. However, you can also define primary keys to supplement those in the database.

 * Relationships -it is an association between tables. Those associations create using join statements to retrieve data. It is a condition that exists between two database tables in which one table contains a foreign key that references the primary key of the other tables. Relationships enable relational databases to divide and store data in separate tables while connecting disparate data items.

* Normalization -Database normalization is the process of organizing data into tables in such a way that the results of using the database are always unambiguous and as intended
  
Relational databases differ from other databases in their approach to organizing data and performing transactions. In an RDD, the data are organized into tables and all types of data access are carried out via controlled transactions. Relational database design satisfies the ACID (atomicity, consistency, integrity and durability) properties required from a database design. Relational database design mandates the use of a database server in applications for dealing with data management problems.

The four stages of an RDD are as follows:

* Relations and attributes: The various tables and attributes related to each table are identified. The tables represent entities, and the attributes represent the properties of the respective entities.
* Primary keys: The attribute or set of attributes that help in uniquely identifying a record is identified and assigned as the primary key
* Relationships: The relationships between the various tables are established with the help of foreign keys. Foreign keys are attributes occurring in a table that are primary keys of another table. The types of relationships that can exist between the relations (tables) are:<br><br>
  * One to one<br>
   * One to many<br>
    * Many to many
 
                                                            **NORMALIZATION**
 
*  Normalization is the process of organizing the data in the database.
*  Normalization is used to minimize the redundancy from a relation or set of relations. It is also used to eliminate undesirable characteristics like Insertion, Update, and Deletion Anomalies.
*  Normalization divides the larger table into smaller and links them using relationships.
The normal form is used to reduce redundancy from the database table.


The main reason for normalizing the relations is removing these anomalies. Failure to eliminate anomalies leads to data redundancy and can cause data integrity and other problems as the database grows. Normalization consists of a series of guidelines that helps to guide you in creating a good database structure.

Data modification anomalies can be categorized into three types:

  * Insertion Anomaly: Insertion Anomaly refers to when one cannot insert a new tuple into a relationship due to lack of data.<br>
   * Deletion Anomaly: The delete anomaly refers to the situation where the deletion of data results in the unintended loss of soe other important data.<br>
* Updatation Anomaly: The update anomaly is when an update of a single data value requires multiple rows of data to be updated.<br>

Types of Normal Forms:
Normalization works through a series of stages called Normal forms. The normal forms apply to individual relations. The relation is said to be in particular normal form if it satisfies constraints.

|Normal Form	|Description|
|-------------|-----------|
|1NF | 	A relation is in 1NF if it contains an atomic value.|
|2NF |	A relation will be in 2NF if it is in 1NF and all non-key attributes are fully functional dependent on the primary key.|
|3NF|	A relation will be in 3NF if it is in 2NF and no transition dependency exists.|
|BCNF|	A stronger definition of 3NF is known as Boyce Codd's normal form.|
|4NF|	A relation will be in 4NF if it is in Boyce Codd's normal form and has no multi-valued dependency.|
|5NF|	A relation is in 5NF. If it is in 4NF and does not contain any join dependency, joining should be lossless.|

Advantages of Normalization:<br><br>
 * Normalization helps to minimize data redundancy.<br>
 * Greater overall database organization.
  * Data consistency within the database.
  * Much more flexible database design.
*  Enforces the concept of relational integrity.<br><br>

Disadvantages of Normalization:<br>
* You cannot start building the database before knowing what the user needs.
 * The performance degrades when normalizing the relations to higher normal forms, i.e., 4NF, 5NF.
 * It is very time-consuming and difficult to normalize relations of a higher degree.
 * Careless decomposition may lead to a bad database design, leading to serious problems.



      


