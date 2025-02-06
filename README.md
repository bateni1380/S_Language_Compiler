# S_Language_Compiler
These codes were written for advanced theory of computation class presented by Dr. Alizadeh in Tehran University at Feb 2025

# Introduction
![image](https://github.com/user-attachments/assets/da5d1c98-d7d8-43d2-ab6a-cb8474565888)

In [S language](https://en.wikipedia.org/wiki/S_(programming_language)), each line of code is represented by an integer number 
You can see the coding algorithm in [this book](https://books.google.de/books?id=6G_arEqHtysC&printsec=frontcover&redir_esc=y#v=onepage&q&f=false) in pages 65-67.
This app decodes these code. The decoding is based on the book.

# How to use it
In first file there is a class named `Instruction`
You can print the instruction related to this code by running the following code:

```python
instruction = Instruction(code=code)
print(instruction)
```

Also in second file, you can run a progrm written in this language with some input variables, then get state of each variable in each snapshot of program.
You can use `Program` class and `print_snapshots` function to see the result: 

```python
p = Program(instruction_codes, input_variables)
snapshots = p.run()

print_snapshots(snapshots)
```
