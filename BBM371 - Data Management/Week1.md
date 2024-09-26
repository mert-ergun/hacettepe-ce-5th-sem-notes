## BBM371 - Data Management: A Detailed Summary of Week 1

**I. Introduction and Course Information**

* **Course Website:** http://web.cs.hacettepe.edu.tr/~bbm371
* **Announcements:** http://piazza.com/hacettepe.edu.tr/fall2023/bbm371
* **Textbook:** Database System Concepts, Seventh Edition by Avi Silberschatz, Henry F. Korth, S. Sudarshan 
* **Reference Books:** 
    * Database Management Systems by Raghu Ramakrishnan
    * Database System Implementation by Hector Garcia-Molina, Jeffrey D. Ullman, Jennifer Widom
* **Grading:**
    * 2 Midterm Exams (25 points each) - Closed book and notes
    * Final Exam (50 points) - Closed book and notes

**II. Introduction to Data Management and Databases**

* **Data vs. Information:**
    * **Data** refers to raw, unorganized facts. Examples include: results of a dice roll, observations in a classroom, music on a CD, or a computer file.
    * **Information** is processed and organized data that becomes meaningful and useful.  
    * Data transforms into information through a process of adding context, structure, and meaning.
* **Data-Centric Applications:** Applications where data plays a central role. Examples include:
    * Airline reservation systems
    * Banking applications
    * Hospital systems
    * University systems
* **Why Use a Database System?**
    * **Data independence and efficient access:** Separates data structure from application logic, enabling efficient data retrieval.
    * **Reduced application and development time:** Provides tools and functionalities for managing data, simplifying application development.
    * **Data integrity and security:** Enforces data constraints and restricts access to unauthorized users, ensuring data accuracy and security.
    * **Uniform data administration:** Provides a centralized system for managing data definitions, access control, and data integrity.
    * **Concurrent access:** Allows multiple users to access and modify data simultaneously while maintaining consistency.
    * **Recovery from crashes:** Provides mechanisms for restoring data to a consistent state after system failures. 
* **Representing Data:** Data can be represented in various forms:
    * Text
    * Numbers
    * Images
    * Audio
    * Video 

**III. Purpose of Database Systems**

* **Early database applications built on file systems faced several challenges:**
    * **Data redundancy and inconsistency:** Duplication of data across files led to inconsistencies and difficulties in maintaining data accuracy.
    * **Difficulty in accessing data:** Required writing custom programs for each data retrieval task.
    * **Data isolation:** Data scattered across multiple files made it challenging to access and analyze related information.
    * **Integrity problems:** Enforcing data constraints was complex and often embedded in application code.
* **Database systems address these challenges by:**
    * **Atomicity of updates:** Ensures that all parts of a transaction are completed successfully or the database is rolled back to a consistent state.
    * **Concurrent access management:** Allows multiple users to access and modify data concurrently while preventing data inconsistencies.
    * **Security enforcement:** Provides mechanisms for controlling data access and protecting sensitive information.

**IV. What is a DBMS?**

* A DBMS (Database Management System) is a software package designed to store and manage large, integrated data collections (databases).
* It models real-world enterprises by representing information about:
    * **Entities:** Real-world objects such as students, faculty, or courses.
    * **Relationships:** Associations between entities, such as a student being enrolled in a course.

**V. History of DBMS**

* **Early Years (1950s - 1960s):**
    * Data stored on magnetic tapes with sequential access limitations.
    * Punched cards used for data input.
* **Late 1960s - 1970s:**
    * Hard disks allowed direct data access.
    * Network and hierarchical data models emerged.
    * Ted Codd introduced the relational data model, which became a cornerstone of modern database systems.
* **2000s:**
    * Rise of big data storage systems (Google BigTable, Yahoo PNuts, Amazon).
    * Emergence of NoSQL systems to handle diverse data types and massive datasets.
    * Big data analysis techniques like MapReduce gained popularity.
* **2010s:**
    * Resurgence of SQL as a front-end for MapReduce systems.
    * Development of massively parallel database systems for high-performance data processing.
    * Emergence of multi-core main-memory databases for faster data access.

**VI.  Example of a Traditional Database Application**

* A university database system managing information about:
    * Students
    * Courses
    * Professors
    * Enrollment details (who takes what course, who teaches which course).

**VII. Building a Database System: With and Without a DBMS**

* While storing data in files seems simple, it leads to problems as data complexity increases. 
* **Using a DBMS provides significant advantages**:
    * Data integrity
    * Concurrent access control
    * Data security
    * Efficient data retrieval 

**VIII. Why Study Databases?**

* **Shift from computation to information:** The focus is shifting from processing power to managing and extracting value from vast amounts of data.
* **Increasing data volume and diversity:** From digital libraries to genomic data, managing diverse and large datasets is crucial.
* **DBMS as a foundation of CS:**  Databases involve concepts from operating systems, programming languages, artificial intelligence, and multimedia.

**IX. Data Models**

* A data model provides a high-level, abstract way to describe:
    * Data itself
    * Relationships between data
    * Data semantics (meaning)
    * Data constraints (rules for data integrity)
