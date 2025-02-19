# Unexpected Instance Variable Modification in Ruby

This repository demonstrates a potential issue in Ruby related to modifying instance variables directly using `instance_variable_set`. While functional, directly manipulating instance variables can bypass encapsulation and lead to unexpected behavior, especially in larger or more complex projects.

## The Bug
The `bug.rb` file showcases the use of `instance_variable_set` to modify the `@value` instance variable of the `MyClass` object.  Although this works, it's generally discouraged as it circumvents the intended method of accessing and modifying object attributes.

## The Solution
The `bugSolution.rb` file provides an alternative, more robust solution using a setter method. This adheres to the principles of encapsulation, making the code more maintainable, predictable, and less prone to errors caused by unexpected instance variable modification.