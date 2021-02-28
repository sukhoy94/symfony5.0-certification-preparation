QA
1. PHP interpreted or compiled language?

```   
Both. PHP is compiled down to an intermediate bytecode that is then interpreted by the runtime engine.

The PHP compiler's job is to parse your PHP code and convert it into a form suitable for the runtime engine. Among its tasks:

Ignore comments
Resolve variables, function names, and so forth and create the symbol table
Construct the abstract syntax tree of your program
Write the bytecode
Depending on your PHP setup, this step is typically done just once, the first time the script is called. 
The compiler output is cached to speed up access on subsequent uses. If the script is modified, however, 
the compilation step is done again.

The runtime engine walks the AST and bytecode when the script is called.
The symbol table is used to store the values of variables and provide the bytecode addresses for functions.

This process of compiling to bytecode and interpreting it at runtime is typical for languages that run on some 
kind of virtual runtime machine including Perl, Java, Ruby, Smalltalk, and others.
```
2. How to disable short tags
```
Short tags (example three) are available by default but can be disabled either via the short_open_tag php.ini
configuration file directive, o rare disabled by default if PHP is built with the --disable-short-tags configuration.
```

3. php types
```
PHP supports ten primitive types.

Four scalar types:

bool
int
float (floating-point number, aka double)
string

Four compound types:

array
object
callable
iterable

And finally two special types:
resource
NULL

To forcibly convert a variable to a certain type, either cast the variable or use the settype() function on it.
```

4. Difference between heredoc and nowdoc syntax: 
```
Nowdocs are to single-quoted strings what heredocs are to double-quoted strings. 
A nowdoc is specified similarly to a heredoc, but no parsing is done inside a nowdoc. 
```

