# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > to organize like processes

02. What is the difference between a `class` and an `interface`?

  > classes can pass functions to one another and implement values while interfaces can only be ran 

03. What is the method that returns an instance of a class, yet it has no return type?

  > void

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

  > public

06. In the Car example what is `string` an indication of?

  > return type

07. In the Car example what is `abstract` preventing?

  > preventing another class from accessing the function

08. In a SQL table, what is the difference between information in a row and information in a column?

  > information in a row is specific to one object while information in a column is specific to one property

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE characters(
    id INT AUTO_INCREMENT PRIMARY KEY NOT NULL,
    name VARCHAR(255),
    age VARCHAR(255),
    description VARCHAR(255)
  )

10. In SQL how can you query more than a single table? Provide an example.

  > SELECT *
    FROM accounts
    JOIN objects ON object.creatorId = account.id
    WHERE account.id = '1'
