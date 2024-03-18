# C Compiler Phases

This repository contains code and resources for various phases of a C compiler. Each phase is implemented separately to understand the workings of a compiler better.

## Lexical Analyzer

The lexical analyzer is the first phase of the compiler, responsible for converting the source code into a sequence of tokens. This phase removes comments, white spaces, and identifies keywords, identifiers, constants, operators, and punctuation symbols.

### Usage

To use the lexical analyzer, you can compile the provided code (`lexAnalyzer.c`) using a Lex tool:

```bash
lex lexAnalyzer.l
cc lex.yy.c 
./a.out < testCases/ifelse.c
```
The Symbol Table will be generated in symbolTable.txt file.
There is also a lex file to remove comments from a given .c file 

```bash
lex commentRemover.l
cc lex.yy.c
./a.out < testCases/ifelse.c
```

A new file called output.c will be created.

