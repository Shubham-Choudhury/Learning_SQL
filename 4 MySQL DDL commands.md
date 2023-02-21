# **MYSQL CREATE TABLE STATEMENT**

The `CREATE TABLE` statement is used to create a new table in a database.

    CREATE TABLE table_name (
        column1 datatype,
        column2 datatype,
        column3 datatype,
       ....
    );

- The `column` parameters specify the names of the columns of the table.

- The `datatype` parameter specifies the type of data that can be stored in each column.

        CREATE TABLE students(
            roll_no BIGINT PRIMARY KEY,
            `name` VARCHAR(50),
            age int,
            gender CHAR(1),
            hobbies VARCHAR(50)
        );

# **MYSQL TRUNCATE TABLE**

The `TRUNCATE TABLE` statement is used to delete all the records from a table, including all spaces allocated for the records are removed.

    TRUNCATE TABLE table_name;

# **MYSQL DROP TABLE**

The `DROP TABLE` statement is used to delete an existing table.

    DROP TABLE table_name;

# **MYSQL ALTER TABLE STATEMENT**

MySQL `ALTER` statement is used when you want to change the name of your table or any table field. It is also used to add or delete an existing column in a table.

The `ALTER` statement is always used with `ADD`, `DROP` and `MODIFY` commands according to the situation.

### **ADD A COLUMN IN THE TABLE**

Syntax:

    ALTER TABLE table_name
    ADD new_column column_definition
    [FIRST | AFTER column_name];

#### **PARAMETERS**

- `table_name` - The name of the table in which you want to add a column.

- `new_column` - The name of the new column that you want to add.

- `column_definition` - The definition of the new column that you want to add.

- `FIRST | AFTER column_name` - It is optional. It tells MySQL where in the table to create the column. If this parameter is not specified, the new column willbe added to the end of the table.


        ALTER TABLE students
        ADD COLUMN hometown VARCHAR(10)
        AFTER age;

        ALTER TABLE students
        ADD COLUMN(
            contact VARCHAR(10),
            address VARCHAR(30)
        );

### **MODIFY COLUMN IN THE TABLE**

The `MODIFY` command is used to change the column defination of the table.

Syntax:

    ALTER TABLE table_name
    MODIFY column_name column_definition
    [FIRST | AFTER column_name];

#

        ALTER TABLE students
        MODIFY age INT(3);

### **RENAME COLUMN IN TABLE**

The `CHANGE` command is used to change the name of the column in the table.

Syntax:

    ALTER TABLE table_name
    CHANGE old_column_name new_column_name column_definition
    [FIRST | AFTER column_name];

#

        ALTER TABLE students
        CHANGE contact student_contact VARCHAR(10)
        AFTER address;

### **RENAME TABLE NAME**

The `RENAME` command is used to change the name of the table.

Syntax:

    ALTER TABLE table_name
    RENAME TO new_table_name;

#

        ALTER TABLE students
        RENAME TO student_details;


### **DROP COLUMN IN TABLE**

The `DROP` command is used to delete the column from the table.

Syntax:

    ALTER TABLE table_name
    DROP COLUMN column_name;

#

        ALTER TABLE student_details
        DROP COLUMN hobbies;





