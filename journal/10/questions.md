# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | To label areas of your code space |

02. What is the difference between a `class` and an `interface`?

  > | An interface defines what a class can be |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | Void |

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  

  > | string |

06. In the Car example what is `string` an indication of?

  > | the return type |

07. In the Car example what is `abstract` preventing?

  > | ANSWER HERE |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | a column is a key while a row is the whole object |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | CREATE TABLE characters 
  name NOT NULL
  age NOT NULL
  description NOT NULL |

10. In SQL how can you query more than a single table? Provide an example.

  > | SELEct
      characters.*,
      dogs,*
