# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | let, const, var |

02. What is the definition of a function?

    > | Something that we can call in JavaScript in order to accomplish a task, usually a small one. |

03. What are the `SOLID` principles?

    > | - Single Responsibility
        - Open closed Principle
        - Liskov Substitution
        - Interface Segregation
        - Dependency Inversion  |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | fruit = fruit.filter(f => f !== 'pineapple') |

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

    > | function themFriendListAdd(){
        them.friends.push(you)
    }
    function youFriendListAdd(){
        them.friends.push(them)
    } |

06. Give an example of a JavaScript `Conditional`:

    > | if(object.property) {        <-this would mean; if this property is true, then do whatever we put in the curly braces
    
    }
    |

07. What is the main difference between `parameters` and `arguments`?

    > | A parameter is like a placeholder for the argument that we are going to pass in, once we've been given that information, while an argument is usually given to us from our index |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > |  Putting the word debug in the first line of your function, this will allow the computer to run through every line of code in that function to show the developer what the logic is in real time.|

09. What is the difference between a `primitive` value and a `reference` value?

    > | A primitive value is a variable that is declared and has some sort of value of data, of any othe types that are associated with JS, while a reference value is attached to an object. |

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for(i = -100, i ) |
