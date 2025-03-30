# Glossary for Key Approaches

## A

### acceptance criteria  
A clear and specific set of requirements that must be met for a user story or feature to be considered complete and accepted by a stakeholder.  
**Example**: “Given a logged-in user, when they click ‘Logout’, then they should be redirected to the login page.”

### access control  
Rules and mechanisms that determine who is allowed to access which parts of a system, such as files, functions, or data.  
**Use case**: Only admins can delete user accounts.

### ACID  
An acronym for Atomicity, Consistency, Isolation, and Durability. These are the four key properties of reliable database transactions.  
- **Atomicity**: All steps in a transaction complete, or none do.  
- **Consistency**: The database is never left in a bad state.  
- **Isolation**: Transactions don’t interfere with each other.  
- **Durability**: Once committed, data won’t be lost—even if the system crashes.

### ACL (Access Control List)  
A list that specifies which users or roles have what level of access (read, write, execute) to a specific resource.  
**Example**: A file ACL might show that Alice can read and write, but Bob can only read.

### adapter design pattern  
A structural design pattern that allows incompatible interfaces to work together by converting one interface into another.  
**Analogy**: Think of it like a power adapter that lets your US plug fit into a European outlet.

### @AfterAll  
A JUnit annotation used to mark a method that should run once after all test cases in a test class have completed.  
**Use case**: Clean up shared resources like closing a database connection.

### @AfterEach  
A JUnit annotation used to run a method after each individual test case.  
**Use case**: Resetting variables or data between tests to avoid test pollution.

### aggregate object  
A collection of elements (like an array or list) that can be traversed using an iterator in the Iterator design pattern.

### agile  
An iterative and flexible software development methodology emphasizing collaboration, customer feedback, and small, frequent releases.  
**Common traits**: Standups, sprints, retrospectives, and a focus on "working software over comprehensive documentation."

### allocation, memory  
The process of reserving space in a computer’s memory to store data temporarily.  
**Types**: Static allocation (at compile-time) and dynamic allocation (at runtime).

### API (Application Programming Interface)  
A set of rules and definitions that allow one piece of software to talk to another.  
**Example**: When a weather app fetches today’s forecast from a server, it’s using an API.

### arena (Python)  
In Python’s memory management system, an arena is a large block of memory that is internally divided into smaller blocks or pools used to store Python objects.

### argument (GraphQL)  
In a GraphQL query, arguments are like parameters that refine the data you’re requesting.  
**Example**: `getUser(id: 123)` — `id` is the argument.

### assert statement  
A programming construct that checks whether a condition is true. If not, it typically throws an error.  
**Example**: `assert x > 0` ensures `x` is positive during debugging or testing.

### assertEquals  
A specific assertion used in testing frameworks like JUnit to confirm two values are equal.  
**Example**: `assertEquals(expected, actual)`

### assertions, type-specific  
Assertions tailored to specific data types to make tests more expressive.  
**Example**: `assertThat(string).endsWith("world")`

### AssertJ  
An assertion library that provides a rich, fluent syntax for writing more readable and intuitive tests in Java.  
**Bonus**: It works seamlessly with JUnit.

### assertSame  
Checks that two objects reference the exact same memory location, not just equal content.  
**Example**: `assertSame(obj1, obj2)` passes only if `obj1` and `obj2` are the *same* object.

### assertThrows  
Used in test cases to verify that a specific exception is thrown during execution.  
**Example**: `assertThrows(IllegalArgumentException.class, () -> someFunction(null));`

### attack tree  
A diagram used to model potential security threats to a system by visualizing the steps an attacker might take to achieve a goal.  
**Think of it like** a decision tree but for security.

### authentication  
The process of verifying that someone is who they claim to be.  
**Example**: Entering a username and password to log in.

### authorization  
Determines what an authenticated user is allowed to do.  
**Example**: A user is authenticated but only authorized to read data, not edit it.

### automated  
Indicates that a task or test is performed by a script or tool, without manual intervention.  
**Use case**: An automated regression test runs every time code is pushed.

### automatic memory management  
A system where the programming environment takes care of memory allocation and cleanup (e.g., garbage collection), so you don’t have to manually free memory.  
**Languages**: Java, Python, JavaScript.

### automatic variables (C language)  
Local variables that are automatically created and destroyed within the scope of a function.  
**Note**: This is the default behavior for local variables in C.

---

## B

### base object  
In the **Decorator Design Pattern**, the base object is the original object that is being enhanced or extended. Additional behavior is "wrapped" around it using composition, without modifying its source code.  
**Example**: A plain coffee object wrapped with decorators like "milk" or "whipped cream" to build a latte.

### @BeforeAll  
A JUnit annotation for a method that runs **once** before any test methods in a test class are executed.  
**Use case**: Set up shared resources like database connections or test servers.

### @BeforeEach  
A JUnit annotation for a method that runs **before every** individual test method in the test class.  
**Use case**: Resetting data or state to ensure each test starts fresh and independent.

### bind variables  
Used in database queries (especially SQL) to insert values safely, avoiding direct string concatenation.  
**Why it matters**: Helps prevent **SQL injection** attacks by keeping data and query structure separate.  
**Example**: `SELECT * FROM users WHERE id = ?`

### black box testing  
A testing method where the tester only sees the **inputs and outputs**, without knowing how the system works internally.  
**Analogy**: Like testing a vending machine—put in a dollar, expect a soda, no idea what’s going on inside.

### blacklisting  
A security approach where known **bad inputs** or patterns are blocked.  
**Example**: Rejecting any input that contains `<script>` to avoid cross-site scripting (XSS).  
**Limitation**: Hard to cover every malicious case—**whitelisting** is usually preferred.

### block (Python)  
In Python memory management, a **block** is a chunk of memory within a pool used to store individual objects. Python organizes memory into arenas → pools → blocks.

### block starting symbol (C language)  
Also known as **BSS**, this refers to a special memory segment in C used for uninitialized global or static variables.  
**Fun fact**: It helps optimize memory usage by not allocating storage until needed.

### body (SOAP)  
The main part of a SOAP message that contains the actual **data payload**.  
**Structure**: Inside the `<Envelope>` element, the `<Body>` holds the operational content—often formatted in XML.

### bottom-up approach  
A development or testing strategy where small units are built or tested **first**, and then integrated into larger systems.  
**Example**: Write unit tests for functions before testing the entire application logic.

### box testing  
A general term for types of testing categorized by the tester’s **visibility into the system’s internals**:  
- **Black box**: No visibility  
- **White box**: Full visibility  
- **Gray box**: Partial/internal knowledge  
Think of it as “how much of the ‘box’ you can see.”

### broken cryptographic routine  
A cryptographic method that has known weaknesses, has been compromised, or is outdated.  
**Example**: MD5 is a broken hashing algorithm due to collision vulnerabilities.

### brute-force attack  
A hacking method where an attacker tries **every possible combination** of passwords until one works.  
**Prevention tips**: Use long, complex passwords and rate-limit login attempts.

### BSS (Block Starting Symbol)  
A memory segment in C/C++ for **uninitialized static and global variables**. It conserves space by not storing the actual zero values, just their intent.

### buffer overflow vulnerability  
Occurs when a program writes more data to a buffer (e.g., an array) than it can hold, which may overwrite adjacent memory.  
**Why it's dangerous**: Can lead to **security exploits**, crashes, or remote code execution.

### bug bash  
A focused event, usually a day or week, where everyone on the team (not just QA) helps find and fix bugs.  
**Best practice**: Hold bug bashes regularly (2–4 times a year) to improve quality and catch edge cases.

### bug book  
A document that tracks known **security vulnerabilities** in a system, including their details, impact, and current status.  
**Think of it as**: A vulnerability journal for your application.

### bug priority  
How **urgently** a bug should be fixed.  
- **High priority**: Fix ASAP—maybe it's blocking development.  
- **Low priority**: Won’t stop release; fix later.

### bug severity  
How **bad** the bug’s impact is on the system.  
- **High severity**: Crashes app or causes data loss  
- **Low severity**: Cosmetic issue, like a UI typo

### bug triage  
The process of reviewing, classifying, and prioritizing bugs. It helps the team decide what gets fixed first, who will fix it, and when.  
**Analogy**: Like a hospital triage nurse assigning urgency to incoming patients.

### build phase  
A step in the **software development lifecycle (SDLC)** where the actual code is written and assembled into a working product.  
**Activities include**: Writing source code, compiling, integrating components, and preparing for testing.

---

## C

### call stack  
A special stack data structure used by programming languages to keep track of function calls.  
Each time a function is called, a frame is added to the stack; when a function ends, its frame is popped off.  
**Why it matters**: Understanding the call stack helps debug issues like infinite recursion or stack overflows.

### certificate  
A digital document that verifies the identity of a website or service.  
**Example**: When you visit a site with HTTPS, it presents a certificate to prove it's legit.  
**Common use**: TLS/SSL certificates for secure connections.

### changing functional declaration  
A refactoring step where a function or method is renamed (or its signature is updated) to better reflect what it does.  
**Why**: Improves code readability and understanding.

### CI/CD (Continuous Integration / Continuous Deployment)  
A development practice where code is integrated, tested, and deployed frequently using automation.  
- **CI**: Developers push code changes regularly, triggering automated tests.  
- **CD**: Code that passes CI is automatically deployed to production or staging.  
**Goal**: Faster, safer releases with less manual effort.

### client-side validation  
Validating user input **in the browser** before it’s sent to the server.  
**Why use it**: Gives users instant feedback (e.g., “This field is required”), but it should **never** be the only line of defense—always validate again on the server.

