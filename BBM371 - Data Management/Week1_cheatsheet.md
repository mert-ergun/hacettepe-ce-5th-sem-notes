## BBM371 Week 1: Database Fundamentals - Exam Cheatsheet 

**Key Concepts**

* **Data:** Raw facts.  **Information:** Processed, organized, and meaningful data.
* **DBMS:** Software for storing, managing, and accessing databases. Solves issues faced by file-based systems (redundancy, inconsistency, access difficulties).
* **Advantages of DBMS:** Data independence, efficient access, integrity, security, concurrency, recovery.

**Data Model Basics**

* **Data Model:** High-level description of data structure, relationships, and constraints.
* **Schema:** Specific implementation of a data model for a particular dataset.
* **Relational Model:**  Most common, based on tables (relations) with rows and columns.
* **ER Model:** For database design, represents entities and their relationships.

**Database System Architecture**

* **Three Levels:**
    * **Physical:**  How data is physically stored on disk.
    * **Logical:** Logical structure, base tables representing real data.
    * **View:** Customized views for different users.
* **Data Independence:**  Physical storage can change without impacting applications.

**Database Languages**

* **DDL (Data Definition Language):** Defines schema, tables, attributes, constraints. 
* **DML (Data Manipulation Language):** Accesses and manipulates data. 
    * **SQL:** Declarative DML for querying relational databases.

**Database Applications**

* Often use a **three-tier architecture**:
    * **Client:** User interface.
    * **Application Server:**  Handles logic and data processing.
    * **Database Server:**  Manages the database.

**Additional Points**

* History of DBMS: From magnetic tapes to big data systems and NoSQL.
* SQL isn't Turing-complete; needs a host language for complex logic. 
* Different types of database users (naive, programmers, analysts, administrators).

**Remember:**  This cheatsheet highlights key points. Review the detailed summary for a thorough understanding before your exam! 
