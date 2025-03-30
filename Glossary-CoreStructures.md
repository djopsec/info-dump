# Glossary for Core Structures

## A

**Abstract class**  
A class that cannot be instantiated on its own and is intended to be inherited by other classes. It may contain abstract methods—methods without an implementation—which must be defined in any subclass. Abstract classes are used to define a common interface or base behavior for a family of related classes.

**Abstraction**  
A fundamental concept in software design that involves hiding complex implementation details and exposing only the essential features of an object or system. Abstraction allows programmers to focus on what an object does rather than how it does it.

**Access control**  
A security technique used to regulate who or what can view or use resources in a computing environment. In databases, it refers to permissions that determine who can read, write, update, or delete data.

**Accessor**  
Also known as a getter method, it is used to read the value of a private attribute in a class. Accessors promote encapsulation by providing controlled access to class properties.

**ACID**  
An acronym representing the four key properties of database transactions: Atomicity (all-or-nothing execution), Consistency (preserving database integrity), Isolation (transactions don’t interfere with each other), and Durability (results are permanent once committed).

**Actor (use case)**  
Any user or external system that interacts with a software application to achieve a goal. Actors are often represented in use case diagrams to show how users engage with various system functions.

**Aggregate functions**  
SQL functions that perform a calculation on a set of values and return a single value, such as COUNT, SUM, AVG, MAX, and MIN. They are commonly used in data summarization.

**Aggregation**  
A form of object composition in object-oriented programming where one class contains references to other classes, but the contained objects can exist independently of the parent.

**Analysis (object-oriented)**  
The phase of software development where the problem domain is studied to identify requirements and determine what the system should do. This often leads to defining classes, relationships, and behaviors.

**ANSI**  
The American National Standards Institute, responsible for standardizing many technologies, including the SQL standard. ANSI SQL ensures consistency across different database systems.

**Approximate algorithm**  
An algorithm designed to find a good enough or near-optimal solution when an exact solution is too costly or impossible to compute. Common in fields like machine learning and facial recognition.

**Array**  
A data structure used to store multiple values in a single variable, where each value is identified by an index. Arrays allow constant-time access to elements but can be fixed in size depending on the language.

**Array index out of bounds error**  
An error that occurs when attempting to access an element outside the valid range of indices in an array. This can lead to crashes or unintended behavior.

**Array indexing**  
The operation of accessing an element in an array using its index. Indexing is typically a constant-time operation, making it efficient for data retrieval.

**Array insertion/deletion**  
The process of adding or removing elements from an array. Inserting or deleting from the middle requires shifting elements and is typically a linear-time operation, while modifying the end may be constant time.

**Jagged/Ragged array**  
A multidimensional array where rows can have different lengths. Useful for representing irregular data structures like a calendar with varying days per month.

**Resizable array**  
An array that can grow or shrink dynamically. Languages like Python and JavaScript implement resizable arrays natively (lists in Python, arrays in JavaScript).

**ASCII**  
The American Standard Code for Information Interchange, a character encoding standard that assigns numeric values to letters, digits, and symbols. It allows text to be stored and manipulated in computers.

**Associative table (database)**  
A table that implements a many-to-many relationship by linking two or more tables via foreign keys. Also known as a junction or linking table.

**Atomic transaction**  
A type of database transaction that is treated as a single unit, which either completely succeeds or completely fails. This ensures data integrity in the event of an error.

**Attribute**  
A property or data field that belongs to a class or object. Attributes store the state of an object and can be accessed and modified using accessors and mutators.

**Auto-increment**  
A feature in databases where a numeric field automatically increases with each new row. Commonly used to generate unique IDs for primary keys.

---

## B

**behavior**  
An action that an object can perform. In object-oriented programming, behaviors are typically implemented as methods inside a class. They define *what* the object can do, such as `bark()` for a Dog object or `calculateTotal()` for a ShoppingCart.

**behavioral patterns**  
A category of design patterns that focus on how objects interact and communicate with each other during execution. These patterns encapsulate how responsibilities are distributed and include patterns like Observer, Strategy, and Command.

**big O notation**  
A mathematical notation used to describe the performance or complexity of an algorithm. It expresses how the run time or space requirements grow relative to the input size (n). For example, O(n) means linear time, and O(log n) means logarithmic time.

**binary search**  
An efficient algorithm for finding an element in a *sorted* list. It works by repeatedly dividing the search range in half. If the target value is less than the middle element, the search continues in the left half; if greater, in the right half. Time complexity: O(log n).

**binary search tree (BST)**  
A special kind of binary tree where each node has up to two children. The left child contains values less than the parent node, and the right child contains values greater than the parent. BSTs support fast lookup, insertion, and deletion.

**bit**  
The most basic unit of data in computing. A bit can have a value of either 0 or 1. Bits are the foundation of all digital data, with larger data types (like bytes) made up of multiple bits.

**black boxing**  
An encapsulation technique where internal details of a component or object are hidden, and only necessary interfaces are exposed. Users of the component interact with it solely through these public interfaces, without needing to know how it works internally.

**Boolean data type**  
A data type with only two possible values: `true` or `false`. Booleans are essential in control flow and decision-making within a program, such as evaluating whether a condition is met in an `if` statement.

**BST**  
An acronym for **Binary Search Tree**. See definition above.

**bubble sort**  
A simple sorting algorithm that works by repeatedly swapping adjacent elements if they are in the wrong order. It's easy to understand but inefficient for large datasets due to its O(n²) time complexity.

**bucket**  
A container in a hash table used to store key-value pairs. When multiple keys hash to the same index, a bucket can hold them all—often as a linked list or dynamic array—to handle collisions.

---

## C

**camel case format**  
A naming convention in programming where the first word is lowercase and each subsequent word starts with a capital letter, like `totalPrice` or `numberOfStudents`. Common in Java and JavaScript for naming variables and methods.

**cascading delete**  
A database rule that automatically deletes related records when a parent record is removed. For example, if a customer record is deleted, all of their associated orders can be deleted as well to maintain referential integrity.

**chaining**  
A technique used in hash tables to handle collisions by storing multiple values at the same index in a linked list or another data structure. If multiple keys hash to the same location, they are “chained” together.

