# Code Review tips

#### Functional

1. SOLID: Does the code follow SOLID principles?

```
i. Single responsibility principle
A class should only have a single responsibility, that is, only changes 
to onepart of the software's specification should be able to affect the 
specification of the class.


ii. Open–closed principle
"Software entities ... should be open for extension, but closed for modification."

iii. Liskov substitution principle
"Objects in a program should be replaceable with instances of their subtypes 
without altering the correctness of that program." 

iv. Interface segregation principle
"Many client-specific interfaces are better than one general-purpose interface.

v. Dependency inversion principle
One should "depend upon abstractions, concretions."

```

2. Check for null pointers where exceptions are needed.

3. Buffer Overflows

4. Integer overflows

5. Uninitialised objects

6. DRY: Are re-usble properties, routines being cached?

7. Formatting: Where are the spaces and line breaks? Are they using tabs or spaces? How are the curly braces laid out?

8. Style: Are the variables/parameters declared as final? Are method variables defined close to the code where they’re used or at the start of the method?

9. Naming: Do the field/constant/variable/param/class names conform to standards? Are the names overly short?

10. Test coverage: Is there a test for this code?

11. Race conditions: Any global polution? Leakages? Managing callbacks and side effects.

12. Design patterns: What design patterns are used in the new code? Any anti-patterns (in loops etc)

13. Lines of code: Are functions too long?

14. Using modern syntaxes (ES6): Arrow functions, default parameters, block scoping, template strings, spread operators, generator functions, destructuring etc

15. Optimisation in multi-threaded code

#### Security

Attacks and vulnerabilities

1. DoS - denial of service attacks

2. XSS - Cross Site Scripting

3. MIM - Man in the Middle

4. CSRF - Cross Site Request Forgery (use CSRF token implementation )

5. CORS

##### Tools

1. Morgan - for logging vulnerabilities

2. SNYK - Checking vulnerabilities in NPM and other packages in CI/CD pipeline

3. Helmet - Helmet helps you secure your Express apps by setting various HTTP headers. It's not a silver bullet, but it can help! It includes a  11 packages that all work to block malicious parties from breaking or using an application to hurt its users.
