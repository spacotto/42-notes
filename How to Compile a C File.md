# How to Compile a C File

1. Make sure you're in the folder that contains your `.c` files.

2. Compile the files using `cc`, `gcc`, `clang`. They are equivalent.
| Part                    | Meaning                                         |
| ----------------------- | ----------------------------------------------- |
| `cc`, `gcc`, `clang`    | The compiler                                    |
| `-Wall -Werror -Wextra` | Enable helpful warnings                         |
| `file_name.c`           | List of C files to compile                      |
| `-o program_name`       | Output filename (the name of the final program) |


3. Run your program (`a.out` is the standard name)
`./program_name`
