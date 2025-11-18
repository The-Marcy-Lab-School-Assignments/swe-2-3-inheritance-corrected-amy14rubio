# Short Responses

For this short response assignment, aim to write a response with the following qualities (your instructor will give you feedback on these areas):

- [] Addresses all parts of the prompt
- [] Accurately uses relevant technical terminology
- [] Is free of grammar and spelling mistakes (double check with grammarly!)
- [] Uses markdown to enhance readability (preview in VS Code with Command/Control + Shift + V)
- [] Is easy to comprehend

For each prompt below, write your response in the space provided. Aim to answer each prompt in 2-5 concise sentences. Make sure to preview your markdown to check how it is rendered before submitting.

## Prompt 1

In your own words, define what **inheritance** is in object-oriented programming. Then, explain what benefits it provides to developers who use it. Consider what problem it solves — what would be harder or messier without inheritance?

## Response 1

In object-oriented programming, **inheritance** is when a class can access the properties and methods of its parent class because it `extends` that class, often using `super()` to reference the parent’s functionality. Some benefits inheritance provides for developers are that it allows a **subclass to reuse and build on the parent class's code**, and it helps keep programs **better structured, consistent, and predictable**. Code would definitely be messier and harder to follow and understand without inheritance.

## Prompt 2

Consider these classes:

```js
class Animal {
  eat() {
    return 'eating';
  }
}

class Dog extends Animal {
  bark() {
    return 'woof';
  }
}

class Puppy extends Dog {
  play() {
    return 'playing';
  }
}

const rex = new Puppy();
```

Explain what happens when `rex.eat()` is invoked. In your answer, describe the role of **inheritance** and the **prototype chain**.

## Response 3

When `rex.eat()` is invoked, the console prints 'eating'. This is due to **inheritance**, where the program moves up the **prototype chain** to check if the invoked method exists and then executes it.

## Prompt 3

Look at these classes:

```js
class Employee {
  constructor(name, salary) {
    this.name = name;
    this.salary = salary;
  }
  getDetails() {
    return `${this.name} earns $${this.salary}`;
  }
}

class Manager extends Employee {
  constructor(name, salary, department) {
    super(name, salary);
    this.department = department;
  }
  getDetails() {
    return `${super.getDetails()} at the ${this.department} department`;
  }
}
```

Complete the `Manager` class by filling in the `constructor` and `getDetails` methods. Explain why you need to use `super` in each method and what would happen if you didn't use it.

## Response 3

`super` needs to be used in the constructor because the `Manager` class must call the parent class’s `constructor` to properly set up the `name` and `salary` properties. `super` is then used in `getDetails()` to return the same message as the parent class while adding the manager's department information. If `super` weren't used, I would have to rewrite the code using unnecessary and much longer lines of code, like so:

```js
class Manager extends Employee {
  constructor(name, salary, department) {
    this.name = name;
    this.salary = salary;
    this.department = department;
  }
  getDetails() {
    return `${this.name} earns $${this.salary} at the ${this.department} department`;
  }
}
```
