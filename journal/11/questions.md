# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | Allows classes to extend or modify already existing classes |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | It allows a class to add members to other classes  |

3. How does ***accessibility*** affect inheritance?

  > | Effects weather other classes can access members in that class. |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | A primary key is the id of the object itself, while a foreign key is the id of another object your trying to attach to |

5. What is an ***alias***?

  > | Allows you to rename a namespace |

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

  > | ANSWER HERE |
