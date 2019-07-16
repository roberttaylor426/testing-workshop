# Testing workshop

## Why do we test?

The fundamental values of software:

1. Meet the needs of the customer today
2. Accommodate changing requirements

### Zooming in:

* Help ensure correctness
* Help keep the code clean by allowing us to make changes with confidence
* Better than documentation, they're an executable specification
* They can aid with code design
* Help you think outside-in
* Shorten the feedback loop
* Reduced stress (see [Ease at Work by Kent Beck](https://www.infoq.com/presentations/self-image/))

## Beware!

### Tests are not zero-cost

* They can become tightly coupled to the system
* They can become expensive to run and maintain

In short, they need to be treated as first class citizens. Design and maintain them with the same consideration and priority you would apply to production code.

### Applying tests to a legacy codebase is _hard_

* Code was likely not designed with testing in mind
    * Coupling to frameworks, databases and other delivery mechanisms can be hard to break apart
* Learning how to test effectively takes practice
    * What to test, what not to test?
    * How do I make thing x testable?
* Productivity in the short-term will drop
    * Stakeholders and developers alike quickly lose patience

## Different types of tests

See [the testing pyramid](https://www.google.com/search?client=ubuntu&hs=2EC&channel=fs&biw=1920&bih=982&tbm=isch&sa=1&ei=5S4uXamoIYu-a5j7iIgK&q=testing+pyramid&oq=testing+py&gs_l=img.3.0.0l6j0i5i30l4.51700.54500..55600...0.0..0.200.2100.1j5j8......0....1..gws-wiz-img.....0..0i67._SHf6G5RWWw).

In general, further up the pyramid means:

* Greater confidence in system correctness
* Tests are slower to run
* Tests are harder to write and maintain
* Defect localization becomes harder

Unit tests should be written [FIRST](https://hackernoon.com/test-f-i-r-s-t-65e42f3adc17):

 * Fast
 * Isolated
 * Repeatable
 * Self-validating
 * Thorough and timely

## TDD

Practice that emerged out of [Extreme Programming (XP)](http://www.extremeprogramming.org/). Write tests before production code :-S

### Red-Green-Refactor

1. Write test to drive the implementation
2. Write minimal implementation to get the test to pass
3. Refactor
4. Repeat!

### You try!

Let's try the [Roman Numerals Kata](http://codingdojo.org/kata/RomanNumerals/).
