# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | let, var, const |

02. What is the definition of a function?

    > | a set of instructions to be acted on when told to |

03. What are the `SOLID` principles?

    > | a set of guidelines that make the code more maintainable |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | fruit[2] |

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > |let nameOne = you.find(your => your.name) |
    let nameTwo = them.find(their => theirName)
    nameOne = them.friends
    nameTwo = you.friends

06. Give an example of a JavaScript `Conditional`:

    > | if(hats > 0){
        let heads = hats
        console.log(heads)
    } |

07. What is the main difference between `parameters` and `arguments`?

    > | parameters are the definition created within a functions ().
    arguments are the value a parameter receives from the html |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | use the debug tool in visual code |

09. What is the difference between a `primitive` value and a `reference` value?

    > | A data type built into javascript that isnt an object and has no methods or properties |

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for(let i = -100; i > 100) {
        console.log(i)
    }
