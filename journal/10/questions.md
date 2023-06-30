# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | To give your program the ability to reference and utilize different classes from different files. |

02. What is the difference between a `class` and an `interface`?

  > | An interface cannot implement the methods it defines, however a class can use both the methods it defines and the ones defined in an interface. |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | private readonly |

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

  > | Public |

06. In the Car example what is `string` an indication of?

  > | Data type |

07. In the Car example what is `abstract` preventing?

  > | It's hiding the internal details of the class and it will only show the functionality |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | Information in a column is all the same 'key', where values in that column all correspond to that key. Information in a row has all different keys, but correspond to one instance. |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | 
    CREATE TABLE characters(
      name STRING NOT NULL,
      age STRING NOT NULL,
      description STRING NOT NULL,
      id INT NOT NULL AUTO_INCREMENT PRIMARY KEY
    )
   |

10. In SQL how can you query more than a single table? Provide an example.

  > | You can query multiple tables by joining them. For instance, if you had a table 'characters', and for each character there was a costume in the 'costumes' table:
  SELECT *
  FROM characters char
  JOIN costumes cost
    ON char.id = cost.id
   |
