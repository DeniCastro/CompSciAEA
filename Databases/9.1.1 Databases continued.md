
# Relational Databases & Keys

##  What Is a Relational Database?

A **Relational Database** is a type of database that organises data into **multiple related tables**. Instead of storing all information in one big table (which can get repetitive and inefficient), data is split into **smaller, related tables**, which can be linked together through **relationships**.

This model helps:
- Avoid data duplication
- Improve data integrity
- Make data easier to update and maintain

---

##  Primary Key

A **Primary Key** is a field (or combination of fields) that uniquely identifies each record in a table.

### Example: `Students` Table

| StudentID | FirstName | LastName | DateOfBirth |
|-----------|-----------|----------|-------------|
| 1         | Alice     | Johnson  | 2005-04-21  |
| 2         | Bob       | Smith    | 2006-08-15  |

- The `StudentID` field is the **primary key**.
- Each student has a unique ID – no duplicates allowed.

---

##  Relationships Between Tables

In a relational database, **tables are connected using relationships**. The three main types are:

| Relationship Type | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| One-to-One        | One record in Table A matches one record in Table B                        |
| One-to-Many       | One record in Table A matches many records in Table B                     |
| Many-to-Many      | Many records in Table A match many in Table B (usually via a linking table) |

### Example: One-to-Many

Let’s say one student can enrol in **multiple courses**.

**Table: `Students`**

| StudentID | Name   |
|-----------|--------|
| 1         | Alice  |
| 2         | Bob    |

**Table: `Courses`**

| CourseID | CourseName     |
|----------|----------------|
| 101      | Maths          |
| 102      | History        |

**Table: `Enrolments`**

| EnrolmentID | StudentID | CourseID |
|-------------|-----------|----------|
| 1           | 1         | 101      |
| 2           | 1         | 102      |
| 3           | 2         | 101      |

In this case:
- `Enrolments` connects `Students` and `Courses`.
- One student (`StudentID`) can be related to many courses.
- One course (`CourseID`) can also relate to many students.

---

##  Foreign Key

A **Foreign Key** is a field in one table that refers to the **primary key** in another table. It helps enforce **referential integrity** (ensuring that linked records actually exist).

### Example:

In the `Enrolments` table above:
- `StudentID` is a **foreign key** referencing the `Students` table.
- `CourseID` is a **foreign key** referencing the `Courses` table.

---

##  Summary

- **Relational Databases** break down information into connected tables.
- A **Primary Key** uniquely identifies each record in a table.
- **Relationships** allow tables to connect meaningfully: One-to-One, One-to-Many, or Many-to-Many.
- **Foreign Keys** are used to reference records from another table.

---
