[Link to article](https://github.com/zakirullin/cognitive-load?tab=readme-ov-file)

# Introduction

The author aims to establish cognitive load as a key if not the one true metric of evaluating good code. The author demonstrates this with practical examples.

# What is cognitive load

* The average person can hold about 4 facts in their brain at any given time. _Note: This is not a proven fact, but rather an approximation. The more accurate way of thinking about this would be, that every human being has a finite amount of facts that they can hold in their brain at any given time._
* Two types of cognitive load
    * Intrinsic: Inherent difficulty of the task. Can't be reduced.
    * Extraneous: Difficulty created because of poor design of the code and other factors. Can be reduced.

# Reducing cognitive load

* Reducing complex conditionals.
    * Use intermediate variables such as _isAllowed_ instead of _if(condition1 && condition2 || condition3) { allowSomething(); }_
    * Early returns from conditionals instead of nested ifs.
* Inheritance nightmare
    * Prefer [composition over inheritance](https://www.youtube.com/watch?v=hxGOiiR9ZKg)
* Shallow classes, methods, or interfaces
    * Refer to John Ousterhoust's [A philosophy of software design](https://web.stanford.edu/~ouster/cgi-bin/book.php)
    * Simple interfaces with deep functionality
* Single responsibility principle - the author is a bit vague about this (intetionally, perhaps?). One way of defining single responsibility could be that a module handles the actions required of one entity in the business domain and a function performs a single action on a single entity in the business domain. 
    * E.g., `Comment` module handles the actions required for `Comments` entity in the `Goals` domain. `create` function handles creating the `GoalComment` taking care of pre-creation steps like `authorization`, `validation`, and post-creation steps like `notifcation`. This strongly ties in with DDD ideas. 
* Shallow microservices - the age-old monolith vs microservices debate. A well-crafted monolith is the best solution for an early stage business. The monolith could be decomposed to a collection of deep macroservices if business needs demand it. It is never advisable to decompose a monolith to a massive amount of microservices, turning it into a distributed monolith.
* Avoid using language specific features. _Note: This is different from writing code in your language's idiom. Python code must still be pythonic. Just don't use some obscure quirk of Python that will confuse future developers, including you._
* Using descriptive response codes instead of just HTTP. _Note: This doesn't mean inventing your own response codes. A HTTP GET call to a non-existent resource must still return 404 and a call to a restricted resource before the user logs in must return 401. But these can be annotated in the response payload to reduce cognitive load._
* Too much DRY - _A little copying is better than a little dependency._
* Tight coupling with frameworks - keep business logic outside your framework. This will help new developers get onboarded faster.
* Simple architectures instead of layered complexity. Avoid _clever architectures_. Involve junior devs in architecture reviews.
* Do not mistake **familiarity** for **simplicty**. A bad code base might have low cognitive load for developers who are familiar with it but that doesn't mean it is simple. _This can be measured using the DX core metric of time taken to first PR for a new engineer._

# My takeaways

* Encourage developers of all levels to participate in architecture and code review.
* Measure time to first PR when the team scales.
* Discuss with Maher to understand the reasoning behind our choices for an event driven microservices architecture.

