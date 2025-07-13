Function Elements
=======

#include <unistd.h>

void    ft_putchar(char c)
{
    write (1, &c, 1);
}

| Code                         | Name                     | Purpose                                    |
| ---------------------------- | ------------------------ | ------------------------------------------ |
| `void ft_putchar(char c);`   | Declaration (Prototype)  | Tells the compiler the function exists     |
| `void ft_putchar(char c) {}` | Definition               | Provides the actual code to execute        |
| `{ ... }`                    | Scope / Body             | Contains the logic and defines local scope |

`#include <unistd.h>`
| Element      | Meaning                                                                 |
| ------------ | ----------------------------------------------------------------------- |
| `#include`   | Preprocessor directive – tells the compiler to include a library        |
| `<unistd.h>` | Header file – provides access to the `write` system call (among others) |

`void ft_putchar(char c)`
| Element      | Meaning                                                       |
| ------------ | ------------------------------------------------------------- |
| `void`       | Return type – the function doesn't return anything            |
| `ft_putchar` | Function name                                                 |
| `(char c)`   | Parameter – a character named `c` is passed into the function |

`write (1, &c, 1);`
| Element      | Meaning                                                                     |
| ------------ | --------------------------------------------------------------------------- |
| `write`      | System call – used to write data to a file descriptor                       |
| `(1, &c, 1)` | Arguments: `1` = standard output, `&c` = address of character, `1` = 1 byte |
| `;`          | Statement terminator                                                        |