* A **schema** is a detailed description of a particular collection of data using a specific data model.
* **Common Data Models:**
    * **Relational model:** Most widely used, based on tables with rows and columns.
    * **Entity-Relationship (ER) model:** Useful for database design, representing entities and their relationships.
    * **Object-based data models:** Combines object-oriented concepts with database functionalities.
    * **Semi-structured data model (XML):** Represents data in a self-describing, hierarchical format.
    * **Older models:** Network model and hierarchical model.

**X. Relational Data Model**

* The **dominant data model** used in practice.
* Represents data in **relations (tables)** with rows and columns.
* Each relation has a **schema** defining:
    * Name of the relation
    * Name of each field (attribute or column)
    * Data type of each field
* **Example:** Students(sid: string, name: string, login: string, age: integer, gpa: real)

**XI. Levels of Abstraction in a Database System**

* **Physical Layer:**  Deals with the physical storage of data on disk, including:
    * Exact physical location
    * Precise physical structure (e.g., how records are stored)
* **Logical (Conceptual) Layer:** Describes the logical structure of the database:
    * Conceptual model composed of base tables.
    * Base tables represent real data and contain physical records.
* **View (External) Layer:** Presents customized views of the data to different users:
    * Hides unauthorized data.
    * Provides customized views of the data, combining information from multiple tables.
    * Allows deriving new attributes from existing ones.

**XII. Data Independence**

* **Physical Data Independence:**  The ability to modify the physical schema (storage structure) without impacting the logical schema or applications.
* Applications rely on the logical schema, not the physical storage details.
* Changes in physical storage (e.g., adding an index) should not require application code changes.

**XIII. Structure of a Database System**

* Typically follows a layered architecture, with each layer responsible for specific functionalities.
* **Key components:**
    * Query Optimization and Execution
    * Relational Operators
    * Files and Access Methods
    * Buffer Management
    * Disk Space Management
* These layers need to address concurrency control and recovery to ensure data consistency and reliability.

**XIV. Database Architectures**

* **Centralized Databases:**
    * Single machine with shared memory among cores.
* **Client-Server Architecture:** 
    * One server machine handles database operations for multiple client machines.
* **Parallel Databases (BBM471):** 
    * Distribute data and processing across multiple interconnected machines for performance improvements.
    * Shared memory, shared disk, or shared nothing architectures.
* **Distributed Databases (BBM471):** 
    * Data physically distributed across geographically separate locations.
    * May involve schema/data heterogeneity.

**XV. Data Definition Language (DDL)**

* Used to define the database schema, specifying:
    * Tables and their attributes (columns)
    * Data types of attributes
    * Integrity constraints (e.g., primary keys, foreign keys, data validation rules)
* **Example:** `create table instructor (ID char(5), name varchar(20), dept_name varchar(20), salary numeric(8,2))`
* DDL statements are processed by the DDL compiler, which generates table templates stored in the **data dictionary**.

**XVI. Data Manipulation Language (DML)**

* Used to access and manipulate data within the database.
* Two main types:
    * **Procedural DML:** Requires specifying both what data to retrieve and how to retrieve it.
    * **Declarative DML:** Focuses on what data to retrieve without specifying the retrieval procedure. SQL is an example of a declarative DML.
* Declarative DMLs are generally easier to learn and use.
* The portion of DML focused on information retrieval is called a **query language**.

**XVII. SQL Query Language**

* Non-procedural, declarative language for querying relational databases.
* Takes input tables and returns a single result table.
* **Example:** `select name from instructor where dept_name = 'Comp. Sci.'`
* While powerful for data retrieval, SQL is not Turing-complete and requires embedding within a host language (like C++, Java, or Python) for complex computations and application logic.

**XVIII. Database Access from Application Programs**

* **Host Language:** Applications interact with databases using a host language like C++, Java, or Python.
* **Embedded SQL:** SQL queries are embedded within the host language code to access and manipulate data.
* **Application Program Interface (API):** APIs like ODBC (Open Database Connectivity) and JDBC (Java Database Connectivity) provide a standard way for applications to communicate with databases.

**XIX. Database Applications Architectures**

* **Two-Tier Architecture:** Application directly interacts with the database server. 
* **Three-Tier Architecture:**  A middle tier (application server) sits between the client and the database server. The application server handles application logic, data processing, and communication with both the client and the database. 

**XX. Database Users**

* **Naive Users:** Interact with the database through applications (e.g., bank tellers, online shoppers).
* **Application Programmers:** Develop applications that access and manipulate data using host languages and APIs.
* **Sophisticated Users (Analysts):** Use query languages and data analysis tools to extract insights from data.
* **Database Administrators:** Manage and maintain the database system, ensuring data integrity, security, and performance.

**XXI. Overview of Database Concepts Covered in the Course**

* **Covered in this course:**
    * Entity Relationship (ER) Diagrams
    * Data Definition Language (DDL)
    * Structured Query Language (SQL)
    * Utilizing the Memory Hierarchy (Buffering)
    * How to Store Data in Files
    * Finding data fast; Indexing Structures
    * External Sorting
* **Covered in BBM 471:**
    * Normalization / Functional Dependencies
    * DBMS Models
    * Relational Query Languages (RA, TRC, DRC)
    * Query Optimization
    * Concurrency Control
    * Crash Recovery 
