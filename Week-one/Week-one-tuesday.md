<h2>Interpreted and compiled programming languages</h2>

Compiled languages are translated into code that the machine can understand and execute. The main advantage of these type of languages is that they tend to be faster because they are not being translated at run time, the disadvantage is that the code needs to be compiled or translated every time there's a change in the codebase. Whereas the interpreted language is translated at run time which means every command is executed line by line, so there's no need to run an entire compilation step before testing the code which makes it more flexible. The disadvantage of interpreted languages is that they tend to be slower than compiled languages, however, that gap is closing with the development of just-in-time compilation.

<h2>Is Java compiled or interpreted, or both?</h2>

Both. The code is first compiled to bytecode and then in the run-time environment the bytecode can be interpreted using the Java Interpreter.


<h2>Pseudocode Currency Converter exercise</h2>

<code>
START
USD Amount <-- GET
BTCExchange Rate <-- GET
Result <-- USD Amount * BTCExchange Rate
PRINT Result
END
</code>