**CHAR**  
A data type in SQL that stores fixed-length character strings. If you define a `CHAR(10)` column and store a 5-character string, it will be padded with spaces to fill the 10-character limit.

**character data type**  
A basic data type that holds a single character, such as `'A'` or `'7'`. In many languages, characters are represented using standardized encodings like ASCII or Unicode.

**child class**  
A class that inherits from another class, known as the parent or superclass. It gains access to the parent's attributes and methods and can override or extend them. Also called a subclass.

**child node**  
In a tree structure, a node that is directly connected and below another node (its parent). A node can have multiple children, forming branches in a tree.

**class**  
A blueprint for creating objects in object-oriented programming. A class defines the properties (attributes) and behaviors (methods) that the created objects, or instances, will have.

**class relationships**  
Represent how classes in a system are connected. Common relationships include inheritance, association, aggregation, and composition. These are typically visualized in UML class diagrams.

**class responsibilities**  
The actions and behaviors a class is expected to perform. Good object-oriented design ensures that each class has a clear and focused responsibility (Single Responsibility Principle).

**clause, SQL**  
A part of an SQL statement that defines a specific operation or condition. Examples include `WHERE`, `ORDER BY`, `GROUP BY`, and `FROM`. Each clause plays a distinct role in shaping query behavior.

**code smell**  
A surface indication that something in the code might be wrong or poorly designed. While not always a bug, it suggests deeper problems such as duplication, long methods, or lack of cohesion, which can lead to maintenance issues.

**collaborator**  
In class design, a class that interacts with another class to perform a function. Identifying collaborators is crucial during the design phase to understand class dependencies and responsibilities.

**collection algorithms**  
Algorithms designed to manipulate data structures like arrays, lists, sets, or dictionaries. These include searching, sorting, filtering, and mapping over elements in the collection.

**collision**  
An event in a hash table when two different keys produce the same hash index. Collisions are handled using techniques like chaining or open addressing to preserve data integrity.

**column (database)**  
A vertical part of a database table representing a specific attribute of the data. For example, a `users` table might have columns for `id`, `name`, and `email`.

**compile-time polymorphism**  
A type of polymorphism resolved during compilation, typically through method overloading. The compiler selects which method to call based on the method signature—parameter type and number.

**composite key**  
A combination of two or more columns in a table that together serve as a unique identifier for a row. Composite keys are used when no single column is unique enough on its own.

**composition**  
A strong form of object relationship in which one class owns another and is responsible for its lifecycle. When the parent object is destroyed, so are its components. This is a “has-a” relationship.

**computational algorithms**  
Algorithms that compute new data from existing data, such as statistical computations, numerical simulations, or transformations. Often used in scientific, financial, and AI applications.

**conceptual model**  
An abstract representation of the key entities and their relationships within a domain. Often the first step in designing a database or object model, focusing on the logic and requirements before technical implementation.

**concrete class**  
A class that has complete implementations for all its methods and can be instantiated. It may implement abstract methods defined in an abstract class or interface.

**consistent transaction**  
A database transaction that preserves the correctness of data by ensuring that all rules, constraints, and relationships remain valid after the transaction.

**constant time**  
An operation that takes the same amount of time regardless of the input size. Denoted as O(1) in Big O notation, such as accessing an element in an array by its index.

**CRC cards**  
Short for Class, Responsibility, and Collaborator cards. A simple object-oriented design tool that helps identify the key roles of classes and how they collaborate with each other.

**creational patterns**  
A category of design patterns focused on object creation. They abstract the instantiation process and include patterns like Singleton, Factory, and Builder to increase flexibility and reuse.

**CRUD**  
An acronym that stands for Create, Read, Update, and Delete—the four basic operations for managing data in a database or persistent storage system.

---

## D

**data structure**  
A specialized format for organizing, processing, and storing data in a computer. Examples include arrays, linked lists, stacks, queues, trees, and hash tables. Choosing the right data structure improves program efficiency and readability.

**data type**  
A classification that specifies what kind of value a variable can hold, such as integers, floating-point numbers, strings, or Booleans. It defines the operations that can be performed on the data and how it’s stored in memory.

**data type (database)**  
Specifies the kind of information a database column can store, such as `VARCHAR`, `INT`, or `DATE`. Data types help maintain data integrity and optimize storage.

**database**  
A structured collection of data that can be easily accessed, managed, and updated. Databases allow for efficient querying, updating, and reporting, and are often managed by a Database Management System (DBMS).

**database column**  
The vertical part of a database table that stores a single attribute or field across all records. For example, a `users` table may have a `username` column storing each user’s name.

**database field**  
Another term for a cell in a database table; the intersection of a row and a column. It represents the actual data value for a given record and attribute.

**database index**  
A data structure that improves the speed of data retrieval in a database. It works like a table of contents, allowing the system to find records more quickly without scanning every row.

**database key**  
A value used to uniquely identify a record in a database table. Primary keys ensure that each row is unique, while foreign keys link rows between different tables.

**relational database**  
A type of database that organizes data into related tables using rows and columns. Relationships between tables are established using keys, enabling powerful queries and data normalization.

**database row**  
A horizontal entry in a database table, representing a single record. For example, a row in a `products` table might include information like product ID, name, and price.

**database table**  
A collection of related data organized into rows and columns. Tables are the basic building blocks of relational databases and each one represents a distinct entity, like `customers` or `orders`.

**database transaction**  
A sequence of operations performed as a single logical unit of work. If any part of the transaction fails, the entire operation is rolled back to ensure consistency and integrity.

**DATETIME**  
A database data type that stores date and time values. It is often used to track events like when a row was created or last updated.

**DBMS**  
Stands for Database Management System. This is software used to define, manipulate, retrieve, and manage data in a database. Examples include MySQL, PostgreSQL, and Microsoft SQL Server.

**DCL**  
Data Control Language, a subset of SQL that handles access permissions in a database. Common DCL commands include `GRANT` and `REVOKE`.

**DDL**  
Data Definition Language, a part of SQL used to define and manage database structures such as tables and indexes. Common DDL commands include `CREATE`, `ALTER`, and `DROP`.

