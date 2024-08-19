# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > it is used to import the servers controlers models and repository

02. What is the difference between a `class` and an `interface`?

  > class determines the properties while interface just uses the properties

03. What is the method that returns an instance of a class, yet it has no return type?

  > abstract

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > abstract (it will be usable on any classes that extend the cars class publicly)

06. In the Car example what is `string` an indication of?

  >the return type

07. In the Car example what is `abstract` preventing?

  > you cannot create an instance of the class you can only extend the class

08. In a SQL table, what is the difference between information in a row and information in a column?

  >  collumns are the name of what will be stored  rows are the actual data

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > Create table characters(
    id INT not NULL PRIMARY KEY AUTO_INCREMENT,
    name varchar(255) not null,
    age smallint not null,
    description string not nul
  )

10. In SQL how can you query more than a single table? Provide an example.

  > select from
    characters.*,
    movies.*
