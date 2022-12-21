# Translation Software


## Compilers

- Translate high-level code to byte-code (machine code)
- Accept high-level source code and output object code

**Phases**:
1) **Lexer**: Seperates the source code into *tokens*.[^1]
2) **Parser**: Groups tokens into syntactically valid statements.
3) **Intermediate Code Generator**: Converts statements into a stream of simple instructions.
4) **Optimizer**: Optimizes the instructions by several techniques such as removing redundancy.
5) **Code Generator**: Produces an object file containing the bytecode.
6) **Linker**[^2]:
	1) Creates a single executable file.
	2) Integrates libraries and modules referenced in the source code.
	3) Assigns relative addresses to different programs.
7) **Loader**[^3]: Loads the executable file into main memory for execution.

[^1]: Also called *Tokenization* or *Lexical Analysis*.
[^2]: Also see [Linking](../../Extras/Linking.md).
[^3]: Also see [Loading](../../Extras/Loading.md).