### code smell  
A piece of code that technically works but feels "off"—it may be overly complex, duplicated, or hard to follow.  
**Analogy**: It’s like a musty room—you know something needs cleaning.  
**Fix**: Refactor it!

### compacting  
A step in garbage collection where fragmented memory blocks are reorganized to close gaps, making more space available.  
**Think of it like**: Defragmenting your hard drive, but for memory.

### composition vs. inheritance  
Two ways of reusing code:
- **Inheritance (IS-A)**: A class extends another.  
  → `Car IS-A Vehicle`
- **Composition (HAS-A)**: A class uses another as a component.  
  → `Car HAS-A Engine`

**Why prefer composition?** It’s more flexible and avoids tight coupling between parent and child classes.

### concurrency  
When a program can execute **multiple tasks at the same time** (or appear to).  
**Common in**: Multithreaded applications, web servers, and game engines.  
**Example**: Handling multiple web requests in parallel.

### configuration  
Settings or options that control how an application runs.  
**Examples**: Environment variables, API keys, feature toggles.  
**Tip**: Keep configuration separate from code, and avoid hardcoding sensitive info.

### containerized  
Packaging an application along with everything it needs to run—dependencies, libraries, configs—into a self-contained environment (usually via Docker).  
**Why it rocks**: “It works on my machine” becomes “It works everywhere.”

### convention  
An unofficial standard or best practice followed by developers.  
**Examples**:  
- Java method names use camelCase  
- Tests live in a `/tests` directory  
**Why follow them?** Conventions make codebases predictable and easier to read.

### copy, deep  
Creates a new object **and** new copies of everything it references.  
**Useful when**: You want to completely duplicate a structure, not just its top-level reference.  
**Example**: Cloning a nested JSON object so changes to the copy don’t affect the original.

### copy, shallow  
Creates a new object that **shares references** to inner objects with the original.  
**Result**: Changing a nested value in the copy affects the original.  
**Use with caution** in shared-state scenarios.

### CPU (Central Processing Unit)  
The brain of the computer—it executes program instructions.  
**Fun fact**: It reads data from memory, runs calculations, and writes results back—billions of times per second.

### cross-site scripting (XSS)  
A type of attack where a hacker injects malicious code (often JavaScript) into a web page that’s viewed by others.  
**Example**: `<script>alert("hacked")</script>`  
**Prevention**: Always escape or sanitize user input.

### CVE (Common Vulnerabilities and Exposures)  
A public list of known security vulnerabilities, each with a unique ID (like `CVE-2024-12345`).  
**Use it to**: Track and patch security issues in dependencies.

### CWE (Common Weakness Enumeration)  
A list of **common software weaknesses**, like “buffer overflow” or “hardcoded passwords.”  
**Maintained by**: MITRE.  
**Why it matters**: Great for understanding root causes of vulnerabilities, not just symptoms.

### cyclic reference  
A situation where two or more objects reference each other, forming a loop.  
**Problem**: Can confuse garbage collectors and cause memory leaks if not handled properly.  
**Example**: `A → B → A`

---

## D

### dangling pointer  
A pointer that references a memory location that has already been freed or deallocated.  
**Why it's bad**: Accessing a dangling pointer can cause crashes or unexpected behavior.  
**Mostly seen in**: Low-level languages like C and C++.

### data segment (C language)  
A portion of memory used to store **initialized global and static variables**.  
**Differs from** the BSS segment, which stores uninitialized variables.

### DBA (Database Administrator)  
The person responsible for managing and maintaining databases.  
**Tasks may include**:  
- Configuring and tuning the database  
- Performing backups and recovery  
- Setting up user permissions  
- Monitoring performance and security

### deallocation, memory  
The process of **freeing up memory** when it’s no longer needed, so it can be reused.  
**In manual memory management languages** (like C), this must be done explicitly with functions like `free()`.  
**In garbage-collected languages**, the system handles it for you.

### decorator design pattern  
A structural design pattern used to add responsibilities or behavior to objects **dynamically**, without modifying their code.  
**Analogy**: Think of wrapping a present with layers of ribbons, bows, and sparkles.  
**Example**: A text box object wrapped with scrollbars, then border decorations.

### deep copy  
A copy of an object where **all referenced objects** are also copied recursively.  
**Use when**: You want to duplicate a structure completely and avoid shared state between the original and copy.

### define phase  
A phase in the **Software Development Life Cycle (SDLC)** where project requirements are gathered and clearly documented.  
**Deliverables**: Specifications, acceptance criteria, and user stories.

### DELETE operation (REST)  
An HTTP method that removes a specified resource from a server.  
**Example**: `DELETE /users/123` removes the user with ID 123.  
**Note**: Often requires authentication and confirmation.

### dependency graph  
A visual or structured map that shows which parts of a system **depend on which external libraries or modules**.  
**Use case**: Helps identify weak points and understand the impact of updating a dependency.

### dependent object  
In the **Observer Design Pattern**, this is the “subscriber” or “listener” that reacts when the “subject” changes.  
**Example**: A news feed subscriber gets updates from the publisher.

### deploy phase  
The stage in the SDLC where the finished product is released into production or staging environments.  
**May involve**:  
- Packaging code  
- Uploading to servers or containers  
- Triggering CI/CD pipelines

### design pattern, adapter  
A pattern that allows two incompatible interfaces to work together.  
**Analogy**: Like using a travel adapter to plug your U.S. charger into a European outlet.

### design pattern, decorator  
See `decorator design pattern` above.

### design pattern, factory method  
A **creational pattern** that lets a class defer the instantiation of objects to its subclasses.  
**Benefit**: You can create new types of objects without changing the code that uses them.  
**Example**: A `ShapeFactory` that returns a `Circle`, `Square`, or `Triangle`.

### design pattern, iterator  
A behavioral pattern that provides a standard way to loop through a collection **without exposing its internal structure**.  
**Example**: `for (item in list)` in Python or JavaScript.

### design pattern, observer  
A behavioral pattern where one object (subject) notifies a group of dependent objects (observers) when its state changes.  
**Use case**: Event-driven systems like user interface updates or messaging apps.

### design pattern, strategy  
Encapsulates related algorithms in separate classes and makes them interchangeable.  
**Why it’s cool**: You can choose the best behavior at runtime.  
**Example**: Different sorting strategies (`quickSort`, `mergeSort`, `bubbleSort`).

### design phase  
An SDLC stage where the team maps out the system architecture, mockups, database schemas, and technical decisions before building.  
**Output**: Wireframes, UML diagrams, API contracts.

### design principle, open-closed  
States that **software entities should be open for extension, but closed for modification**.  
**Why it matters**: Encourages building flexible systems without breaking existing code.

### design principle, single responsibility  
States that a class or module should have only **one reason to change**—i.e., it should do one thing and do it well.  
**Helps with**: Code readability, maintainability, and testability.

### design principles  
General rules or philosophies that guide good software design.  
**Examples**: SOLID principles, KISS (Keep It Simple, Stupid), DRY (Don’t Repeat Yourself).

### development sprint  
A short, fixed period of time (usually 1–4 weeks) in **Agile** development where a team works to complete specific tasks or user stories.  
**Includes**: Planning, daily standups, demos, and retrospectives.

### DevOps  
A culture and set of practices that combines **software development (Dev)** and **IT operations (Ops)**.  
**Goal**: Shorten the development lifecycle while delivering features, fixes, and updates frequently and reliably.

### DevSecOps  
An evolution of DevOps that also integrates **security** into the workflow.  
**Motto**: “Shift security left” — address vulnerabilities earlier in the pipeline.

### DoS (Denial of Service)  
A cyberattack in which a system is overwhelmed with traffic or requests, making it unavailable to legitimate users.  
**Common method**: Sending millions of requests per second to crash the server.

### DS (Data Segment)  
Same as the **data segment** in C. Stores initialized global/static variables in memory.

### dummy object  
A basic placeholder object used in testing that fills in for a real one but has no behavior.  
**Use case**: Just there to make the test compile or execute.

### dynamic analysis  
The process of analyzing a program **while it runs** to gather data like memory usage, CPU consumption, and execution flow.  
**Useful for**: Performance tuning and finding runtime bugs.

### dynamic memory allocation  
The process of allocating memory during a program’s **execution**, as opposed to compile time.  
**Example**: Using `malloc()` in C or creating new objects in Python.

---

## E

### endurance testing  
A form of **performance testing** that evaluates whether a system can handle a certain load over a **long period of time**.  
**Why it's useful**: It reveals memory leaks, resource exhaustion, and degradation that only show up after prolonged usage.  
**Example**: Simulating 1,000 users interacting with a web app continuously for 48 hours.

### envelope (SOAP)  
The outermost structure of a **SOAP message**, acting as a wrapper for the message's metadata and content.  
**Contains**:  
- **Header**: Optional metadata  
- **Body**: Required content (the actual message)  
**Think of it as**: An email envelope that contains the actual message and delivery instructions.

### error messaging, information disclosure through  
When an error message **leaks sensitive details** to users or attackers.  
**Example**:  
- "Invalid username" (leaks that the username exists)  
- A full **stack trace** shown on a public-facing app  
**Fix**: Use generic error messages and log details internally.

### error, out of memory  
Occurs when a system or application tries to allocate memory, but **none is available**.  
**Why it happens**:  
- Memory leaks  
- Handling too much data  
- Mismanaged loops or recursions  
**Prevention**: Monitor memory usage, clean up resources, use pagination for large data loads.

