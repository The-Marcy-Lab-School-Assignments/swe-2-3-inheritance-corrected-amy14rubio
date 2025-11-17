# Short Response Assignment Feedback

## Checklist

- [ ] Grammar free
- [ ] Answers all parts of the question
- [ ] Accurately uses technical terminology
- [ ] Is easy to comprehend
- [ ] Uses markdown

## Score Summary

**Total Score: 0/18 (0%)**

- **Prompt 1**: Technical 0/3 + Writing 0/3 = 0/6
- **Prompt 2**: Technical 0/3 + Writing 0/3 = 0/6
- **Prompt 3**: Technical 0/3 + Writing 0/3 = 0/6

**Status**: ❌ Below 75% threshold - Must be revised and resubmitted

## Overview Takeaways

This submission is incomplete - all three short response prompts are left blank. To complete this assignment, you need to provide answers to all three prompts addressing inheritance concepts, the prototype chain, and using `super` in constructors and methods.

---

## Detailed Feedback by Prompt

### Prompt 1: Definition of Inheritance

**Technical Score: 0/3**  
**Writing Quality Score: 0/3**  
**Total: 0/6**

#### Issues

- ❌ No response provided
- ❌ Does not address any part of the prompt

#### What You Need to Do

You need to:
1. Define what inheritance is in object-oriented programming (in your own words)
2. Explain what benefits it provides to developers
3. Consider what problem it solves - what would be harder or messier without inheritance?

---

### Prompt 2: Prototype Chain and Inheritance

**Technical Score: 0/3**  
**Writing Quality Score: 0/3**  
**Total: 0/6**

#### Issues

- ❌ No response provided
- ❌ Does not address any part of the prompt

#### What You Need to Do

You need to explain:
1. What happens when `rex.eat()` is invoked (where `rex` is a `Puppy` instance)
2. Describe the role of **inheritance** in this process
3. Describe the role of the **prototype chain** in this process

**Hint**: `Puppy` extends `Dog`, which extends `Animal`. When `rex.eat()` is called, JavaScript looks up the prototype chain to find the method.

---

### Prompt 3: Using `super` in Constructors and Methods

**Technical Score: 0/3**  
**Writing Quality Score: 0/3**  
**Total: 0/6**

#### Issues

- ❌ No response provided
- ❌ Does not address any part of the prompt

#### What You Need to Do

You need to:
1. Complete the `Manager` class constructor by filling in the code (should call `super(name, salary)`)
2. Complete the `getDetails()` method (should call `super.getDetails()` and add department info)
3. Explain why you need to use `super` in the constructor
4. Explain why you need to use `super` in the `getDetails()` method
5. Explain what would happen if you didn't use `super` in each case

**Example solution:**
```js
constructor(name, salary, department) {
  super(name, salary);
  this.department = department;
}

getDetails() {
  return `${super.getDetails()} and manages ${this.department}`;
}
```

---

## Action Items for Revision

1. **Complete all three responses**: Each prompt requires a detailed response
2. **Use markdown formatting**: Use bold, italics, and code blocks to enhance readability
3. **Proofread**: Check for spelling and grammar errors before submitting
4. **Provide code examples**: Include code examples where appropriate (especially for Prompt 3)
5. **Review the README**: The assignment instructions provide guidance on what to include

---

## Resources for Improvement

- Review the class materials on inheritance and the `extends` keyword
- Review the materials on `super()` and when to use it
- Review the concept of the prototype chain
- Look at the Shapes and Library Items classes you're implementing - they use inheritance, which can serve as examples
- Use markdown preview in VS Code (Command/Control + Shift + V) to check formatting
- Consider using a grammar checker before submitting

---

## Summary

This assignment requires written responses to three prompts about inheritance concepts in JavaScript. All prompts are currently blank and need to be completed. Aim for 2-5 concise sentences per response (or more for Prompt 3 which requires code), use proper markdown formatting, and include code examples where appropriate. Once completed, this will help demonstrate your understanding of these important OOP concepts.

