# Clean Code

- [Clean Code](#clean-code)
  - [Sections](#sections)
    - [Section 01 - Getting Started](#section-01---getting-started)
      - [What is Clean Code?](#what-is-clean-code)
      - [Key pain points](#key-pain-points)
      - [Clean Code with Clean Architecture](#clean-code-with-clean-architecture)
      - [Clean Code with Patterns and Principles](#clean-code-with-patterns-and-principles)
    - [Section 02 - Naming](#section-02---naming)
      - [How to name things correctly?](#how-to-name-things-correctly)
      - [Best Practices](#best-practices)
    - [Section 03 - Comments and formatting](#section-03---comments-and-formatting)
      - [Comments](#comments)
      - [Formatting](#formatting)
        - [Vertical Formatting](#vertical-formatting)
        - [Horizontal Formatting](#horizontal-formatting)
  - [References](#references)

## Sections

### Section 01 - Getting Started

#### What is Clean Code?

- Clean code is easy to understand
  - Be readable and meaningful
  - Reduce cognitive load
  - Be concise and "to the point"
  - Avoid unintuitive names, complex nesting and big code blocks
  - Follow common best practices and patterns
  - Be fun to write and to maintain

#### Key pain points

- The names: variables, functions, classes
- Structure and Comments: Code formatting, good and bad comments
- Functions: length, parameters
- Conditionals and Error Handling: Deep nesting, missing error handling
- Classes and Data Structures: missing distinction, Bloated classes

#### Clean Code with Clean Architecture

| Clean Code                         | Clean Architecture               |
| ---------------------------------- | -------------------------------- |
| How to write the code              | Where to write which code        |
| Focus on the single problems/files | Focus on the projects as a whole |

#### Clean Code with Patterns and Principles

| Clean Code                                          | Patterns and Principles                         |
| --------------------------------------------------- | ----------------------------------------------- |
| Write code which is readable and easy to understand | Write code which is maintainable and extensible |

### Section 02 - Naming

> - Names should be meaningful. It helps us understand code without going through it in detail
> - The names are used to describe: what's stored in a variable/property, or what a function/method does, or what kind of object will be created when instantiating a class

#### How to name things correctly?

- Variables, Constants, and Properties: (object, number, string, boolean, etc.)
  > The name implies which kind of data is being stored
  - Use nouns (e.g., `user`, `product`) or short phrases with adjectives (e.g., `isValid`, `isLoggedIn`)
  - Can be more specific (e.g., `customer` instead of `user`)

- Functions and Methods:
  > The name means that they perform tasks and operations
  - Use verbs (e.g., `login()`, `createUser()`) or short phrases with adjectives (e.g., `isValid()`, `isEmpty()`)
  - Avoid names that sound like properties as `email()`
  - Can be more specific as `createUser()` instead of just `create()`

- Classes:
  > The class name should describe the kind of object it will create
  - Use nouns (e.g., `User`, `Payment`) or short phrases with nouns (e.g., `RequestBody`)

#### Best Practices

- Avoid generic names (e.g., `handle()`, `data`, `item`)
- Avoid including descriptions and unnecessary or redundant details
- Choose distinctive names to make it easy to choose
- Consistent name

### Section 03 - Comments and formatting

#### Comments

- What are Bad Comments?
  > It can mean "redundant", "confusing", or even "misleading"

  - **Redundant information**: they add nothing and waste time reading them
  - **Dividers/Block markers**: they only stop your reading flow and make
analyzing the code file harder.
  - **Misleading comments**: they mislead the reader.
  - **Commented-out code**:  instead, just delete it because we can use source control, and we can always bring back old code
- How can we improve it?
  - **Legal information**: maybe we are required to add legal information to your code, which is right at the top of the code file.
  - **"Required" explanations**: explanations that can’t be replaced by good naming
  - **Comment of Warnings**: in rare cases, warnings next to some code
  - **Todo notes**: shouldn't over-do it

#### Formatting

> Code formatting is important and greatly improves readability and conveys meaning
> Each language has different formatting rules.

##### Vertical Formatting

> Using the - well - vertical space in your code file.

- Best practices:
  - Adding blank lines or maybe combining with grouping related concepts together
  - Vertical Density and Vertical Distance

    | Vertical Density                                     | Vertical Distance                                               |
    | ---------------------------------------------------- | --------------------------------------------------------------- |
    | The related concepts should be kept closely together | The  concepts which are not closely related should be separated |

  - Ordering Functions/Methods
    - The ordering should follow the "stepdown rule"
    - A function B should be (closely) below function B - at least if your programming language allows such an ordering.
  - Splitting code across files
    - Should be split into multiple files, and then use import and export statements to connect your code

##### Horizontal Formatting

> Using the horizontal space - that means lines should be kept short and readable

- Best practices:
  - Using short names
  - Breaking lines into multiple lines: should use relatively short lines

## References

- [Udemy: Clean Code](https://www.udemy.com/course/writing-clean-code/)