### error, stack overflow  
A crash that occurs when too many function calls are pushed onto the **call stack**, often due to infinite recursion.  
**Analogy**: Like adding too many books to a stack until it topples over.  
**Fix**: Ensure base cases are correctly defined in recursive functions.

### escaping references  
Happens when a variable (usually private or temporary) is unintentionally **exposed or leaked** to other parts of the program.  
**Why it’s risky**: Can break encapsulation and lead to unintended side effects.  
**Example**: Returning a mutable internal list directly from a class method.

### expected result  
In testing, this is what you **expect to happen** when a test is run with specific input.  
**Why it matters**: Without an expected result, you don’t know if a test passed or failed.  
**Format**: Often written as “Given → When → Then” in acceptance criteria.

### extract function refactoring  
A technique used to break down a long or complex function into smaller, **reusable**, and **clearer** functions.  
**Benefits**:  
- Improves readability  
- Encourages reuse  
- Simplifies debugging and testing  
**When to use**: If a function does too many things or has repeated code.

---

## F

### factory method design pattern  
A **creational design pattern** that provides an interface for creating objects, but allows subclasses to decide **which class to instantiate**.  
**Why use it?** It decouples object creation from its usage, promoting flexibility and scalability.  
**Example**: A `NotificationFactory` that creates either `EmailNotification` or `SMSNotification` based on input.  
**Bonus**: It supports the **Open-Closed Principle**—you can add new types without changing existing code.

### fake object  
A type of **test double** that contains working, but non-production-ready logic.  
**Use case**: Useful for testing basic flows without requiring the real system, like simulating a database without actual queries.  
**Example**: A fake payment processor that always returns success.

### faking it  
In **test-driven development (TDD)**, this means writing the **simplest code possible** to make a test pass—without worrying about the full implementation yet.  
**Why it helps**: Keeps you from over-engineering and helps you build incrementally.  
**Example**: Return a hardcoded value like `return 42;` just to satisfy a failing test.

### fault (SOAP)  
An optional part of a **SOAP message** that provides information about **errors** that occurred during message processing.  
**Structure**: Located inside the `<Body>` element, it includes details like fault code, message, and more.  
**Analogy**: Like a red “error card” inside a returned envelope saying, “This didn’t go through, here’s why.”

### field name (GraphQL)  
In a GraphQL query, a field is a **unit of data** you're asking for. Each field corresponds to a piece of data on the server.  
**Example**: In the query `{ user { name email } }`, `name` and `email` are fields requested from the `user` object.

### fragmentation, heap  
Occurs when objects are **allocated and deallocated** in a way that leaves small, unusable gaps in heap memory.  
**Impact**: Reduces performance and available memory.  
**Fix**: Compaction during garbage collection or using memory pools.

### free (C language)  
A **manual memory management** function in C that deallocates heap memory previously allocated with `malloc()` or `calloc()`.  
**Important**: Failing to call `free()` causes **memory leaks**.  
**Pitfall**: Don't `free()` memory twice or you'll risk undefined behavior.

### functional declaration, changing  
In TDD or refactoring, this means **renaming or adjusting** a method’s signature to better match its purpose.  
**Example**: Rename `process()` to `generateInvoice()` to make its behavior clearer.

---

## G

### garbage collection  
A **memory management process** that automatically finds and removes objects that are no longer used by the program.  
**Why it matters**: Prevents memory leaks without requiring the programmer to manually deallocate memory.  
**Used by**: Languages like Python, Java, and JavaScript.  
**Analogy**: Like a cleaning robot that finds and throws away forgotten items around the house.

### GET operation (REST)  
An HTTP method used to **retrieve data** from a server.  
**Example**: `GET /users/123` returns the user with ID 123.  
**Important**: GET requests should be **idempotent**—calling them multiple times shouldn't change the state of the server.

### given  
A keyword used in **acceptance criteria** or **BDD (Behavior-Driven Development)** to describe the **starting state** of a scenario.  
**Example format**:  
`Given` I am logged in,  
`When` I view my dashboard,  
`Then` I see my latest activity.

### GraphQL  
A **query language** for APIs that allows clients to **request exactly the data they need** and nothing more.  
**Why it’s cool**:  
- Reduces over-fetching and under-fetching  
- Gives clients control over data  
- Great for complex or nested data structures  
**Contrast with REST**: REST uses fixed endpoints, GraphQL uses a flexible schema.

### gray box testing  
A type of software testing that blends both **black box** and **white box** approaches.  
**What it means**: Testers have **partial knowledge** of the internal workings of the system.  
**Use case**: Often used for integration tests, where some understanding of architecture is beneficial.  
**Analogy**: You can peek behind the curtain—but only halfway.

---

## H

### Hamcrest  
A third-party **assertion framework** for Java that lets you write **more readable test assertions** using matchers.  
**Example**:  
Instead of `assertEquals("hello", value);`  
You can write: `assertThat(value, is("hello"));`  
**Why it rocks**: Great for writing expressive, fluent tests in JUnit.

### happy path scenario  
A test or workflow that follows the **ideal user journey**, where everything goes as expected without any errors.  
**Why it’s useful**: Verifies that the system behaves correctly under normal conditions.  
**Example**: A user signs up with valid information, receives a confirmation email, and logs in without issue.

### hasNext method  
Used in the **Iterator Design Pattern**, this method checks if there are **more elements** to iterate over.  
**Returns**: A Boolean—`true` if more elements exist, `false` otherwise.  
**Example** (Java):  
```java
while (iterator.hasNext()) {
    System.out.println(iterator.next());
}
```

### HATEOAS (Hypermedia as the Engine of Application State)  
A constraint of REST APIs that means the server provides links in its responses so the client can discover **what actions are possible next**.  
**Why it matters**:  
- Makes APIs self-descriptive  
- Reduces tight coupling between client and server  
**Example**: A `GET /orders/123` response includes a `_links` field with URLs for `cancel`, `update`, or `checkout`.

### header (SOAP)  
An **optional part of a SOAP message** that contains **metadata** like authentication information, message routing details, or custom tags.  
**Where it lives**: Inside the `<Envelope>` but before the `<Body>`.  
**Analogy**: Like the "To:", "From:", and "Subject:" of an email—important but not the actual message content.

### heap fragmentation  
Occurs when memory on the **heap** is allocated and deallocated in such a way that it creates **small unusable gaps** between blocks.  
**Impact**: Reduces performance and can lead to memory errors.  
**Fixes**: Some garbage collectors compact memory to address this.

### heap memory  
A section of RAM used to store data that needs to **persist beyond a function call**, such as dynamically created objects.  
**Managed by**: The garbage collector in high-level languages.  
**Contrast with**: Stack memory, which is temporary and tied to function calls.  
**Analogy**: Heap memory is like long-term storage; stack memory is your work desk.

---

## I

### infected file upload  
A malicious file uploaded to a system that may contain **viruses, malware, or scripts** designed to exploit vulnerabilities.  
**Why it matters**: Uploaded files can be used to gain access, run unauthorized code, or extract sensitive data.  
**Best practices**:  
- Scan files for malware  
- Restrict file types  
- Store uploaded files outside the web root

### information disclosure through error messaging  
Occurs when error messages provide **too much internal detail**—like stack traces, server names, or database schemas.  
**Why it's dangerous**: Attackers can use this info to plan more effective attacks.  
**Fix**: Show **generic messages** to users; log detailed errors internally.

### inheritance  
An **object-oriented programming** concept where a class (child/subclass) **inherits** properties and behaviors from another class (parent/superclass).  
**Why it’s useful**: Promotes code reuse and establishes a hierarchical relationship.  
**Example**: A `Dog` class inheriting from an `Animal` class.

### inheritance vs. composition  
A key design choice in OOP:  
- **Inheritance**: "is-a" relationship (e.g., Dog is an Animal)  
- **Composition**: "has-a" relationship (e.g., Car has an Engine)  
**Rule of thumb**: Prefer **composition** for flexibility and modularity.

### initialization vector  
A **random or pseudorandom number** used with encryption algorithms to prevent pattern detection in encrypted data.  
**Why it’s needed**: Even if the same data is encrypted twice, the IV ensures different results.  
**Use case**: Common in symmetric encryption like AES.

### injection attack  
An attack where **untrusted input** is inserted into a program in a way that alters its intended behavior.  
**Examples**:  
- SQL Injection  
- Command Injection  
- LDAP Injection  
**Prevention**: Input validation, escaping, using parameterized queries.

### input validation issues  
Flaws that arise when a system does **not properly check** or sanitize input.  
**Results in**: Bugs, crashes, or vulnerabilities like XSS and injection attacks.  
**Tip**: Always validate input on both client and server sides.

### integration testing  
A testing level that checks how **different modules or components** of an application work together.  
**Focus**: Verifies **interactions** between units, not just individual ones.  
**Use case**: Making sure the payment processor talks to the inventory system correctly.

### interface (object-oriented)  
A contract or blueprint that defines **method signatures** a class must implement, but not their implementation.  
**Why it’s powerful**: Promotes **flexibility**, **polymorphism**, and decouples code.  
**Example**: A `Drivable` interface with a `startEngine()` method that both `Car` and `Motorcycle` classes implement.

### iteration pattern as language feature  
When a language **abstracts away** the manual creation of iterators with built-in syntax.  
**Examples**:  
- `for item in collection:` in Python  
- `for (let item of array)` in JavaScript  
- `for (String s : list)` in Java  
**Benefit**: Makes iterating through collections easy and readable.

### iterator design pattern  
A behavioral pattern that provides a standard way to **traverse through a collection** without exposing its internal structure.  
**Example**: Walking through an array, list, or tree one element at a time.  
**Used in**: Almost every language with loops or collections.

