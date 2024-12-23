
# Database Management System in Bash

## Overview
This Bash-based Database Management System (DBMS) allows users to create, list, update, select, delete, and manage tables within a database. The system simulates a simple file-based database where data is stored in text files. The system uses various Bash scripts to handle different database and table operations.

## Features
- **Create Database**: Create a new database directory.
- **Drop Database**: Delete an existing database.
- **List Databases**: List all available databases.
- **Connect to Database**: Connect to a selected database to perform operations.
- **Create Table**: Define and create tables within a connected database.
- **Drop Table**: Delete an existing table from a database.
- **List Tables**: List all tables within the selected database.
- **Select from Table**: Retrieve and display data from a table.
- **Insert into Table**: Add new records to a table.
- **Update Table**: Modify existing records in a table.
- **Delete from Table**: Remove records from a table.

## User Experience
Colors are used to enhance the user experience:
- **Yellow**: Warnings and invalid inputs.
- **Blue**: Information and general output.
- **Green**: Success messages.
- **Magenta**: Highlighted and important information.
- **Gray**: Data output.

## Entry Point
The entry point of the system is the **MainMenu** function, where users can select various operations to manage databases and tables.

## Database Operations

### 1. Create Database
To create a new database, the user selects the **Create Database** option from the main menu. The system will ask for the database name and create a new directory for it.

```bash
create_database
```

### 2. Drop Database
The **Drop Database** option allows users to delete an existing database. Once a database is dropped, all of its contents are permanently removed.

```bash
drop_database
```

### 3. List Databases
The **List Databases** option will list all available databases.

```bash
list_databases
```

### 4. Connect to Database
The user can **connect to a database** by selecting it from the list. Once connected, the system will allow the user to perform operations on that database.

```bash
connect_to_database
```

## Table Operations

### 1. Create Table
Tables can be created within the selected database. The user provides a table name and column definitions, including column names and data types (e.g., int, string).

```bash
create_table
```

### 2. Drop Table
Tables can be dropped from the selected database, deleting both the table data and its metadata.

```bash
drop_table
```

### 3. List Tables
This option lists all the tables in the currently connected database.

```bash
listTables
```

### 4. Select from Table
Users can select and view data from a table. The system allows the user to view all rows or search for rows by specific column values.

```bash
select_from_table
```

### 5. Insert into Table
New records can be inserted into a table using the **Insert into Table** option.

```bash
insert_into_table
```

### 6. Update Table
Existing records can be updated based on specific filter conditions. Users provide the column and value to be updated.

```bash
update_table
```

### 7. Delete from Table
Users can delete rows from a table by specifying a filter condition.

```bash
delete_from_table
```

## Code Structure
The code is divided into several components:

1. **MainMenu**: The entry point of the system where users can choose database and table operations.
2. **Database Operations**: Functions for creating, dropping, listing, and connecting to databases.
3. **Table Operations**: Functions for creating, listing, selecting, inserting, updating, and deleting tables.
4. **Validations**: Functions to validate inputs such as database names, table names, column names, and data types.

## Example
When you start the system, you will be greeted with a menu:

```bash
-- -- -- -- Welcome to Your DB -- -- -- --
>> Choose an option:
1) Create Database
2) List Databases
3) Exit
```

After selecting an option, the system will guide you through the steps, providing feedback through color-coded messages.

## Conclusion
This Bash-based DBMS provides a simple and lightweight way to simulate database management in a shell environment. It supports the basic operations required for managing databases and tables, with an emphasis on ease of use and a clean user interface.
