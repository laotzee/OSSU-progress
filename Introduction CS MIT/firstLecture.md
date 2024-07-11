
--- 


# Topics of the course
- Represent knowledge with *data structures*
- *Iteration and recursion* as computational metaphors

- *Abstraction* of procedures and data types
- *Organize and modularize* systems  using object classes and methods

It is important to code to be readable, for yourself and other people, organization is also important

- Different classes of *algorithms*; searching and sorting for instance
- *Complexity* of algorithms

Part of computer science, know the difference between a good algorithm and a bad algorithm. 

---  

*What does a computer do?* Fundamentally, performs calculations and remember the results. *What kind of calculations?* built-in to the language and the ones you  define as a programmer. 

	Computers only do what you tell them to do

# Types of Knowledge

## Declarative knowledge
When talking about *declarative knowledge*, it means the awareness and understanding of factual information about the world - *knowing that* that  in contrast to *knowing how*. Its necessary and sufficient conditions are that the information must be true, that the person must believe it to be true, and that the person must be in a position of knowing it. 

Examples of declarative knowledge might include: 
- that princess Diana died in 1997
- that Goethe was 83 when he finished writing Faust
- that there is a village in Hertfordshire, England, called Ugley.  

## Imperative Knowledge
It is a recipe of how to 

- Flow of control 
- 

# Types of Computers

## Fixed Computers
Holds a set of instructions and cannot be changed. 

## Stored Program computers
Store a series of instructions, and can be change so that the computer does a different thing.

- Sequence of instructions stored inside a computer, the built-in predefined set of primitive instructions are:
	- Arithmetic and logic
	- Simple tests, logic tests that returns a false or true value (boolean value)
	- Moving data
 - Special program (interpreter) executes each instruction in order
	 - Use tests to change flow of control through sequence
	 - Stop when done
  
- Computer architecture

# Basic Primitives

**But, what are primitives?**  is a fundamental data type that cannot be broken down into a more simple data type. For example, an integer is a primitive data type, while an array, which can store multiple data types, is not. 

- *Alan Turing* prove that you can *compute anything* using 6 primitives: move left, move right, read, write, scan and do nothing. 
- Modern programming languages have more convenient set of primitives
- Can abstract methods to create new primitives.
- Anything computable in one language is computable in any other programming language. (*This is very powerful!!*) 

A programming language provides:
- A set of primitive operations
- Expressions, which area complex but legal combinations of primitives in a programming language
- Expressions and computations that have value and meaning

# Aspects of Languages

A primitive construct in a programming language can be *A number, strings, simple operations* 
- *semantics*: is the meaning associated with  syntactically correct string of symbols with not static semantic error. Programming languages expressions only have a single meaning, but it may not be what the programmer intended

# Where things go wrong
- *Syntactic errors*: Common and easily caught
- *Static semantic errors*: Some languages check for these before running programs and can cause unpredictable errors
- No semantic errors but different meaning than what programmer intended
	- Program crashes, stops running
	- Program run forever
	- Program gives an answer but different than expected

# Python Programs

- Programs manipulate *data objects*
- Objects have a type that defines the kinds of things programs can do to them 
- Object are:
	- *Scalar* (cannot be subdivided)
		- Int
		- Float
		- Bool
		- NoneType, special and has one value
	- *Non-scalar* (have internal structure that can be accessed)
		- Lists
		- Tuples
		- Sets
		- Dictionaries

## Expressions
- Combine objects and operators to form expressions
- An expression has a values, which has a type

## Abstracting expressions

**Why give names to values of expressions?
- To reuse names instead of values
- Easier to change code later

# Book Reading Ideas

- Definition of:
	- Halting problem
	- Turing completeness
	- 

- The idea of *programming as the process of assembling a sequence of operations remains central*
- The best and worst thing about programming is that *the computer will do exactly what you tell it to do*
- Whenever possible, programs should be written in such a way that when they don't work properly, it is self-evident. 
- The code that the programmer writes is refer to as *source code*
- The creator of python is called Guide Von Rossum
- *Scalar* objects are indivisible
- *Non-scalar* objects have an internal structure
- *Literals*: A notation for representing a fixed value in source code. They can also be defined as raw values or data given in variables or constants. 
- *Straight-line Programs*: Execute one statement after another in the order in which they appear, and stop when they run out of statements
- *Branching programs*: being the most simple a conditional statement. It has three parts:
	- A test; an expression that evaluates to either True or False
	- A block of code that is executed if the test evaluates to True
	- An optional block of code that is executed if the test evaluates to False
- A conditional inside another is called *nested*
- *Overloading*: having different meaning depending upon the types of the object to which it is applied. It is said the the '+' and the asterisk are overloaded.
	- 4+3
	- 'a'+'a'
	- 3*'a'
	- 3 asterisk 4
	- 
- 