### iterator object  
The object that implements the **logic to traverse** an aggregate structure in the iterator design pattern.  
**Must include**:  
- `hasNext()` – Are there more elements?  
- `next()` – What’s the next element?  
**Used in**: Languages like Java, C#, Python, and JavaScript.

---

## J

### Java EE  
**Java Enterprise Edition**—a version of Java that provides tools and APIs for developing **enterprise-level applications**, including **web services, distributed computing**, and multi-tier architectures.  
**Use case**: Big apps like banking systems, inventory management, or any large-scale backend platform.  
**Includes**: JAX-RS, JPA, JMS, and more.

### JAX-WS  
**Java API for XML-Based Web Services**—a Java standard for building **SOAP-based web services**.  
**Why it matters**: Enables the creation and consumption of web services using XML as the data format.  
**Common use**: When working with legacy systems or enterprise-level APIs that still rely on SOAP.

### Jira  
A **project management and bug-tracking tool** used by development teams to manage tasks, sprints, user stories, and bugs.  
**Features**:  
- Ticket-based tracking  
- Integration with CI/CD pipelines  
- Dashboards, kanban boards, and burndown charts  
**Why it's everywhere**: It’s flexible, scalable, and popular in agile workflows.

### JSON  
**JavaScript Object Notation**—a lightweight, **human-readable** format used for **data interchange**.  
**Why it's great**:  
- Easy to read and write  
- Language-independent  
- The go-to format for **RESTful APIs**  
**Example**:  
```json
{
  "name": "Soft Boy King",
  "subscribers": 100,
  "pets": ["Peach", "Pearl"]
}
```

### JUnit  
The **standard unit testing framework for Java**, part of the **xUnit family** of test frameworks.  
**Why developers love it**:  
- Clean annotations (`@Test`, `@BeforeEach`)  
- Integrates easily with build tools (like Maven and Gradle)  
- Works great with IDEs and CI/CD tools  
**Use case**: Write and run tests during development to catch bugs early.

---

## K

### key (C language, database, or GraphQL)  
A **unique identifier** used to reference data, whether in memory or storage.  
**In databases**:  
- A **primary key** uniquely identifies each row.  
- A **foreign key** connects rows across tables.  
**In GraphQL**:  
- Keys help map fields and values in queries.  
**In C**:  
- Keys may refer to **hash map lookups** or **pointers to structures**.

### keyword (programming languages)  
A **reserved word** that has a special meaning in a programming language and **cannot be used** for variable names.  
**Examples**: `if`, `else`, `class`, `return`, `while`  
**Why it matters**: Keywords form the **syntax rules** of a language—they're the building blocks of structure and control flow.

### key-value pair  
A **pairing of data** where a **key** acts as a unique identifier and the **value** is the data associated with it.  
**Common in**:  
- **Dictionaries** (Python)  
- **Objects** (JavaScript)  
- **Maps** (Java)  
**Example**:  
```json
{
  "name": "Peach",
  "type": "dog"
}
```

---

## L

### language transparency  
The ability of systems—especially **web services**—to communicate across different programming languages using **common formats** like XML or JSON.  
**Why it matters**: A client written in Python can talk to a server written in Java with zero issues.  
**Example**: A REST API returns JSON. JavaScript, Python, and Ruby can all parse and use it.

### latency  
The time delay between a **client request** and the **server's response**.  
**Types**:  
- **Network latency**: How long the data takes to travel.  
- **Application latency**: Time taken to process the request.  
**Why it's important**: High latency = slower apps = frustrated users.

### latest result  
In a **test plan**, this refers to the **most recent outcome** of executing a test—pass, fail, or error.  
**Why track it**: Helps determine if a fix worked, if a bug re-emerged, or if your feature is still stable.  
**Good practice**: Keep a historical record for auditing and analysis.

### load testing  
A type of **performance testing** used to see how an application handles **expected user traffic**.  
**Goal**: Identify the maximum number of concurrent users or transactions the system can support without slowing down.  
**Example**: Simulate 1,000 users placing orders at once in an online store.

### log aggregation attack  
An attack where sensitive data is **accidentally logged** and later collected by someone with access to log files.  
**Example**: Logging full credit card numbers or passwords during error tracking.  
**Fix**:  
- Mask sensitive data  
- Limit access to logs  
- Sanitize what gets logged

### loose coupling (REST)  
A design philosophy where different parts of a system are **independent** and interact only through **well-defined interfaces**.  
**Why it matters**:  
- Makes systems easier to maintain and scale  
- Changes in one service won’t break others  
**Example**: A mobile app consumes a REST API—it doesn't care how the backend is implemented, just that the API works.

### loosely coupled (Observer pattern)  
A relationship where objects **know as little as possible** about each other.  
**Why it rocks**:  
- Promotes modularity  
- Makes code easier to test and extend  
**Example**: In the Observer pattern, the subject notifies observers without knowing their exact implementation.

---

## M

### main memory  
The **primary working memory** of a computer, also known as **RAM** (Random Access Memory).  
**What it does**: Temporarily stores data and instructions that the CPU actively uses.  
**Important note**: It's **volatile**—data disappears when the computer is shut down.  
**Analogy**: Like your short-term memory while you’re cooking—you hold info for the current recipe but forget it once you’re done.

### malloc (C language)  
Stands for **"memory allocation"**—a C function used to reserve a block of memory on the **heap**.  
**Syntax**:  
```c
int *ptr = malloc(sizeof(int) * 10);
```  
**Must-do**: Always pair it with `free()` to avoid memory leaks.

### man in the middle  
A type of **cyberattack** where a malicious actor secretly intercepts and possibly alters communication between two parties.  
**Example**: Someone on the same public Wi-Fi intercepts traffic between you and your bank.  
**Protection**: Encryption, TLS, and certificate pinning.

### manual memory management  
A system where **developers are responsible** for allocating and freeing memory.  
**Used in**: Languages like C and C++.  
**Why it’s risky**: Easy to forget to free memory or access it after it’s been freed (dangling pointer).

### manual testing  
Testing done **by a human**, following the steps a user might take in an application.  
**Why it’s useful**: Great for usability feedback and edge cases that automated tests might miss.  
**Drawbacks**: Time-consuming and not scalable for frequent checks.

### matcher  
In **Hamcrest** or similar assertion frameworks, a matcher is a **predicate or condition** used to test whether an actual value fits an expected pattern.  
**Example**:  
```java
assertThat(name, startsWith("Soft"));
```  
**Why it helps**: Improves readability of tests.

### Maven  
A **build automation and dependency management tool** for Java projects.  
**What it does**:  
- Builds and compiles code  
- Manages third-party libraries (dependencies)  
- Handles packaging and deployment  
**Bonus**: Uses an XML file called `pom.xml` to define project structure and plugins.

### memory allocation  
The act of **reserving memory** in RAM for program data.  
**Types**:  
- **Static**: Allocated at compile time  
- **Dynamic**: Allocated at runtime  
**Why it matters**: Efficient memory use keeps your program fast and prevents crashes.

### memory allocation, dynamic  
Memory allocated **at runtime** using tools like `malloc()` in C or automatically in high-level languages like Python.  
**Use case**: When the amount of memory needed isn’t known until the program is running.

### memory allocation, static  
Memory allocated **at compile time**, often for global or static variables.  
**Benefit**: Fast, because memory is ready at runtime.  
**Limitation**: Less flexible—must be known ahead of time.

### memory deallocation  
The process of **releasing memory** that is no longer needed.  
**Manual**: In C with `free()`  
**Automatic**: Via garbage collection in languages like Java or Python  
**Why it matters**: Prevents memory leaks and performance issues.

### memory, heap  
A section of memory for **dynamic allocation**, where values can persist beyond the scope of a single function call.  
**Used for**: Objects, large data structures, and anything created at runtime.  
**Managed by**: The programmer (in C) or garbage collector (in Java, Python).

### memory leak  
Occurs when a program **fails to release memory** it no longer needs, leading to reduced performance or crashes over time.  
**Example**: Forgetting to call `free()` in C, or holding unnecessary references in Java.  
**Fix**: Good memory hygiene, profiling, and garbage collection.

### memory management  
The practice of **allocating, using, and releasing memory** efficiently.  
**Why it matters**: Prevents crashes, improves speed, and ensures scalability.  
**Includes**:  
- Stack vs. Heap  
- Manual vs. Automatic memory management  
- Garbage collection and profiling

### memory management, automatic  
When a language handles memory cleanup **for you** using a garbage collector.  
**Languages**: Python, Java, JavaScript  
**Perks**: Reduces bugs and developer burden  
**Caveat**: You still need to avoid holding onto memory you no longer need.

### memory management, manual  
The programmer is responsible for **both allocation and deallocation** of memory.  
**Used in**: C, C++  
**Risk**: Forgetting cleanup leads to memory leaks and dangling pointers  
**Reward**: Full control and sometimes better performance.

### memory profiler  
A tool used to **track memory usage** while a program is running.  
**Use case**: Find memory leaks, excessive allocation, or bloated objects.  
**Examples**:  
- VisualVM (Java)  
- memory_profiler (Python)

### memory, stack  
Memory that stores **function-specific data**, like variables and return addresses.  
**Why it’s efficient**: Fast and automatically managed  
**Limit**: Limited size; leads to stack overflow if misused  
**Analogy**: Like a stack of plates—last in, first out.

### microservice  
A small, independent piece of an application that performs a **single business function** and communicates with other microservices over a network.  
**Why they’re great**:  
- Scalable  
- Easier to deploy and maintain  
- Can use different languages or frameworks per service  
**Downside**: Harder to manage without solid architecture and DevOps practices.

