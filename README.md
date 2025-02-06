# S_Language_Compiler
These codes were written for advanced theory of computation class presented by Dr. Alizadeh in Tehran University at Feb 2025

# Introduction
![Screenshot 2025-02-06 061817](https://github.com/user-attachments/assets/db2c7c6a-915f-496c-b920-a1a50795afbb)

In [S language](https://en.wikipedia.org/wiki/S_(programming_language)), each line of code is represented by an integer number. You can see the coding algorithm in [this book](https://books.google.de/books?id=6G_arEqHtysC&printsec=frontcover&redir_esc=y#v=onepage&q&f=false) in pages 65-67.

The first notebook `EX1_Decoder` Inputs some integers, then it decodes these integers based on the books decoding, then it returns the corresponding codes in S language.
The second notebook `EX2_Universal_Program` Inputs some integers, then it decodes these integers based on the books decoding, then it gets a list of inputs ($x_{1}, x_{2}, ..., x_{n}$), then it runs the program (corresponding to those integers) on the input variables ($x_{1}, x_{2}, ..., x_{n}$). Then it prints all snapshots of the program in each step.

# How to use it
In first file there is a class named `Instruction`.

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
