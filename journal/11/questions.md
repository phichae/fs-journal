# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | It allows us to use classes inside of other classes like ControllerBase inside of the controllers. |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | It depends on the accessibility of the member in that class, if it's set to private, it is not directly accessible. |

3. How does ***accessibility*** affect inheritance?

  > | Private members are inaccessible from a derived class directly. |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | A primary key is the "main" column that SQL will use to reference records in the table. Foreign key is when SQL attaches a column from a different Table to use to reference the data in that table.|

5. What is an ***alias***?

  > | A different name for a table that the developer can specify in their SQL query. |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > | 
    SELECT
    *
    FROM patient_doctors pd
    JOIN patients p ON pd.patientId = p.id
    JOIN doctors d ON pd.doctorId = d.id
    WHERE d.id = @doctorId
    |