### mob testing session  
A time-boxed group activity where the **entire team tests** an application together.  
**Benefits**:  
- Multiple perspectives  
- Real-time feedback  
- Fun and collaborative  
**Recommended**: When testing complex features or during bug bashes.

### mock  
A **test double** that simulates the **behavior** of a real object without depending on its actual implementation.  
**Why use it**:  
- Isolate the system under test  
- Avoid slow or flaky dependencies  
**Example**: Mocking a network request to test UI behavior offline.

### mocking framework  
A library that helps you create, configure, and verify mocks.  
**Popular tools**: Mockito (Java), unittest.mock (Python), Jest (JavaScript)  
**Superpower**: Let you define expected calls, return values, and verify interactions.

### Mockito  
A **popular mocking framework for Java** that allows developers to easily create and verify mock objects.  
**Features**:  
- Simple syntax  
- Works with JUnit  
- Helps test interactions (Was the method called? With what arguments?)  
**Example**:  
```java
verify(myService).doSomething("Hello");
```

### multi-threading  
An approach where multiple **threads of execution** run concurrently within the same application.  
**Use case**: Parallel tasks like downloading files or handling multiple users.  
**Challenges**: Race conditions, deadlocks, and memory management complexity.  
**Supported in**: Java, Python (via `threading`), C++, and more.

### mutation (GraphQL)  
A **GraphQL operation** used to **change data** on the server—like creating, updating, or deleting records.  
**Example**:  
```graphql
mutation {
  updateUser(id: "123", name: "Soft") {
    name
    email
  }
}
```

---

## N

### next() method  
In the **Iterator design pattern**, `next()` is a method used to **retrieve the next element** in a sequence or collection.  
**Paired with**: `hasNext()`  
**Common in**:  
- Java: `Iterator.next()`  
- Python: `__next__()` in custom iterators  
**Example**:  
```java
while(iterator.hasNext()) {
    Item item = iterator.next();
}
```  
**Why it matters**: Enables flexible, controlled iteration without exposing the underlying data structure.

### nonce  
A **random or pseudorandom number** used only once in a cryptographic operation.  
**Purpose**: Prevents **replay attacks**, where a malicious actor tries to reuse valid data packets.  
**Use case**: Often paired with password hashing or token-based authentication.  
**Mnemonic**: "Number used ONCE."

### node (linked list or tree)  
A **single unit** in a data structure that holds a value and references to other nodes.  
**Types**:  
- In a **linked list**, it points to the next node.  
- In a **tree**, it may have children and a parent.  
**Why it matters**: Nodes are the building blocks of complex structures like graphs, trees, and lists.

### node, child  
In a **tree structure**, a **child node** is one that **descends from another node** (its parent).  
**Visualize**:  
```
        A (parent)
       / \
      B   C (children)
```

### node, leaf  
A **terminal node** in a tree that has **no children**.  
**Use case**:  
- In a file system tree, a file is a leaf node  
- In a decision tree, a final decision is at a leaf node

### node, parent  
A **node with one or more children**. It's the **origin point** for branches in a tree structure.  
**Fun fact**: The **root node** has no parent.

### node, root  
The **topmost node** in a tree—every other node descends from it.  
**Example**: In a company org chart, the CEO is the root node.

### node, sibling  
Two nodes that **share the same parent**.  
**Why it’s useful**: Understanding relationships between nodes helps when navigating or restructuring trees.

### non-deterministic algorithm  
An algorithm that may yield **different outputs for the same input** depending on factors like random choices or parallel execution.  
**Used in**:  
- AI  
- Heuristics  
- Cryptography  
**Example**: A genetic algorithm that evolves over time but doesn't always follow the same path.

### non-functional requirements  
Requirements that specify **how** a system performs rather than **what** it does.  
**Examples**:  
- Speed  
- Scalability  
- Security  
- Usability  
**Why it matters**: They ensure your app not only works but works **well** and consistently.

### normalization rules  
In databases, rules that organize data to **reduce redundancy** and **improve integrity**.  
**Levels**:  
- First Normal Form (1NF): No repeating groups  
- Second Normal Form (2NF): All non-key fields depend on the whole key  
- Third Normal Form (3NF): No transitive dependencies  
**Goal**: Make data clean, efficient, and easier to maintain.

### null  
A special marker used to signify that a **variable has no value or is empty**.  
**In databases**: A field marked as null means "no data here."  
**In code**: Can indicate missing, uninitialized, or optional values.  
**Careful**: Nulls can lead to **null pointer exceptions** or confusing bugs if not handled correctly.

--

## O

### observer design pattern  
A **behavioral design pattern** where one object (the **subject**) notifies all its **observers** when its state changes.  
**Why it matters**: Allows for **loose coupling**—the subject doesn’t need to know what the observers do.  
**Real-life analogy**: A YouTube channel (subject) has subscribers (observers) who get notified when a new video is uploaded.  
**Use case**: GUI frameworks, event handling, and pub/sub systems.

### on-the-wire attack  
An attack that occurs **during data transmission**, often exploiting unsecured channels.  
**Example**: Intercepting unencrypted login credentials sent over HTTP.  
**Prevention**: Use **TLS/SSL**, **encryption**, and **secure authentication tokens**.

### open-closed design principle  
Part of the **SOLID** design principles. It states:  
> “Software entities (classes, modules, functions) should be **open for extension** but **closed for modification**.”  
**Translation**: You should be able to add new functionality **without changing existing code**.  
**How**: Use **inheritance**, **interfaces**, or **composition** to extend behavior.  
**Why**: Reduces the risk of introducing bugs into stable, tested code.

### OpenAPI  
A **specification format** for describing RESTful APIs in a machine- and human-readable way.  
**Why it’s great**:  
- Helps automate client code generation  
- Supports API documentation tools (like Swagger UI)  
- Encourages consistency across teams  
**Bonus**: It’s **language-agnostic**—works with any tech stack.

### out of memory error  
Occurs when a program or system tries to allocate **more memory than is available**.  
**Causes**:  
- Memory leaks  
- Unbounded data growth  
- Infinite recursion  
**Fixes**:  
- Use memory profilers  
- Optimize data structures  
- Monitor runtime memory use

### OWASP  
**Open Worldwide Application Security Project**—a non-profit that produces resources for building secure software.  
**Famous for**:  
- The **OWASP Top 10**: A list of the most critical web security risks  
- Cheat sheets and testing guides  
**Why follow it**: Industry standard for secure development practices.  
**Fun fact**: You’ll see OWASP referenced in **code reviews, audits, and job interviews**.

---

## P

### partial failure  
A situation where **part of a system fails**, but the rest remains operational.  
**Example**: In a microservice architecture, one service might be down, but the others continue working.  
**Why it matters**: Apps should degrade **gracefully**—not crash entirely due to isolated issues.  
**Solution**: Use **fallbacks**, **circuit breakers**, or **retry logic**.

### password hashing algorithm  
A one-way function used to **securely store passwords**.  
**How it works**:  
- User password → hash (with optional salt)  
- Hash is stored, not the password  
- During login: input password is hashed again and compared  
**Common algorithms**: bcrypt, Argon2, PBKDF2  
**Important**: Never store plain-text passwords.

### pen test  
Short for **penetration test**—a simulated attack on a system to find vulnerabilities.  
**Goal**: See how a real-world attacker might exploit weak spots.  
**Often includes**:  
- Social engineering  
- Network scanning  
- Exploiting injection flaws  
**When to use**: Before product release or major updates.

### performance testing  
Testing to assess how well a system performs under load.  
**Checks for**:  
- Response time  
- Throughput  
- Resource usage  
**Types**:  
- Load testing (typical conditions)  
- Stress testing (extreme conditions)  
- Soak testing (long-term conditions)

### plan phase  
The first phase of the **SDLC (Software Development Life Cycle)**.  
**Focus**: Gather business requirements, define goals, and outline high-level features.  
**Why it's crucial**: A strong plan saves time later by preventing scope creep and misunderstandings.

### pointer (C language)  
A variable that stores the **memory address** of another variable.  
**Syntax**:  
```c
int *ptr = &value;
```  
**Powerful but dangerous**: Can lead to **segmentation faults**, **dangling pointers**, or **buffer overflows** if misused.  
**Use case**: Dynamic memory management, data structure implementation, passing by reference.

### POJO  
**Plain Old Java Object**—a simple Java class that doesn’t extend or depend on specialized libraries or frameworks.  
**Traits**:  
- Contains fields, getters/setters, maybe constructors  
- No annotations or inheritance from external tools  
**Why it matters**: Keeps things **simple and flexible**; easy to use with frameworks like Spring.

### polymorphism, replace conditional with  
A refactoring technique where **complex `if` or `switch` logic** is replaced with **object-oriented polymorphism**.  
**Example**:  
Instead of:
```java
if (type.equals("Dog")) { ... }
else if (type.equals("Cat")) { ... }
```
Use:
```java
Animal animal = getAnimal();
animal.makeSound();
```
Each subclass (Dog, Cat) has its own `makeSound()`.

### pool (Python)  
A **chunk of memory** in Python’s memory management system, used to optimize performance.  
**Structure**:  
- **Arenas** (large chunks) contain  
  - **Pools** (medium-sized blocks), which contain  
    - **Blocks** (individual objects)  
**Why it exists**: Memory reuse reduces fragmentation and speeds up allocation.

### POST operation (REST)  
A **RESTful HTTP method** used to **create new resources**.  
**Example**:  
```http
POST /users
{ "name": "Soft", "role": "Admin" }
```  
**Side effects**: Typically changes server state.  
**Idempotent?**: No. Calling it twice may create two different resources.

