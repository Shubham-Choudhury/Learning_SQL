# **WHAT IS RELATIONAL DATABASE**

A relational database management system or RDBMS is a database system that stores and and fetches data in the form of tables. Thus the data is stored in the form of rows and columns. DBMS such as My-SQL and ORACLE are based on the principle of relational DBMS.

# **HOW DOES A RELATIONAL DATABASE WORK**

Relational Databases use tables to store data about related objects. Each column contains data attributes, whereas each row holds a record of unique data known as key.

Realational Database or RDBMS are managed using SQL short form for Structured Query Language. Therefore SQL codes are used to retrieve information from relational databases by doing various interactive operations like JOIN, TRUNCATE etc.

# **WHAT IS THE STRUCTURE OF A RELATIONAL DATABASE MODEL?**

A relational database model represents how data is stored in tables, which helps from relations between data values.

Consider a relational table named EMPLOYEE with attributes EMP_ID, NAME, SALARY, AGE.

<table>
    <thead>
        <tr>
            <th>EMP_ID</th>
            <th>NAME</th>
            <th>SALARY</th>
            <th>AGE</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td>Shubham</td>
            <td>50000</td>
            <td>21</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Dipta</td>
            <td>60000</td>
            <td>19</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Ananya</td>
            <td>37000</td>
            <td>17</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Priti</td>
            <td>45000</td>
            <td>23</td>
        </tr>
    </tbody>
</table>


### **There are some important terminologies that you should keep in mide while forming a relational database.**
<br>

**Attribute:** Attributes are properties that define the relational database. Eg: EMP_ID, NAME etc.

**Tuple:** A tuple is a set of attributes that uniquely identifies a record in a table. Eg: (1, Shubham, 50000, 21)

**Relation Schema:** A relational schema defines its relation with other attributes altogether. Eg: EMPLOYEE(EMP_ID, NAME, SALARY, AGE).

**Degree:** Degree is defined by several attributes we have in a relational table. Eg: The degree of the EMPLOYEE table is 4.

**Cardinality:** Cardinality is defined by the number of tuples in a table. Eg: The cardinality of the EMPLOYEE table is 4.

**NULL Values:** The values or data which are unknown are kept as NULL.
<br>
<br>

# **ADVANTAGES OF RELATIONAL DATABASES**

* **Security:** Provides the functionality to restrict access to some tables to specific users.

* **Simplicity:** A relational database model is much simpler as compared to other network models.

* **Speed:** The speed is higher due to its simplicity and ease.

* **Accuracy:** Relational databases use foreign and primary keys to make tables interrelated.

* **Accessibility:** Relational databases do not require any specific path to access data.

* **Multi-User:** Relational databases can be accessed by multiple users simultaneous.

# **FLAT FILE DATABASE vs RELATIONAL DATABASE**

<table>
    <thead>
        <tr>
            <th>FLAT FILE DATABASE</th>
            <th>RELATIONAL DATABASE</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Flat file databases cannot incorporate multiple tables.</td>
            <td>Relational databases supports multiple tables</td>
        </tr>
        <tr>
            <td>The data is stored int the form of plain text.</td>
            <td>The data is stored in the form of tables, and there exists an interrelation between the tables.</td>
        </tr>
    </tbody>
</table>
