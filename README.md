# S_Language_Compiler
These codes were written for advanced theory of computation class presented by Dr. Alizadeh in Tehran University at Feb 2025

![image](https://github.com/user-attachments/assets/da5d1c98-d7d8-43d2-ab6a-cb8474565888)

# Introduction
In S language, each line of code is represented by an integer number (you can see the coding algorithm here)
This app decodes these code.

# How to use it
In first file there is a class named `Instruction`
You can print the instruction related to this code by running the following code:

```python
code = #some integer#
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