### Postman  
A tool for testing APIs by sending HTTP requests (GET, POST, PUT, DELETE) and inspecting responses.  
**Great for**:  
- Manual testing of endpoints  
- Mocking requests  
- Automating test collections  
**Bonus**: Visual interface makes it beginner-friendly.

### profiler, memory  
A tool that monitors **memory usage over time**, helping identify **leaks**, **inefficiencies**, or **hotspots**.  
**Examples**:  
- `memory_profiler` (Python)  
- VisualVM (Java)  
- Chrome DevTools (JavaScript)  
**Why it’s helpful**: Optimizes performance and prevents crashes.

### PUT operation (REST)  
A **RESTful method** used to **update** a resource or create it if it doesn't exist.  
**Key trait**: It’s **idempotent**—calling it multiple times won’t change the result.  
**Example**:  
```http
PUT /users/123
{ "name": "Soft", "role": "Dog Dad" }
```

---

## Q

### QA  
Short for **Quality Assurance**, QA is the process of ensuring that a product meets defined standards and functions as intended.  
**More than testing**: QA includes planning, documentation, and process management.  
**Goal**: Catch issues **before** they reach production.  
**Common tools**: Jira (for bug tracking), Selenium (for automated UI testing), Postman (for API testing)

### QA deliverables  
The **artifacts produced by QA** throughout the development cycle.  
**May include**:  
- Test plans  
- Test cases  
- Bug reports  
- Regression test reports  
- Test summary reports  
**Why they matter**: Help communicate what’s been tested, how thoroughly, and what the outcomes were.

### quality assurance  
A **systematic process** to ensure quality in software products.  
**Key activities**:  
- Writing and executing test cases  
- Verifying that features meet requirements  
- Logging and tracking bugs  
- Reviewing design and code for potential issues  
**Outcome**: Confidence that the product will work reliably and meet user needs.

### query document (GraphQL)  
In **GraphQL**, a query document is a string sent to the server describing **what data you want**.  
**Example**:
```graphql
{
  user(id: "123") {
    name
    email
  }
}
```  
**Note**: It’s **structured like JSON**, but it’s not JSON—just looks similar!

### query (GraphQL)  
The most common operation in GraphQL—used to **retrieve data** from a server.  
**Difference from REST**: Instead of multiple endpoints, GraphQL uses one endpoint with flexible queries.  
**Advantage**: Only fetch what you need—no more, no less.

---

## R

### rainbow table  
A **precomputed table** used to reverse cryptographic hash functions, often for cracking passwords.  
**How it works**: Instead of brute-forcing a password, attackers look up a hash value in a rainbow table to find the original password.  
**Defense**: Use **salting**—adding random data to passwords before hashing to make rainbow tables useless.

### RAM  
**Random-Access Memory**, the short-term memory of a computer.  
**Fast and volatile**: It clears when the system powers off.  
**Used for**:  
- Storing active programs  
- Holding runtime variables  
**Fun fact**: The more RAM, the more applications your computer can handle at once without slowing down.

### range-act-assert pattern  
A testing structure in **TDD** that organizes tests into three phases:  
1. **Arrange**: Set up test data and context  
2. **Act**: Run the method or action under test  
3. **Assert**: Verify that the result is as expected  
**Example (in Java)**:
```java
// Arrange
User user = new User("Soft", "Admin");

// Act
boolean result = user.hasPrivileges();

// Assert
assertTrue(result);
```

### realloc (C language)  
A C language function that **resizes** a previously allocated memory block.  
**Why it matters**: Allows programs to grow or shrink memory use dynamically without data loss.  
**Syntax**:  
```c
int* newPtr = realloc(oldPtr, newSize);
```

### red-green-refactor cycle  
A core part of **Test-Driven Development (TDD)**.  
1. **Red**: Write a test that fails  
2. **Green**: Write the minimal code needed to pass the test  
3. **Refactor**: Clean up the code while keeping the test passing  
**Why it rocks**: Encourages continuous improvement and safe experimentation.

### refactoring  
Changing the **internal structure** of code without changing its **external behavior**.  
**Why refactor?**  
- Improve readability  
- Reduce duplication  
- Make code easier to extend and maintain  
**Example**: Extracting logic from a long method into smaller, named methods.

### refactoring, extract function  
A specific refactoring method where you **pull out part of a method** into its own function.  
**Why?**  
- Improves readability  
- Makes code reusable  
- Supports clean design principles

### reference counter  
A mechanism used in **memory management** to track how many references exist to an object.  
**When the counter hits zero**, the object can safely be deleted or garbage collected.  
**Used in**:  
- Python’s memory management  
- Smart pointers in C++

### references, escaping  
When an object is accidentally **exposed to the wrong scope**, leading to unintended access or lifecycle issues.  
**Danger**: Can prevent garbage collection, causing **memory leaks**.  
**Watch for**: Returning internal objects directly or passing them to global contexts.

### replace conditional with polymorphism  
A **refactoring technique** used to replace complex `if/else` or `switch` statements with polymorphic method calls.  
**Benefit**: Cleaner, more extensible code.  
**Example**:
```java
// Instead of
if (shape == "circle") { drawCircle(); }
else if (shape == "square") { drawSquare(); }

// Use polymorphism
Shape shape = new Circle();
shape.draw();
```

### resolver (GraphQL)  
In GraphQL, a **function that provides the value** for a specific field in a query.  
**Example**:  
```javascript
const resolvers = {
  Query: {
    user: (parent, args, context) => getUserById(args.id)
  }
}
```
**Why it's cool**: Resolvers separate the schema (what data is requested) from the logic (how to get it).

### REST  
**Representational State Transfer**—a web architecture style for building APIs using standard HTTP methods.  
**Core operations**:  
- **GET**: Retrieve data  
- **POST**: Create data  
- **PUT**: Update data  
- **DELETE**: Remove data  
**Bonus**: REST is stateless—each request contains all the info needed.

### RESTful API  
An **API that follows REST principles**.  
**Traits**:  
- Resource-based  
- Uses HTTP verbs  
- Stateless communication  
**Example**:  
```http
GET /users/123
```

### risk register  
A document that **tracks potential risks**, including their likelihood, impact, and mitigation strategies.  
**Why it’s important**: Encourages proactive thinking and helps reduce the chance of surprises later.  
**Common in**: Security, compliance, DevSecOps, and enterprise planning.

### ROM  
**Read-Only Memory**—non-volatile memory used to store **firmware or startup code**.  
**Slower than RAM**, but it retains data even when the system is powered off.  
**Example**: BIOS code that starts your computer lives in ROM.

--

## S

### sad path scenario  
A scenario in which a system behaves **unexpectedly or returns an error**.  
**Example**: A user enters an invalid password or submits a form with missing required fields.  
**Why it matters**: Helps ensure graceful error handling and good user experience under failure conditions.

### salt  
**Random data** added to a password before hashing it, making it **unique and secure**.  
**Purpose**: Defeats rainbow table attacks and prevents attackers from knowing when two users have the same password.  
**Use case**:  
```plaintext
Password: "Soft123"  
Salt: "A93s!"  
Hash: hash("A93s!Soft123")
```

### sandboxing  
A method of **isolating a program** in its own environment so it can't affect other parts of the system.  
**Use case**: Run potentially unsafe code, like a browser extension, without letting it access your file system.

### scenario  
In testing, a **step-by-step description** of a specific situation or user interaction.  
**Includes**:  
- Preconditions  
- Inputs  
- Expected outputs  
**Used in**: Manual testing, automated scripts, and BDD (Behavior-Driven Development)

### schema (GraphQL)  
The **blueprint of your API** in GraphQL. It defines what queries can be made, what types exist, and how they relate.  
**Think of it as**: The contract between client and server.

### scope of testing  
Part of a **test strategy** that outlines **what will be tested**, **how**, and **who is responsible**.  
**Includes**:  
- Unit tests  
- Integration tests  
- UI tests  
- Performance tests  
**Why it matters**: Helps allocate time, tools, and effort efficiently.

### scripting attack  
A form of **code injection** where an attacker runs a script—often JavaScript—in someone else's browser.  
**Example**: Cross-site scripting (XSS)  
**Prevention**: Input validation, output encoding, and using secure frameworks.

### scrum  
A popular **Agile methodology** focused on iterative development, collaboration, and frequent delivery.  
**Key components**:  
- Sprints (typically 1-2 weeks)  
- Standups  
- Retrospectives  
**Roles**: Product Owner, Scrum Master, and Development Team

### SDLC (Software Development Life Cycle)  
A structured process that covers the **entire lifecycle of a software product**.  
**Phases**:  
- Plan  
- Define  
- Design  
- Build  
- Test  
- Deploy  
**Goal**: Deliver high-quality software efficiently and predictably.

### secondary storage  
Long-term data storage like **hard drives, SSDs, or USBs**.  
**Unlike RAM**, this data doesn’t disappear when the system shuts off.  
**Analogy**: Like your brain’s long-term memory.

### secret storage service  
A tool or service that **securely stores sensitive information**, like API keys or passwords.  
**Examples**:  
- AWS Secrets Manager  
- HashiCorp Vault  
- Kubernetes Secrets

### security testing  
Testing aimed at discovering **vulnerabilities and weaknesses** in a system.  
**Includes**:  
- Penetration testing  
- Static and dynamic analysis  
- Input validation testing  
**Goal**: Reduce risk and protect user data.

### selection set (GraphQL)  
The part of a GraphQL query that specifies **which fields you want returned**.  
**Example**:  
```graphql
{
  user {
    name
    email
  }
}
```

