# Three simple rules to not fail (too much) the foundations of your data design

Designing a robust and efficient relational database is crucial for the smooth operation and management of data in any application. It will asloa llow for easier evolution over time. In this article we will outline three simple rules that will help you abide by the fundamental principles of database design.

Database normalization is the process of structuring a relational database in accordance with a series of principles and rules called normal forms ( aka NF ) in order to reduce data redundancy and improve data integrity.
There are actually 10 normal forms discovered from 1970 to 2003 ( please find some more about them on wikipedia ( https://en.wikipedia.org/wiki/Database_normalization ) if you are interested ). Here are the three first and most important ones : 
* First Normal Form (1NF) : Ensure that each table column contains atomic, indivisible values and each row is unique.
* Second Normal Form (2NF) : Ensure that all non-key attributes are fully functional dependent on the primary key.
* Third Normal Form (3NF) : Ensure that all attributes are only dependent on the primary key, eliminating transitive dependencies.

It could be more straightforward, could it not ? Let's try with these next three guidelines instead.

* **Rule #1: one table represents one item**  
Here an "item" refers to a specific "entity" such as a person, object, concept, or relationship. This principle emphasizes that each table in a database should represent a single, distinct item. Adhering to this rule helps simplifying the database structure, since ensuring each table being focused on a single item, redundancy is minimized, and the database schema becomes more intuitive.
* **Rule #2: one row represents on unique instance of the item**  
An instance is a unique record that represents a specific occurrence of the item the table describes. Ensuring that uniqueness guarantees the integrity of the data. This helps in maintaining accurate and reliable records.
* **Rule #3: on column represents one unique attribute of the item**  
An attribute is an intrinsic characteristic or property of the item represented by the table. Each column in a table should store a unique attribute of the fact. With each column representing a single attribute, the database schema remains clear and unambiguous. 

By adhering to these fundamental principles of database design you can create a robust, efficient, and easy-to-maintain database. Applying these principles through a methodical design process, including identifying items, defining attributes, and normalizing data, ensures a clear, organized, and effective database schema. Of course there are sometimes need for other data design structure such as snowflake or star schema but that's another discussion.

---

published in linkedin : https://www.linkedin.com/pulse/three-simple-rules-fail-too-much-foundations-your-data-arbaudie-7vkwf/


---

Mentioned in [![Mentioned in Awesome MariaDB](https://awesome.re/mentioned-badge.svg)](https://github.com/Vettabase/awesome-mariadb)
