# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > var, let, const

02. What is the definition of a function?

    > a program that can be called within your program

03. What are the `SOLID` principles?

    > Single-responsibility Principle, Open-closed Principle, Liskov Substitution Principle, Interface Segregation Principle, Dependency Inversion Principle

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > fruit.splice(2, 1)

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

    > you.friends.push(them)
    them.friends.push(you)

06. Give an example of a JavaScript `Conditional`:

    > if{

    }
    else if{

    }
    else{}

07. What is the main difference between `parameters` and `arguments`?

    > argumetns are the objects that a function accepts, parameters are the vars you are putting in them.

08. Instead of writing everything to the console, what is a better way to debug your code?

    > printing things into the html 

09. What is the difference between a `primitive` value and a `reference` value?

    > primitive is things like var, bool, int, string reference is like 

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for(let i = -100; i > 100; i++){
        console.log(i);
    }
