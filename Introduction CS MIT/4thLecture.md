
**What is a stack frame?** A frame of data that gests pushed onto the stack. In the case of a call stack, a stack frame would representa  function call and its argument data
**What is lexical scoping?** Defines how variables names are resolved in nested functions. Inner functions contain the scope of parent functions even if the parent function has return. 
**What is symbol table?**
**?**

--- 
# Keyword Arguments and Default Values

- Positional arguments: formals are bound to actuals using the name of the formal parameters.


# Scoping

- Each function defines a new *name space* also called *scope*.
- 

# Specification of a Function 

## Assumptions
Describe conditions that must be met by clients of the function. Typically describe constraints on the actual parameters. Almost always, they specify the acceptable set of types for each parameter and not infrequently, some constrains on the value of one or more of the parameters.

## Guarantees
Describe conditions that must be met by the function, provided that it has been called in a way that satisfies the assumptions. 

# Important Concepts

- Decomposition: creates structure. It allows us to break a program into parts that are reasonably self-contained, and that may be reused in different settings.
- Abst3raction: Hides detail. It allows us to use a piece of code as if it were a black box - that is, something whose interioer details we cannot see, don't need to see, and shouldn't even want to see.  The essence of abstraction is preserving infromation that is relevant in a given context, and forgetting information that is irrelevant in the context. *The key to using abstraction effectively in programming is finding a notion of relevance that is appropritate for both the builder of an abtraction and the potential clients of the abstraction* That is the true art of programming . 

# Recursion

It is defined as the process in which a function calls itself directly or indirectly, and the corresponding function is called a recursion function. 


# Lecture

- More code not necessarily a good thing
- Measure good programmers by  the amount of functionality
- Functions as a mechanism to achieve decomposition and abstraction. 

 Code is divided into *modules* that are:
 - Self-contained
 - breaks up the code
 -  Reusable
 - keeps the code organized
 - Keep the code *coherent* 

*None* represents the absence of a value

## return vs print

| return | print |
| -------| ------|
|return only has meaning *inside* a function| print can be used outside functions|
|Only one  return executed inside a function| can execute many print statements inside a function|
|Code inside function, but after return statement not executed|Code insude function executed after a print statement|
|Has a value associated with it, given to a function caller|Has a value associated with it, outputted to the console|