**cascading delete**  
A rule in relational databases where deleting a parent record also automatically deletes related child records, helping maintain referential integrity.

**DELETE statement**  
An SQL command that removes rows from a database table based on specified conditions. Care must be taken when using it to avoid deleting unintended data.

**denormalization**  
The process of introducing redundancy into a database design to improve read performance, often at the expense of write efficiency and data integrity.

**deque**  
Short for “double-ended queue,” a data structure that allows elements to be added or removed from both the front and back, offering flexibility for queue-like operations.

**dequeue**  
The operation of removing an element from the front of a queue. Not to be confused with a `deque`, which supports removals at both ends.

**design (object-oriented)**  
The process of defining the structure and relationships of objects within a system. This includes selecting classes, their responsibilities, and how they interact.

**design pattern**  
A proven solution to a common software design problem. Design patterns promote best practices and are grouped into categories such as creational, structural, and behavioral.

**desktop databases**  
Database systems intended for use by a small number of users on a local machine, such as Microsoft Access. They are not designed for high scalability or web-based access.

**destructor**  
A method that is automatically called when an object is destroyed, used to free resources or perform cleanup tasks. In some languages, this is referred to as a finalizer.

**deterministic algorithm**  
An algorithm that, given the same input, will always produce the same output following the same sequence of steps.

**dictionary (collection)**  
A collection of key-value pairs where each key maps to a specific value. Also known as a hash map, associative array, or map in different languages.

**difference (set)**  
In set theory, the difference between two sets is the collection of items found in the first set but not in the second. Useful in data comparison operations.

**divide-and-conquer algorithm**  
A strategy that solves a problem by breaking it into smaller subproblems, solving each recursively, and then combining the results. Common in sorting algorithms like merge sort.

**DML**  
Data Manipulation Language, a subset of SQL used to query and update data. Commands include `SELECT`, `INSERT`, `UPDATE`, and `DELETE`.

**doubly linked list**  
A linked list where each node contains a reference to both the next and the previous node, allowing for efficient traversal in both directions.

