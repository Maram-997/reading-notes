# Read : Class 09 - FUNCTIONAL PROGRAMMING

## What is functional programming? 
a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable.

## What is a pure function and how do we know if something is a pure function?

It returns the same result if given the same arguments (it is also referred as deterministic)
* It does not cause any observable side effects
What are the benefits of a pure function? The code’s definitely easier to test. We don’t need to mock anything.

## What are the benefits of a pure function?
Pure functions are much easier to read and reason about. All relevant inputs and dependencies are provided as parameters, so no effects are observed that alter variables outside of the set of inputs. This means that we can quickly understand a function and its dependencies, just by reading the function's declaration.



## What is immutability?

Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.


## What is Referential transparency 

pure functions + immutable data = referential transparency

<!------------------------------->

## What is a module?
s a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node. js application. Each module in Node. ... CommonJS is a group of volunteers who define JavaScript standards for web server, desktop, and console application.
## What does the word ‘require’ do?
The require() method is used to load and cache JavaScript modules. So, if you want to load a local, relative JavaScript module into a Node. js application, you can simply use the require() method.
## How do we bring another module into the file the we are working in?
The static import statement is used to import read only live bindings which are exported by another module.

Imported modules are in strict mode whether you declare them as such or not. The import statement cannot be used in embedded scripts unless such script has a type="module". Bindings imported are called live bindings because they are updated by the module that exported the binding.


## What do we have to do to make a module available?
module.export = to what we want make it available