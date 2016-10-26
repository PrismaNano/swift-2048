swift-2048
==========

A port of [iOS-2048](https://github.com/austinzheng/iOS-2048) to Apple's new Swift language. The game is present and working, but a number of auxiliary features haven't yet been implemented.

Like the original Objective-C version, swift-2048 does not rely upon SpriteKit. See the description for iOS-2048 for more information.

Instructions
------------

You will need the Xcode 8 to build and run the project. This project also targets iOS 10.

Tap the button to play the game. Swipe to move the tiles.

Thoughts on Swift
-----------------

Swift is a well-designed language that will, hopefully, drag mainstream programming halfway to ML (kicking and screaming the entire way, of course).

If you really want to see my out-of-date thoughts on Swift, check out the git history for README.md.

### Features Swift has that Objective-C lacks
(Not comprehensive)

- Tuples
- Tagged enums (similar to Scala typeclasses)
- Primitive types treated like objects (actually structs) - extensions can declare new methods upon ``Int``, for example
- Enums and structs that support functions and constructors
- ``override`` keyword to explicitly denote a method overriding a superclass implementation
- C++ style function overloading
- Optional function arguments with default values
- Nested functions
- Pattern matching (match with arbitrary conditionals on values, ranges, tuple structure, enums, or types)
- Generics (type reification, not type erasure)
- Typed containers
- Safe typecasting
- Optionals (and optional chaining, implicitly unwrapped optionals, ``weak`` vs ``unowned``, ...)
- Overflow-safe arithmetic
- ``@auto_closure`` attribute, allowing for a very basic form of pass-by-name (as opposed to pass-by-value) function arguments
- ``@final`` attribute, to prevent overriding
- Other attributes, which have a purpose similar to Java annotations or Python decorators
- Type properties (analogous to class methods; must be computed for classes, but can be stored for enums and structs)
- Syntactical sugar for function currying
- Operator overloading
- Custom operators
- Arbitrary behavior for subscripts
- REPL
- Multiple forms of closure literal convenience syntax
- Capture lists in closure declarations, to avoid retain cycles when using closures
- Native range operators and limited array slicing (``..`` and ``...``)


### Objective-C features with no direct native Swift idiom
(AFAIK; some of these might be available through interop)

- Method swizzling
- Key-Value Observing (KVO)
- Adding or modifying methods and classes at runtime
- Invocations
- Message proxying

### Features I wish Swift had

- Better support for n-dimensional array initialization
- Tuples usable as dictionary keys (although there are technical issues)
- Python/MATLAB-style array slicing
- Abstract methods


License
-------
(c) 2014 Austin Zheng. Released under the terms of the MIT license.

2048 by Gabriele Cirulli (http://gabrielecirulli.com/). The original game can be found at http://gabrielecirulli.github.io/2048/, as can all relevant attributions. 2048 is inspired by an iOS game called "Threes", by Asher Vollmer.
