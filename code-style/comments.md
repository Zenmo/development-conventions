# Location

A class or its most important method usually should have a comment.

Comments on parts or details should be close to the code which they apply to. They should not all go at the top of the class.

# Content

Comments should not explain things that are obvious from the class or method name, parameter names, exception messages or log messages.

Rather it should explain the background:

- broader context of the class within the program
- what assumptions are made that are not possible to check in the code
- what do the parameters represent

# Style

Comments should be in English.

Comments should be imperative mood. Example:

- good: *increment the value by one and pass it on*
- bad: *this increments the value by one and passes it on*

# Common coding agent pitfalls

## History

When refactoring or moving functionality, comment on the functionality as it is now. Do not mention where the code originally came from. Do not mention symbols that don't exist anymore.

## ALL CAPS

All caps should be used sparingly.

## Assume less context

Write comments as if for a reader who is casually browsing the code and doesn't know what he is looking at.
