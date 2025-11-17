# Technical Coding Feedback

## Overview Takeaways

This submission appears to be incomplete. All class definitions are empty, containing only the class declarations without any implementation. To complete this assignment, you'll need to implement two problem sets: Shapes (Shape, Circle, Rectangle, Square) and Library Items (LibraryItem, Book, DVD, Magazine) according to the requirements in the README.

## Inline Feedback

### Problem Set 1: Shapes

**Lines 3-5 (shapes.js)**: The `Shape` class is declared but contains no implementation. You need to:
- Add a constructor that accepts a `type` parameter and stores it
- Implement `getArea()` method that returns `0`

**Lines 7-9 (shapes.js)**: The `Circle` class is declared but contains no implementation. You need to:
- Make it extend `Shape` using `extends Shape`
- Add a constructor that accepts a `radius` parameter
- Call the parent constructor with `super('Circle')`
- Store the `radius` property
- Override `getArea()` to calculate and return `Math.PI * radius ** 2`

**Lines 11-13 (shapes.js)**: The `Rectangle` class is declared but contains no implementation. You need to:
- Make it extend `Shape` using `extends Shape`
- Add a constructor that accepts `length` and `width` parameters
- Call the parent constructor with `super('Rectangle')`
- Store the `length` and `width` properties
- Override `getArea()` to calculate and return `length * width`

**Lines 15-17 (shapes.js)**: The `Square` class is declared but contains no implementation. You need to:
- Make it extend `Rectangle` using `extends Rectangle`
- Add a constructor that accepts a `side` parameter
- Call the parent constructor with `super('Square', side, side)` (passing side for both length and width)
- The `getArea()` method will be inherited from Rectangle, so you don't need to override it

### Problem Set 2: Library Items

**Lines 3-5 (library-items.js)**: The `LibraryItem` class is declared but contains no implementation. You need to:
- Add a constructor that accepts `title` and `author` parameters
- Store both properties
- Implement `getInfo()` method that returns a formatted string with title and author

**Lines 7-9 (library-items.js)**: The `Book` class is declared but contains no implementation. You need to:
- Make it extend `LibraryItem` using `extends LibraryItem`
- Add a constructor that accepts `title`, `author`, and `pages` parameters
- Call the parent constructor with `super(title, author)`
- Store the `pages` property
- Override `getInfo()` to include pages information

**Lines 11-13 (library-items.js)**: The `DVD` class is declared but contains no implementation. You need to:
- Make it extend `LibraryItem` using `extends LibraryItem`
- Add a constructor that accepts `title`, `director`, and `duration` parameters
- Call the parent constructor with `super(title, director)` (note: director is the author for DVDs)
- Store the `duration` property
- Override `getInfo()` to include duration information

**Lines 15-17 (library-items.js)**: The `Magazine` class is declared but contains no implementation. You need to:
- Make it extend `LibraryItem` using `extends LibraryItem`
- Add a constructor that accepts `title`, `publisher`, and `issueNumber` parameters
- Call the parent constructor with `super(title, publisher)` (note: publisher is the author for magazines)
- Store the `issueNumber` property
- Override `getInfo()` to include issue number information

## Code Quality Observations

### Current Status

- **Incomplete**: All classes are empty and need full implementation
- **Structure**: The class declarations and module.exports are correctly set up, which is a good start

### Next Steps

1. **Start with Shapes**: This problem set is simpler - implement it first to build confidence
2. **Review the README**: The README contains detailed requirements and examples for each class
3. **Run Tests Frequently**: Use `npm test` to check your progress as you implement each class
4. **Focus on Inheritance**: Pay special attention to using `extends` and `super()` correctly
5. **Understand Method Overriding**: When you override methods, make sure to call `super()` in constructors and understand when to override vs. inherit methods

## Summary

This assignment requires implementing two class hierarchies using inheritance. Start with the Shapes problem set (Shape → Circle, Rectangle → Square), then move to Library Items (LibraryItem → Book, DVD, Magazine). The README provides excellent examples and the test file shows exactly what behavior is expected. Don't hesitate to ask for help if you get stuck on any particular class!