**DRY (Don't Repeat Yourself)**  
A programming principle that emphasizes reducing repetition by abstracting and reusing code. It helps make code more maintainable and reduces bugs.

**durable transaction**  
A transaction property in which changes made are permanently recorded in the database, even in the event of a system crash.

**dynamically typed language**  
A programming language in which variable types are checked at runtime rather than at compile time. Python and JavaScript are examples, allowing for more flexibility but potentially more runtime errors.

---

## E

**encapsulation**  
A core principle of object-oriented programming where data (attributes) and methods (behaviors) are bundled within a class. Encapsulation restricts direct access to some components, promoting modularity and protecting object integrity by using access modifiers (like private, protected, and public).

**enqueue**  
The operation of adding an element to the end (rear) of a queue. It follows the First-In-First-Out (FIFO) principle and is the counterpart to `dequeue`.

**enterprise database management systems**  
Large-scale database systems designed for use by corporations or large organizations. These systems support high availability, strong security, scalability, and the ability to handle thousands of concurrent users. Examples include Oracle Database, Microsoft SQL Server, and IBM Db2.

**ER diagram**  
Stands for Entity-Relationship diagram. It’s a visual tool used to model the structure of a database by showing entities (like tables), their attributes, and the relationships between them. It helps in planning and understanding how data is connected.

**exact algorithm**  
An algorithm that always produces the correct and expected result. Unlike approximate algorithms, exact algorithms are deterministic and leave no room for ambiguity or error in their results.

**execution flow**  
The order in which individual instructions, function calls, or operations are executed during a program’s run. Understanding flow control is critical for debugging and program logic design. Common control structures that affect flow include loops, conditionals, and function calls.

**expression, SQL**  
A combination of one or more values, operators, and SQL functions that evaluate to a single value. For example, `price * quantity` is an expression that calculates the total cost.

---

## F

**factorial**  
A mathematical operation represented by an exclamation point (`!`) that multiplies a number by all positive integers less than itself. For example, `5! = 5 × 4 × 3 × 2 × 1 = 120`. Often used in recursion examples and combinatorics.

**factory method**  
A creational design pattern that provides an interface for creating objects but allows subclasses to alter the type of objects that will be created. It helps encapsulate object creation logic and promotes flexibility and code reuse.

**field (object-oriented)**  
A variable that holds data within a class or object. Also called an attribute or property, a field stores the state of an object and is typically accessed or modified via methods.

**field (database)**  
A single piece of data or attribute for a database row. It’s the intersection of a row and a column in a table, like a cell in a spreadsheet.

**FIFO (First-In, First-Out)**  
A data handling principle where the first element added is the first one removed. Queues operate using FIFO, like waiting in line at a store—first person in, first person served.

**filter**  
An operation or algorithm that removes unwanted or non-matching data from a dataset based on specific criteria. In programming, filtering is often applied to lists or streams to extract useful subsets of data.

**final class**  
A class that cannot be extended or inherited from. In languages like Java, declaring a class as `final` prevents subclassing, which can be useful for security or to preserve intended behavior.

**finalizer**  
A special method that is automatically invoked before an object is destroyed or garbage collected. It allows cleanup operations such as closing files or releasing memory. In many languages, this is handled by a destructor.

**finite set**  
A set that contains a limited number of elements. Finite sets are used in mathematical reasoning, data processing, and algorithms where bounded data is involved.

**first normal form (1NF)**  
A rule in database normalization stating that each table cell must contain only a single value, and each column must contain atomic, indivisible data. It eliminates repeating groups and ensures data integrity.

**foreign key**  
A field in one database table that references the primary key in another table, establishing a relationship between the two tables. Foreign keys enforce referential integrity and link data across tables.

**frozen set**  
An immutable version of a set in Python. Unlike regular sets, frozen sets cannot be changed after they are created, making them hashable and suitable as keys in dictionaries.

**function, hash**  
A function that converts a given key into an index within a hash table. It determines where the key-value pair is stored. A good hash function reduces the number of collisions and ensures uniform distribution.

**functionality**  
The range of operations or behaviors a software system or component can perform. It’s a key component of software requirements and is typically documented during the planning and specification phases.

**functions, aggregate**  
SQL functions that compute a single result from a set of input values, such as `SUM`, `AVG`, `COUNT`, `MIN`, and `MAX`. Used in grouping and summarizing data in queries.

**FURPS**  
An acronym for five key areas of software quality: Functionality, Usability, Reliability, Performance, and Supportability. It is used to evaluate and plan software requirements.

**FURPS Plus**  
An extension of FURPS that adds categories like Design Constraints, Implementation, Standards, and Physical Requirements. It offers a more holistic approach to capturing non-functional requirements in software development.

---

## G

**garbage collection**  
An automatic memory management feature found in many programming languages (like Java, Python, and C#). It reclaims memory used by objects that are no longer needed by the program, preventing memory leaks and optimizing performance. Programmers typically don’t need to manually free memory in languages with garbage collection.

**getter method**  
A method used to access or retrieve the value of a private field in an object. Also called an accessor, a getter enforces encapsulation by allowing controlled read access to internal object data, typically named like `getName()` or `isAvailable()`.

**“god object”**  
A programming anti-pattern where a single class takes on too many responsibilities and controls too much of the application’s logic. This violates the principle of separation of concerns and makes code harder to maintain and test. Avoiding god objects is key to clean, modular design.

---

## H

**hash function**  
A function that takes input (often a key) and returns a fixed-size numerical value, typically used as an index in a hash table. A good hash function distributes values uniformly and minimizes collisions, which occur when different inputs map to the same output.

**head (linked list)**  
The first node in a linked list. It serves as the entry point for traversing the list. The head contains a data value and a reference (or pointer) to the next node in the sequence.

**heap (using trees)**  
A specialized tree-based data structure used to implement priority queues. In a **max heap**, the parent node is always greater than or equal to its children, while in a **min heap**, the parent is always less than or equal to its children. Heaps are often used in algorithms like heap sort and for efficiently retrieving the highest (or lowest) priority item.

---

## I

**identity (object-oriented)**  
The property of an object that distinguishes it from all other objects, even if they have the same values for their attributes. In programming, two objects can have identical properties but still be distinct entities in memory.

**index (array)**  
A numerical position used to access an element in an array or list. Indexing usually starts at 0 in many languages, meaning the first element is at position 0, the second at 1, and so on. Indexing provides constant-time access to elements.

**index, database**  
A data structure (like a B-tree or hash) that improves the speed of data retrieval operations in a database. While indexes can greatly enhance query performance, they also introduce overhead on data modifications (inserts, updates, deletes).

**index number**  
Another way of referring to the index of an element in an array or list. It’s the position number used to retrieve or modify the element in constant time.

**infinite set**  
A set with an unbounded number of elements. In theoretical computer science, infinite sets appear in discussions of recursion, algorithms, and formal languages (e.g., the set of all integers).

**inheritance**  
An object-oriented programming concept where one class (the child or subclass) derives properties and behaviors from another class (the parent or superclass). Inheritance promotes code reuse and establishes a natural hierarchy between related classes.

**initialize**  
The act of assigning an initial value to a variable or data structure. Initialization is essential to prevent bugs related to undefined or unexpected values during program execution.

**instance**  
An individual object created from a class. Each instance has its own state (attribute values) and can perform actions defined by the class’s methods. Think of a class as a blueprint and an instance as the building constructed from it.

**instantiation**  
The process of creating a specific object (instance) from a class. This usually involves calling a constructor method, which sets up the object with initial values.

**interface (object-oriented)**  
A programming structure that defines a contract of methods that a class must implement. Interfaces do not contain implementation details—just method signatures. They promote flexibility and are key in designing systems that rely on polymorphism.

**intersection (set)**  
The set of elements that appear in both of two given sets. For example, the intersection of `{A, B, C}` and `{B, D, E}` is `{B}`. Useful for comparing datasets or filtering overlapping data.

**isolated transaction**  
A database transaction that runs independently of other transactions to avoid interference. Isolation ensures that simultaneous transactions produce the same result as if they were run sequentially, helping maintain data integrity.

---

## J

**jagged array**  
A type of multidimensional array where each "row" or inner array can have a different length. This is useful when working with irregular data structures like a calendar (where months have varying numbers of days). Also called a ragged array.

---

## K

**key, composite**  
A combination of two or more columns in a table used together as a unique identifier for a row. Composite keys are used when no single column can uniquely identify a record. For example, in a course registration table, a combination of `student_id` and `course_id` might serve as the composite key.

**key, database**  
A value or set of values that uniquely identifies a row in a table. The most common example is a primary key. Keys are essential for maintaining relationships between tables and ensuring data integrity.

**key, foreign**  
A column in one table that refers to the primary key in another table. Foreign keys establish links between related tables and enforce referential integrity by ensuring that referenced values exist.

**key, surrogate**  
An artificial key added to a table that has no inherent meaning or business logic. Surrogate keys are typically auto-incremented integers and are used as primary keys to simplify database design and indexing.

**key, synthetic**  
Another name for a surrogate key. It is a system-generated key that provides a unique identifier for table rows without relying on real-world data.

**key-value pair**  
A fundamental data structure in dictionaries, hash maps, and associative arrays. The **key** acts as a unique identifier, while the **value** is the data associated with that key. Common in configurations, lookups, and caching systems.

---

## L

**leaf node**  
A node in a tree data structure that has no children. It represents an endpoint or the bottom of a branch. Leaf nodes are important in recursion, search algorithms, and determining the structure’s depth or completeness.

**LIFO (Last-In, First-Out)**  
A principle where the last element added to a collection is the first one to be removed. Stacks follow the LIFO model—imagine a stack of plates where you take the top one off first.

**linear time**  
A time complexity represented as O(n), meaning the operation's duration grows proportionally with the size of the input. A common example is searching through an unsorted list.

**linked list**  
A linear data structure where elements (nodes) are linked using pointers. Each node contains data and a reference to the next (and sometimes previous) node. Unlike arrays, linked lists are dynamic and allow efficient insertion/removal but have slower access times.

**linking table (database)**  
A table that connects two other tables in a many-to-many relationship using foreign keys. Also called an associative or junction table. For example, a `student_courses` table might link `students` and `courses`.

**list (collection)**  
An ordered, indexable collection of elements. Lists are dynamic in many languages (like Python and JavaScript), allowing for efficient insertion, deletion, and traversal. Also called arrays in some contexts.

**log-linear time**  
A time complexity of O(n log n), often seen in efficient sorting algorithms like merge sort or quicksort. It combines linear and logarithmic growth, representing a balance of performance.

**logarithmic time**  
A time complexity of O(log n), where the number of operations grows slowly compared to input size. Binary search is a classic example—it repeatedly halves the problem space.

---

## M

**many-to-many relationship**  
A database relationship where multiple records in one table can relate to multiple records in another. For example, a student can enroll in many courses, and each course can have many students. This relationship is typically implemented using a linking (junction) table.

**master object**  
An anti-pattern in object-oriented design where a single object has too many responsibilities, trying to control everything else. Similar to a “god object,” it leads to tight coupling and poor maintainability—an object trying to do *way* too much.

**max heap**  
A binary tree where the parent node is always greater than or equal to its children. The largest value is always at the root, making it ideal for implementing priority queues that quickly access the maximum element.

**memento design pattern**  
A behavioral design pattern that allows an object to capture and restore its internal state without exposing its details. Useful for implementing undo features, like rolling back to a previous version of a document.

**merge sort**  
A divide-and-conquer sorting algorithm that splits a list into halves, recursively sorts them, and merges the sorted halves. Its time complexity is O(n log n), and it’s stable, but it requires additional memory.

**method (object-oriented)**  
A function defined within a class that operates on the class’s data (fields/attributes). Methods define the behaviors of objects and may include getters, setters, and business logic.

**method signature**  
The unique combination of a method’s name and its parameters (number, type, and order). It’s how compilers or interpreters differentiate between overloaded methods.

**method, static**  
A method that belongs to the class itself rather than an instance of the class. It can be called without creating an object and is often used for utility or factory methods.

**min heap**  
A binary tree where the parent node is always less than or equal to its children. The smallest value is at the root, making min heaps useful for retrieving the lowest-priority task quickly.

**minimum viable product (MVP)**  
A version of a product with just enough features to be functional and deliver value. MVPs are used to validate ideas early with minimal investment and gather feedback before scaling.

**multidimensional array**  
An array containing other arrays as elements—like a grid or matrix. Used to represent tables, game boards, or any data requiring rows and columns. Commonly visualized as a 2D or 3D structure.

**multiple inheritance**  
A feature in some programming languages (like Python and C++) where a class can inherit from more than one parent class. It allows for greater flexibility but can introduce complexity like the “diamond problem.”

**multiplicity**  
In UML diagrams, multiplicity defines how many instances of one class can be associated with instances of another. For example, `1..*` means one or more. It's a fancy way of saying “how many of these go with how many of those.”

**mutator**  
Also known as a setter method, a mutator is used to change the value of a private field in a class. It allows controlled modification and often includes validation logic.

**MVP (Minimum Viable Product)**  
Abbreviation of minimum viable product—see definition above. A favorite term in startups and agile development.

---

## N

**node**  
A fundamental unit in data structures like linked lists and trees. A node typically contains a piece of data and a reference to one or more other nodes. In a tree, a node may point to child nodes; in a list, it points to the next (and possibly previous) node.

**node, child**  
A node that is directly connected below another node (its parent) in a tree structure. Child nodes can themselves be parents of other nodes, forming branches in the tree.

**node, leaf**  
A node in a tree that has no children. It marks the end of a branch and is often used in recursion, tree traversal, and termination conditions.

**node, parent**  
A node that has one or more child nodes. It’s a higher-level node in a tree that connects to lower-level (child) nodes.

**node, root**  
The topmost node in a tree structure. It has no parent and serves as the starting point for traversing or manipulating the tree.

**node, sibling**  
Nodes that share the same parent in a tree. Sibling nodes are at the same level and often appear side-by-side in visual representations of trees.

**non-deterministic algorithm**  
An algorithm that may produce different outputs or take different paths even with the same input. These algorithms are often used in AI, optimization, or probabilistic models. They typically incorporate randomness or concurrent steps.

**non-functional requirements**  
Requirements that define how a system should perform rather than what it should do. Examples include performance, security, usability, and compliance—qualities that affect the user experience and system behavior.

**normalization rules**  
A set of rules used to design relational databases efficiently by reducing data redundancy and improving data integrity. These rules are divided into normal forms (1NF, 2NF, 3NF, etc.).

**null**  
A special marker used in databases and programming to indicate that a value is missing, undefined, or unknown. Null is not the same as zero or an empty string—it’s the absence of a value altogether.

**numerical data type**  
A type that represents numeric values, such as integers (`int`), floating-point numbers (`float`), or double-precision numbers (`double`). The precision and range depend on the type and programming language.

---

## O

**object**  
An instance of a class in object-oriented programming. Objects bundle together data (attributes) and behavior (methods), and each object maintains its own state. For example, a `Dog` class might have a `bark()` method, and each dog object has its own `name` and `breed`.

**one-to-many relationship**  
A database relationship where one record in a table is associated with multiple records in another. For example, one `Author` can write many `Books`. This is typically implemented by having a foreign key in the “many” table pointing back to the “one.”

**one-to-one relationship**  
A database relationship where each record in one table corresponds to exactly one record in another. For instance, a `User` might have one `Profile`. Often used for splitting rarely used data or sensitive data into a separate table.

**ORDER BY clause**  
An SQL clause that specifies how the results of a query should be sorted—either ascending (`ASC`) or descending (`DESC`). For example: `ORDER BY last_name ASC`.

**ordered list search**  
A search algorithm that assumes the list is sorted and usually uses methods like binary search to find the target value efficiently. Time complexity is typically O(log n).

**overloaded methods**  
Methods in the same class that share the same name but differ in the number or types of their parameters. Overloading allows for flexible function usage and improves code readability. Common in statically typed languages like Java and C++.

---

## P

**parallel algorithm**  
An algorithm designed to divide its workload across multiple processors or threads so that parts can be executed simultaneously. This increases efficiency, especially for large-scale data processing, simulations, or rendering tasks.

**parent class**  
Also called a superclass, it’s the class that is inherited from. It defines base attributes and methods that can be reused or overridden by its child (subclass). For example, a `Vehicle` class might be a parent to `Car` and `Motorcycle`.

**parent node**  
A node in a tree that has one or more child nodes connected to it. It sits one level above its children and can be used to traverse or manage tree structures hierarchically.

**performance**  
How efficiently an application or system operates. This includes speed, responsiveness, memory usage, and throughput. Performance can directly impact user satisfaction and system scalability.

**performance requirements**  
Non-functional requirements that define acceptable performance levels, such as response time, transactions per second, or maximum concurrent users.

**pointer**  
A variable that stores the memory address of another variable or object. Common in low-level languages like C and C++, pointers allow direct memory access and manipulation but must be handled carefully to avoid errors like segmentation faults.

**polymorphism**  
A principle in object-oriented programming that allows methods to behave differently based on the object invoking them. There are two main types:  
- *Compile-time polymorphism* (method overloading)  
- *Run-time polymorphism* (method overriding via inheritance)  
It’s the essence of writing flexible and reusable code.

**pop**  
An operation that removes and returns the last element from a stack (LIFO) or the end of an array. It’s often paired with `push` to manage collections dynamically.

**precision (numerical)**  
The level of exactness with which a number can be represented. For example, a `float` might represent 3.14159, but with limited decimal places. Precision matters in scientific, financial, or statistical computations.

**precondition (use case)**  
A condition that must be true before a use case or function can be executed. Preconditions are used to define valid entry states and avoid errors in logic or input.

**predicate, SQL**  
A logical expression that evaluates to true or false, used in SQL to filter query results. Examples include `price > 100` or `status = 'active'`.

**primary actor**  
In a use case, the person or system that initiates the interaction to accomplish a goal. This actor drives the scenario forward, like a user logging into a system.

**primary key (database)**  
A unique identifier for each record in a database table. A primary key ensures that no two rows have the same value in that field and is often used to establish relationships between tables.

**primitive data type**  
Basic data types provided by a programming language as building blocks, such as `int`, `char`, `float`, or `boolean`. They differ from complex or object-based types and usually offer better performance.

**priority queue**  
A specialized type of queue in which each element has a priority. The element with the highest (or lowest, depending on implementation) priority is dequeued first. Commonly implemented using heaps.

**procedural programming**  
A programming paradigm based on the concept of procedures or routines (functions). Code is organized into sequences of commands and function calls rather than into objects. C and early versions of BASIC are procedural.

**programming paradigm**  
A style or way of programming. Major paradigms include object-oriented, procedural, functional, and declarative programming. Paradigms influence how problems are conceptualized and solved in code.

**property (object-oriented)**  
An attribute or data field associated with a class or object. Properties can have getters and setters and represent the internal state of an object, like `name`, `id`, or `email`.

**push**  
An operation that adds an element to the top of a stack (LIFO) or the end of an array or list. It's the counterpart to `pop` and a core concept in dynamic collections and undo stacks.

---

## Q

**quadratic time**  
A time complexity of O(n²), meaning that as the input size doubles, the number of operations grows fourfold. Common in inefficient sorting algorithms like bubble sort or selection sort. Acceptable for small datasets but disastrous at scale.

**queue**  
A linear data structure that follows the First-In, First-Out (FIFO) principle—think of it like a line at a coffee shop. You `enqueue` to add to the back and `dequeue` to remove from the front. Used in scheduling, task management, and buffering.

**quicksort**  
A fast, divide-and-conquer sorting algorithm. It selects a pivot, partitions the array into smaller elements (left) and larger elements (right), then recursively sorts each partition. Time complexity is typically O(n log n), though it can degrade to O(n²) in the worst case. Quicksort is admired for its speed and in-place operation.

---

## R

**ragged array**  
Another term for a jagged array—a multidimensional array where each row (or inner array) can have a different length. Useful for storing non-uniform datasets, like weekly schedules where each day has a different number of events.

**random access**  
The ability to access an element at any position in a data structure in constant time (O(1)). Arrays and hash maps support random access, whereas linked lists do not—they require sequential traversal.

**recursion**  
A technique where a function calls itself to solve a problem in smaller chunks. Each call reduces the problem toward a base case, which stops the recursion. It’s elegant but must be used with care to avoid infinite loops or stack overflow.

**reference type**  
A data type where variables store references (memory addresses) rather than the actual data. Modifying the object through one reference will affect all other references to it. Common in object-oriented languages like Java and Python.

**referential integrity**  
A rule in relational databases that ensures consistency between related tables. If one table has a foreign key referring to another, the database prevents changes that would break that relationship (like deleting a parent row that's still referenced).

**relational database**  
A database that stores data in tables (relations) with rows and columns. Relationships are maintained using primary and foreign keys, and operations are performed using SQL. Think: structured, scalable, and interconnected.

**relationship**  
The logical connection between tables or entities in a database. Common types include one-to-one, one-to-many, and many-to-many. Relationships enable complex querying and data modeling.

**relationship, many to many**  
A relationship where multiple records in one table relate to multiple records in another. Implemented with a linking table. Example: students enrolled in many courses, and courses taken by many students.

**relationship, one to many**  
A relationship where one record in a table links to many records in another. For example, one author can have many books.

**relationship, one to one**  
A relationship where one record in a table links to exactly one record in another. Example: each user has exactly one profile.

**reliability**  
A measure of a system’s ability to operate without failure. Often defined in terms of uptime, fault tolerance, and recovery from errors. Critical in systems where downtime has high consequences (e.g., healthcare, aviation).

**requirements**  
The features, constraints, and behaviors that a system must meet to be considered complete. Requirements come in two main types: functional (what the system does) and non-functional (how it performs).

**resizable array**  
An array-like data structure that can grow or shrink in size as needed. Languages like Python (`list`) and Java (`ArrayList`) support resizable arrays, providing flexibility without manual memory management.

**root node**  
The topmost node in a tree. It has no parent and serves as the starting point for tree operations such as traversal, insertion, and deletion.

**row (database)**  
A single record in a database table, representing one instance of the entity the table models. For example, one customer in a `customers` table.

**run-time polymorphism**  
Also known as dynamic dispatch, this is when the method that gets called is determined at runtime, based on the actual object type. It enables different objects to respond to the same method in their own way. Key to flexible, extensible code.

**runtime stack**  
A memory structure used to keep track of active function calls in a program. Each time a function is called, a new frame is pushed onto the stack. When the function ends, the frame is popped off. It helps manage local variables, parameters, and return addresses.

---

## S

**search, binary**  
An efficient search algorithm for sorted lists. It repeatedly divides the list in half, comparing the target value to the midpoint. Time complexity: O(log n). Fast, elegant, and far better than scanning everything.

**search, ordered list**  
A search method assuming elements are sorted. Can use binary search or optimized linear techniques. Allows faster lookups compared to unordered data.

**search, unordered list**  
A basic search approach that checks each element one by one—also called linear search. Time complexity is O(n). Simple but slow for large data.

**searching algorithms**  
Algorithms designed to locate specific data within a structure. They vary in efficiency based on whether data is sorted, the structure being searched, and the algorithm used (binary search, depth-first, etc.).

**second normal form (2NF)**  
A database normalization rule that builds on first normal form. It requires that all non-key attributes depend on the entire primary key, not just part of it. Helps reduce redundancy and improves data integrity.

**secondary actor (use case)**  
A supporting role in a use case—this actor is not the initiator but contributes to completing the process. Example: a payment gateway used during an online purchase.

**security requirements**  
Non-functional requirements that define how the system must protect data and resist threats. These include authentication, authorization, encryption, and data integrity measures.

**SELECT statement**  
An SQL command used to retrieve data from a database. It allows you to specify columns, filters, and sorting. Example: `SELECT name FROM customers WHERE city = 'Austin';`

**sequential access**  
A way of accessing data where you must go through elements one at a time to reach the desired item. Linked lists use this model, as opposed to arrays with random access.

**sequential algorithm**  
An algorithm where each step happens one after another. It does not use branching or parallelism and is easy to follow but may be slow for large tasks.

**set**  
An unordered collection of unique elements. Sets are used when duplicates aren’t allowed and quick membership checks are needed. Useful for mathematical operations like union and intersection.

**SET statement**  
An SQL command used to update or assign values in a query or stored procedure. Example: `SET price = 9.99 WHERE id = 4;`

**setter method**  
Also known as a mutator, it allows controlled changes to a private field in an object. Often paired with a getter and used to maintain encapsulation.

**short int**  
A numerical data type that represents small integers—usually 16 bits in size. It saves memory when storing smaller numbers but has limited range.

**sibling nodes**  
Nodes in a tree that share the same parent. For example, in a file system tree, files in the same folder are sibling nodes.

**signed data value**  
A numeric value that can be positive, negative, or zero. The sign bit determines whether the value is above or below zero.

**single inheritance**  
A class hierarchy where a class can inherit from only one parent. Java enforces single inheritance for simplicity and to avoid issues like the “diamond problem.”

**singly linked list**  
A type of linked list where each node points only to the next one. It’s simple and memory-efficient but can only be traversed in one direction.

**snake case format**  
A naming convention where words are separated by underscores, like `total_price_with_discount`. Common in Python for variable and function names.

**SOLID**  
An acronym for five object-oriented design principles:  
- **S**ingle Responsibility  
- **O**pen/Closed  
- **L**iskov Substitution  
- **I**nterface Segregation  
- **D**ependency Inversion  
Following SOLID makes code more maintainable, scalable, and testable.

**sort, bubble**  
A simple sorting algorithm that repeatedly swaps adjacent elements if they’re in the wrong order. Easy to understand, but slow—O(n²) time complexity.

**sort, merge**  
A divide-and-conquer algorithm that splits the array into halves, recursively sorts them, and merges them back. Time complexity: O(n log n). Stable and efficient for large datasets.

**sort, quicksort**  
A fast, recursive algorithm that picks a pivot, partitions the array, and recursively sorts the partitions. Average case: O(n log n). In-place and efficient, but worst-case is O(n²).

**sorting algorithms**  
Algorithms that arrange data in a specific order—ascending or descending. Common ones include bubble sort, insertion sort, merge sort, and quicksort. Sorting improves efficiency in searching and organizing data.

**space complexity**  
A measure of how much memory an algorithm needs to run, based on the size of the input. Critical for applications running in memory-constrained environments.

**SQL**  
Structured Query Language. The standard language for interacting with relational databases—used to query, insert, update, and delete data.

**SQL clause**  
A component of an SQL statement that specifies an operation or constraint. Examples include `WHERE`, `GROUP BY`, and `ORDER BY`.

**SQL expression**  
A fragment of SQL that produces a value. Often used in `SELECT`, `WHERE`, or `SET` statements. Example: `price * quantity`.

**SQL injection**  
A security vulnerability where malicious SQL code is inserted into a query input, potentially giving attackers unauthorized access or control over the database. Prevented by using prepared statements or parameterized queries.

**SQL predicate**  
A condition that evaluates to true or false in a query. Used in `WHERE` clauses to filter results. Example: `age > 18`.

**stack**  
A linear data structure that follows the Last-In, First-Out (LIFO) principle. You `push` items onto the stack and `pop` them off in reverse order. Used in undo features, function calls, and parsing.

**static analysis tool**  
Software that checks code for errors, style violations, or security issues without running the code. Examples include linters and code quality analyzers.

**static variable/method**  
A variable or method that belongs to the class itself, not any individual instance. All objects of the class share it. Useful for shared constants, counters, or utility functions.

**statically typed language**  
A language where variable types are known at compile time. Type mismatches are caught early, offering performance and safety. Examples: Java, C, and C++.

**stored procedure**  
A precompiled group of SQL statements stored on the database server. Stored procedures can be reused and optimized for performance. Often used for complex data manipulation and business logic.

**string**  
A data type composed of a sequence of characters. Strings can be manipulated with operations like concatenation, slicing, and pattern matching.

**string data type**  
Represents text-based data like names, addresses, or messages. Strings are fundamental in both data processing and user interaction.

**structural patterns**  
Design patterns that focus on how classes and objects are composed to form larger structures. Examples include Adapter, Composite, and Decorator patterns.

**subclass**  
A class that inherits from another class (the superclass). A subclass can override or extend the behavior of its parent. Also known as a child class.

**superclass**  
The parent class from which a subclass inherits. It contains shared attributes and methods that can be reused or extended by its subclasses.

**support requirements**  
Non-functional requirements about how the system will be supported—such as documentation, customer service, training, or system maintenance.

**supportability**  
A quality metric indicating how easily a system can be maintained, monitored, extended, or fixed. High supportability is crucial for long-term system success.

**surrogate key**  
An artificial primary key (like an auto-incrementing number) used to uniquely identify rows when no natural key is available. Helps simplify relationships and indexing.

**synthetic key**  
Another term for a surrogate key. Often system-generated, it has no business meaning but is critical for relational integrity.

---

## T

**table, associative (database)**  
A database table used to model many-to-many relationships. It typically includes foreign keys that point to the related records in two other tables. Also known as a junction or linking table.

**table (database)**  
The core structure in a relational database that stores data in rows and columns. Each table usually represents an entity—like `Customers`, `Orders`, or `Products`.

**table, linking (database)**  
Another name for an associative table. It “links” two other tables together via foreign keys to establish a many-to-many relationship.

**third normal form (3NF)**  
A database normalization rule that requires data to be in second normal form and ensures that all attributes are only dependent on the primary key—not on other non-key attributes. This helps eliminate data duplication and update anomalies.

**time complexity**  
A way to measure how the runtime of an algorithm increases with the size of the input. Expressed using Big O notation (e.g., O(1), O(n), O(log n)). It helps you predict and compare algorithm performance.

**TIMESTAMP**  
A database data type used to store date and time information, often including time zone. It’s frequently used for logging when a row was created or modified.

**transaction, atomic**  
An operation that is indivisible and irreducible. Either all changes made in the transaction are saved, or none are. Prevents partial updates in case of errors.

**transaction, consistent**  
Ensures that a database moves from one valid state to another. All rules, constraints, and relationships must be preserved after the transaction completes.

**transaction, database**  
A sequence of one or more SQL operations that are executed as a single logical unit of work. If one part fails, the entire transaction is rolled back to maintain data integrity.

**transaction, durable**  
Once a transaction is committed, the changes are permanent—even in the event of a system crash. This ensures reliability and trust in the database system.

**transaction, isolated**  
Ensures that concurrent transactions don’t interfere with each other. Each one must behave as if it were the only transaction running, preserving accuracy and preventing race conditions.

**tree**  
A hierarchical data structure made up of nodes, where each node can have child nodes. The structure starts at the **root** and branches out. Trees are used in file systems, parsers, and organizational models.

**tree, binary search**  
A type of binary tree where the left child of a node holds a smaller value, and the right child holds a larger value. Enables fast searching, insertion, and deletion—O(log n) average time complexity.

**tree, unbalanced**  
A tree where the left and right subtrees of some nodes differ significantly in depth. This can degrade performance—especially for binary search trees, where an unbalanced tree may resemble a linked list.

---

## U

**UML (Unified Modeling Language)**  
A standardized way to visualize the design of a system. UML uses diagrams to represent classes, objects, use cases, and relationships. It’s super handy for planning software architecture, especially in object-oriented programming.

**unbalanced tree**  
A tree data structure where one side (left or right) grows much deeper than the other. This imbalance can hurt performance—especially for search operations—since it undermines the efficiency of structures like binary search trees.

**union (set)**  
A set operation that combines all unique elements from two or more sets. For example, the union of `{A, B, C}` and `{B, D}` is `{A, B, C, D}`. Frequently used in data merging and comparison logic.

**unit test**  
A small, isolated test that verifies the behavior of a specific part of code—usually a function or method. Unit tests help catch bugs early and support safe refactoring. They're the building blocks of test-driven development (TDD).

**unordered list search**  
A basic search algorithm that checks each element in a list sequentially, since the list isn't sorted. Also called linear search. Time complexity: O(n).

**unsigned data value**  
A numeric value that can only be zero or positive—no negative numbers allowed. Often used when negative numbers don’t make sense (like quantity, IDs, or memory addresses).

**usability**  
A non-functional requirement that describes how intuitive and user-friendly an application is. Good usability includes clear navigation, helpful feedback, and minimal learning curve.

**use case diagram**  
A type of UML diagram that shows how users (actors) interact with a system. It visualizes user goals and the system’s responsibilities, making it ideal for requirements gathering and stakeholder communication.

**use case scenario**  
A narrative or structured description of how an actor achieves a specific goal with the system. It focuses on user intent and step-by-step interaction, helping developers understand practical flows and edge cases.

---

## V

**VARCHAR**  
Short for “variable character.” A database column type used to store strings of text with varying length. Unlike `CHAR`, which reserves space for a fixed number of characters, `VARCHAR` uses only as much space as needed (up to a defined limit), making it more storage-efficient.

**variable, static**  
A variable that belongs to the class itself rather than any instance. All objects of that class share the same value. Used for things like counters, constants, or shared configuration settings.

**visibility**  
In object-oriented programming, visibility defines who can access a class’s methods or attributes. Common levels include:  
- `public`: accessible from anywhere  
- `private`: accessible only within the class  
- `protected`: accessible within the class and its subclasses  
Visibility helps enforce encapsulation and keep internal implementation details hidden.

---

## W

**WHERE clause**  
An SQL clause that filters rows returned by a query based on specific conditions. It allows you to select only the records that match certain criteria.  
Example: `SELECT * FROM orders WHERE status = 'shipped';`

---

## Y

**YAGNI (You Aren’t Gonna Need It)**  
A software development principle that advises against implementing functionality until it’s necessary. It helps keep code clean, focused, and avoids wasting time on hypothetical features. A core tenet of agile and lean development.
