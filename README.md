# ToSon Template maker
### This repo will talk about how to make ToSon files from scracth and how the Syntax works
The offical ToSon website: [![ToSon Site](https://img.shields.io/badge/Website-ToSon-blue?style=for-the-badge&logo=google-chrome&logoColor=white)](https://tosoncode.github.io/ToSon/)

ToSon Template Maker is a lightweight tool for creating and managing ToSon files (.toson) with ease. It allows developers to quickly generate templates, implement commands, and maintain consistent structures for their ToSon projects.

Features

Create ready-to-use ToSon templates

Supports all core ToSon commands

Includes built-in syntax examples for reference

Lightweight and fast, designed for small to medium projects

Dark/light mode support in documentation

Easy integration with other ToSon projects

Installation

Clone the repository:

```git clone https://github.com/ToSonCode/ToSon-temp```

then

```cd ToSon```

Usage

The ToSon Template Maker generates .toson templates using a simple syntax.

Example Template
```[{Main}]{ 
    say >: {
        text: "Hello World" 
        color: "green" 
    } \n
    let x >: { "42" }
    ask >: {
        have "name" >: [
            be "ask1"
        ]n\
        output: "What's your name?"
    }
}
```
Commands Syntax\n

Command	Syntax Example	Description
say: say >: {
    text: "Hello World"
    color: "green"
}
    Print colored text
    
Let: let x >: {
    "42"
}
Assign a variable


ask: ask >: {
    have "name" >: 
        [be "ask1"]
    output: "What's your name?" }
Ask input from user


if/else: if "x" >: {
    value: {
        "42"
        } 
    say >: { text: "X is 42" }
else >: {
    say >: {
        text: "X is not 42" }
    }
}
Conditional execution


repeat:	repeat 3 {
    say >: {
        text: "Hi" 
        }
    }	
Loop commands multiple times


choose:	choose >: {
    from: [
        "A","B"
       ] 
       have "choice" }	
Pick a random value from a list


set:	set block "Main" >: 
    [ 
        { key: val
    }
]	

Assign block variables


list:	list	
Show all implemented commands


Example Usage
[{Main}]{
    say >: {
        variable: none
        text: "Hello World!"
        color: "green"
    }
    let x >: { "42" }
}


This template demonstrates a basic ToSon file with a say command and a variable assignment.

Resources

ToSon Main Repository

ToSon Resources Repository

Contributing

Contributions are welcome! Please follow these steps:

Fork the repository

Create a new branch (git checkout -b feature/YourFeature)

Make your changes

Commit and push your changes

Open a Pull Request

License

MIT License © 2025 ToSon