### server-side validation  
**Input validation performed on the server** before data is processed.  
**Critical**: Even if you validate on the client, the server must re-validate everything.  
**Why**: Client-side validation can be bypassed by malicious actors.

### service, denial of  
Short for **Denial of Service (DoS)**—an attack that **floods a server** with requests to make it unavailable.  
**Variants**:  
- DoS (single source)  
- DDoS (distributed attack)  
**Mitigation**: Firewalls, rate limiting, and traffic filtering

### session  
A server-side object used to **track a user’s state** during their visit to a website.  
**Why needed**: HTTP is stateless—sessions give users continuity.  
**Example**: Remembering that a user is logged in.

### session fixation attack  
An attack in which a **user is tricked into using a known session ID**, allowing the attacker to hijack the session.  
**Prevention**: Regenerate session tokens after login.

### session hijacking  
An attacker **steals a valid session ID** and uses it to impersonate a user.  
**Common causes**:  
- Unencrypted connections  
- XSS attacks  
**Fixes**: Use HTTPS, regenerate tokens often, set secure cookie flags.

### set up-test-tear down pattern  
A **TDD test structure** that includes three phases:  
1. **Set up**: Create necessary objects and data  
2. **Test**: Execute the behavior  
3. **Tear down**: Clean up or reset state  
**Why it matters**: Keeps tests isolated and repeatable.

### shallow copy  
A copy of an object’s **top-level properties**, but not nested objects.  
**Warning**: Changes to inner objects affect both the original and the copy.  
**Use case**: Okay for primitive or flat structures; risky for deep ones.

### single responsibility design principle  
Part of **SOLID** principles.  
> “A class should have only **one reason to change**.”  
**Why it helps**: Encourages **focused, maintainable** code.  
**Example**: One class handles user data; another handles authentication logic.

### soak testing  
A type of **performance testing** where a system is run at **normal load for an extended period**.  
**Purpose**: Uncover issues like memory leaks, database connection exhaustion, or slow degradation.

### SOAP  
**Simple Object Access Protocol**—a protocol for exchanging structured information in web services.  
**Uses**: XML messages, often with WSDL (Web Services Description Language)  
**Compared to REST**: Heavier, but sometimes necessary for enterprise-level security and transaction support.

### SoapUI  
A GUI tool for testing **SOAP (and REST)** APIs.  
**Useful for**:  
- Functional tests  
- Load testing  
- Security testing  
**Bonus**: You don’t need to write code to use it.

### source control  
Software that **tracks changes in code over time**.  
**Examples**: Git, Mercurial, Subversion  
**Why it’s essential**:  
- Enables collaboration  
- Prevents accidental loss  
- Supports branching, merging, and version history

### spoofing attack  
An attack where a bad actor **pretends to be someone else**—often by faking an IP address, MAC address, or login credentials.  
**Goal**: Trick systems or users into granting access.  
**Defense**: Multi-factor authentication, certificate validation, IP filtering

### spy  
In testing, a **test double** used to record information about how it was used.  
**Tracks**:  
- Method calls  
- Call counts  
- Passed arguments  
**Helpful for**: Verifying that something was invoked as expected.

### SQL injection  
A **code injection attack** that allows attackers to manipulate database queries.  
**Example**:
```sql
SELECT * FROM users WHERE username = 'admin' --'
```
**Result**: Bypasses authentication or reveals data.  
**Fix**: Use parameterized queries or ORM tools.

### SSL  
**Secure Sockets Layer**—a **deprecated** encryption protocol.  
**Replaced by**: TLS (Transport Layer Security).  
**Still used in name only**, like in "SSL certificates," which now use TLS under the hood.

### stack, call  
A data structure that tracks the **order of function calls**.  
**Example**: When a function calls another function, that call goes on top of the stack.  
**When the function returns**, it’s popped off.  
**Helps with**: Tracing, debugging, and recursion

### stack memory  
Memory used for **local variables and function calls**.  
**Fast and efficient**, but limited in size.  
**Overflowing the stack** (e.g. too many nested calls) causes a **stack overflow error**.

### stack overflow error  
Occurs when a program **exceeds the call stack’s limit**.  
**Common cause**: Infinite recursion.  
**Fix**: Use iterative methods or fix faulty recursion logic.

### stateless  
A system or server is **stateless** if it **doesn’t retain data between requests**.  
**REST APIs are stateless**—every request must contain all needed info.  
**Pros**: Simpler scaling and debugging.  
**Cons**: Requires passing more data around in each request.

### static analysis  
Examining **source code without executing it** to find errors, smells, or vulnerabilities.  
**Use tools like**: SonarQube, ESLint, FindBugs  
**Helps with**: Code quality, security, and maintainability

### static memory allocation  
Allocating memory **before** the program runs (at compile time).  
**Opposite of**: Dynamic allocation, which happens at runtime.  
**Use case**: C arrays with a known size

### strategy design pattern  
A **behavioral design pattern** where you define a family of algorithms and make them interchangeable.  
**Why?** So behavior can be selected at runtime without altering the client code.  
**Example**:  
```java
PaymentStrategy strategy = new CreditCardPayment();
strategy.pay(amount);
```

### stress testing  
A type of **performance testing** that pushes the system **beyond normal limits** to see how it breaks.  
**Goal**: Identify failure points and recovery mechanisms.

### stub  
A **test double** that returns hardcoded responses for test scenarios.  
**Used when** the real object is too complex, slow, or unavailable.  
**Helps with**: Isolating test subjects and creating predictable outcomes.

### subject object  
In the **Observer pattern**, the subject is the object being observed.  
**It owns the data** and notifies observers when changes occur.  
**Example**: A stock ticker notifying investors of price updates.

### subscription (GraphQL)  
A **GraphQL operation** that allows clients to **receive real-time updates** when data changes.  
**Requires**: WebSockets or another persistent connection.  
**Use case**: Chat apps, live dashboards, notifications

### sweeping  
Part of **garbage collection**, sweeping is the process of **removing objects** that are no longer in use.  
**Usually follows**: A “mark” phase, where live objects are identified.

---

## T

### TDD  
**Test-Driven Development**—a development method where tests are written **before** writing the functional code.  
**Cycle**:  
1. Write a failing test  
2. Write code to pass the test  
3. Refactor  
**Why use it?**  
- Encourages modular, clean code  
- Reduces bugs early  
- Acts as living documentation

### test-code-refactor  
The classic **three-step cycle** in TDD:  
- **Test**: Write a test that fails  
- **Code**: Make the test pass  
- **Refactor**: Improve the implementation  
**Rhythm of development**: Small steps that build trust in your codebase

### test double  
A **stand-in object** used during testing when the real object is unavailable or too complex.  
**Types**:  
- Dummy  
- Stub  
- Spy  
- Fake  
- Mock  
**Purpose**: Isolate the unit being tested.

### test-driven approach  
A mindset where **tests guide development** from start to finish.  
**Focus**: Business requirements, behavior, and correctness  
**Tools**: JUnit, PyTest, Mocha, etc.  
**Best for**: Critical systems, APIs, and code with long lifespans

### test fixture  
A **known, reusable state** set up for a test to run.  
**Example**:  
- A user account object  
- A pre-seeded database  
**Why it matters**: Makes tests repeatable and consistent

### test management  
Planning and controlling the **test process**.  
**Includes**:  
- Tool selection  
- Test environments  
- Data setup  
- Timeline planning  
**Goal**: Make sure testing is effective, efficient, and aligned with project goals.

### test phase  
The part of the **Software Development Life Cycle (SDLC)** where testing is the primary activity.  
**Usually includes**:  
- Unit tests  
- Integration tests  
- Performance tests  
- UAT (User Acceptance Testing)

### test plan  
A **documented plan** for testing a feature or application.  
**Includes**:  
- Scope  
- Resources  
- Schedule  
- Scenarios  
- Expected results

### test strategy  
A high-level **approach to testing** an entire product.  
**Describes**:  
- Tools used  
- Responsibilities  
- Types of tests  
- QA deliverables  
**Why important?** Aligns team on expectations.

### testing, black box  
Testing the **functionality** of a system without knowing the internal logic.  
**Think**: Inputs → Outputs  
**Used for**: Acceptance testing, user testing

### testing, box  
A **category of testing styles** based on knowledge of internals.  
**Types**:  
- White box  
- Black box  
- Gray box

### testing, endurance  
A type of **performance testing** where a system runs under normal conditions for a long time.  
**Goal**: Uncover issues like memory leaks or gradual degradation.

### testing, gray box  
Testing with **partial knowledge** of the system internals.  
**Example**: Testing APIs while knowing internal validation rules.  
**Great for**: Integration and security testing

### testing, integration  
Checks if **components work together** as expected.  
**Example**: Testing how your backend and database interact  
**Middle ground** between unit testing and system testing

### testing, load  
A performance test where the system is subjected to **expected levels of concurrent usage**.  
**Goal**: Find bottlenecks before real users do  
**Tool examples**: JMeter, Locust, Gatling

### testing, manual  
Testing performed by a **human following test steps**.  
**Best for**: Exploratory testing, UI reviews, or one-off scenarios

### testing, performance  
Covers **how well** a system performs under various conditions:  
- Load testing  
- Stress testing  
- Soak testing  
**Measured by**: Response time, throughput, resource usage

### testing, scope of  
The defined **boundaries** of what will and won’t be tested in a project.  
**Clarifies**:  
- Responsibilities  
- Priorities  
- Tools  
- Depth of testing

### testing, security  
Finding **vulnerabilities and weaknesses** in an app’s defenses.  
**Includes**:  
- Penetration testing  
- Fuzzing  
- Static and dynamic code analysis

### testing, soak  
Also called **endurance testing**—this tests a system’s long-term stability under a normal load.  
**Purpose**: Detect memory leaks, unclosed connections, or performance drops over time

### testing, stress  
Pushes the system **beyond expected limits** to see where it fails.  
**Goal**: Ensure that it fails gracefully and not catastrophically

### testing, UI automation  
Testing the **user interface** using scripts and tools instead of manual clicks.  
**Tools**: Selenium, Cypress, Playwright  
**Benefits**: Fast, repeatable, scalable regression tests

### testing, white box  
Also called **clear box testing**—tests the **internal logic** of a system.  
**Best for**: Unit tests, logic verification, coverage analysis

### text segment (C language)  
Part of memory where **compiled code (machine instructions)** are stored.  
**Read-only** in most systems  
**Contrast with**: Data segment (variables), Stack (function calls), Heap (dynamic data)

### then  
Used in **acceptance criteria** and BDD (Behavior-Driven Development) to describe the **expected outcome** of a scenario.  
**Structure**:  
- **Given** some context  
- **When** an action occurs  
- **Then** something should happen

### thread  
A **lightweight process**—a unit of execution within a program.  
**Each thread has its own stack** but shares memory with other threads.  
**Used in**: Concurrency and parallel processing

### TLS  
**Transport Layer Security**—the modern standard for **encrypting communication over networks**.  
**Replaces**: SSL  
**Used in**: HTTPS, email encryption, VPNs  
**Ensures**:  
- Data confidentiality  
- Integrity  
- Authentication

### token  
A **unique identifier** generated during login or authentication.  
**Used for**:  
- Session tracking  
- API authorization (e.g., JWT)  
**Important**: Keep tokens secure—they grant access!

### top-down approach  
A **design strategy** that starts with the big picture and breaks it into smaller components.  
**Contrast with**: Bottom-up, which builds smaller parts first  
**Used in**: Software architecture, API design, TDD planning

### triage, bug  
The process of **classifying bugs** by severity and priority.  
**Answers**:  
- How bad is it?  
- How soon should we fix it?  
**Helps**: Keep focus on what matters most.

### Truth  
A **third-party assertion framework** (from Google) used in Java for writing test validations.  
**Readable and expressive**:  
```java
assertThat(myList).contains("Soft");
```

### two-way certificate pinning  
A **security technique** where both the **client and server** authenticate each other using certificates.  
**Purpose**: Prevent man-in-the-middle attacks  
**Common in**: Banking apps, enterprise systems

### type-specific assertions  
Assertions **tailored to a specific data type**.  
**Examples**:  
- Strings: `startsWith()`, `contains()`  
- Lists: `hasSize()`, `containsExactly()`  

---

## U

### UI automation testing  
Testing the **user interface (UI)** of an application using **automated scripts** instead of manual interactions.  
**Why it's useful**:  
- Repeats tests quickly  
- Catches regressions early  
- Frees up humans to do exploratory testing  
**Tools**: Selenium, Cypress, Playwright  
**Example**: Automatically clicking buttons, filling forms, or checking that elements appear on the screen.

### unit test  
A test that checks a **single, isolated piece of code**, usually a function or method.  
**Why it matters**:  
- Fast and reliable  
- Catches bugs at the source  
- Encourages modular design  
**TDD loves unit tests!** They’re the building blocks of trustworthy software.

### unit testing  
The practice of writing and running **unit tests**.  
**Usually done with**:  
- Frameworks like JUnit (Java), PyTest (Python), or Mocha (JavaScript)  
**Focus**: One “unit” of logic, not interactions between components  
**Bonus**: Often runs in milliseconds—great for fast feedback loops.

### update method  
In the **Observer design pattern**, the `update()` method is what gets called on all observers when the subject changes.  
**Think of it like**:  
> "Hey, something changed—do your thing!"  
**Used in**: Real-time systems, UI frameworks, subscription models.

### URI  
**Uniform Resource Identifier**—a generic way to **name or locate resources** on the internet.  
**Example**:  
- `https://example.com/products`  
- `mailto:soft@example.com`  
**URI vs URL**: Every URL is a URI, but not all URIs are URLs.

### use case  
An **informal, user-focused description** of a system’s behavior.  
**Tells the story of**:  
- What a user wants to do  
- How the system helps them do it  
**Structure**: Often uses steps, actors, preconditions, and outcomes  
**Great for**: Building empathy with users during feature planning

### user persona  
A **fictional character** that represents a real user type.  
**Includes**:  
- Name  
- Demographics  
- Goals  
- Frustrations  
**Purpose**: Help teams **design for real needs**, not just assumptions  
**Example**: “Alex, 32, security analyst, values privacy, hates clunky interfaces.”

### user story  
A **short description** of a feature told from the perspective of the end user.  
**Format**:  
> "As a [type of user], I want [some goal] so that [some reason]."  
**Why it matters**: Keeps development focused on what users truly need  
**Bonus**: Often paired with **acceptance criteria** to define when it’s “done.”

---

## V

### virtual memory  
A technique that lets a system **pretend it has more RAM than it actually does** by temporarily storing data on disk.  
**How it works**: When your computer runs out of physical RAM, it moves inactive chunks of memory to a file on the hard drive (called a "page file" or "swap space").  
**Why it's important**:  
- Keeps applications running even when RAM is full  
- Makes multitasking smoother  
**Downside**: Slower performance when relying heavily on virtual memory

### variable, static  
A **class-level variable** that is shared across all instances of a class.  
**In Java**: `static int counter;` means `counter` is the same for every instance.  
**Why it's used**:  
- Shared counters  
- Configuration constants  
- Utility methods  
**Bonus**: You can access static variables without creating an object of the class.

### visibility  
Refers to **who can access a variable or method** in object-oriented programming.  
**Common levels**:  
- `public`: Accessible from anywhere  
- `private`: Only within the same class  
- `protected`: Within the same class and subclasses  
**Why it matters**: Helps enforce **encapsulation**, keeping the internal workings of a class private and safe from accidental changes

---

## W

### waterfall  
A traditional, **linear software development model** where each phase flows into the next like a waterfall.  
**Phases**: Requirements → Design → Implementation → Testing → Deployment → Maintenance  
**Pros**:  
- Easy to manage  
- Clear milestones  
**Cons**:  
- Rigid  
- Difficult to adapt once underway  
**Best for**: Projects with very clear, unchanging requirements

### web service  
A **software system designed for interoperable machine-to-machine interaction** over a network.  
**How it works**: It exposes functions that other programs can call using standard web protocols like HTTP or SOAP.  
**Example**: A weather web service that returns today’s forecast when called from a mobile app.  
**Formats**: XML, JSON  
**Common types**: RESTful APIs, SOAP-based services

### when  
A keyword used in **acceptance criteria** and **BDD-style testing** to indicate the action or trigger.  
**Structure**:  
- **Given** a condition  
- **When** an action occurs  
- **Then** an outcome should result  
**Example**:  
> When a user submits the form, they should see a confirmation message.

### white box testing  
Testing that **focuses on the internal structure** or logic of an application.  
**You know**: How the code is written, which functions do what, and where the risks lie.  
**Used for**:  
- Unit testing  
- Coverage analysis  
- Debugging logic  
**Contrast with**: Black box testing (which focuses only on input/output)

### whitelisting  
An input validation technique where only **known good input** is allowed.  
**Safer than blacklisting** (which tries to filter out bad input).  
**Example**: Allowing only letters and numbers in usernames  
**Used for**:  
- Preventing injection attacks  
- Controlling access to features or files  
- Ensuring data integrity

### WSDL  
**Web Services Description Language**—an XML-based format for **describing the interface of a SOAP web service**.  
**What it includes**:  
- What operations are available  
- What data types they use  
- Where the service lives (its endpoint)  
**Think of it as**: A contract between the service provider and consumer

---

## X

### XSS  
**Cross-Site Scripting (XSS)** is a **security vulnerability** where an attacker injects malicious scripts into trusted websites.  
**How it works**:  
- The attacker inserts JavaScript or other executable code into a form field or URL  
- The server doesn’t sanitize it properly  
- Other users unknowingly run that script when viewing the page  
**Impact**:  
- Stolen cookies and session tokens  
- Defaced websites  
- Hijacked user interactions  
**Defense**:  
- Proper input sanitization and output encoding  
- Content Security Policy (CSP) headers  
**Variants**:  
- Stored XSS (persisted in the database)  
- Reflected XSS (via a URL)  
- DOM-based XSS (manipulates the page in the browser)

### xUnit  
A family of **unit testing frameworks** for different programming languages, all based on a shared architecture and philosophy.  
**Examples**:  
- JUnit (Java)  
- NUnit (.NET)  
- PyTest or unittest (Python)  
- Mocha (JavaScript)  
**Why it's awesome**:  
- Consistent test structures  
- Built-in assertions  
- Supported by most IDEs and CI tools  
**Structure**: Arrange → Act → Assert

---

## Z

### zero-day  
A **zero-day vulnerability** is a **security flaw that’s unknown to the software vendor** and has no fix at the time it's discovered.  
**Why it’s dangerous**:  
- Exploited before anyone even knows it's a risk  
- Often sold on black markets or used in targeted attacks  
- Leaves systems completely defenseless  
**Name origin**: Developers have had **zero days** to address the issue  
**Defense tips**:  
- Keep systems updated  
- Use behavior-based threat detection  
- Apply defense-in-depth (multiple layers of security)

