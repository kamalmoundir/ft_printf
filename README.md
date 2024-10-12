
# ft_printf

## Introduction

The `ft_printf` project is part of the 42 curriculum. The objective is to recreate the C library function `printf`, which is widely used for formatted output. This project will enhance your understanding of variadic functions, string manipulation, and low-level programming in C.

## Features

`ft_printf` supports the following conversion specifiers:

- `%c`: Prints a single character.
- `%s`: Prints a string.
- `%p`: Prints a pointer address.
- `%d` / `%i`: Prints a signed integer.
- `%u`: Prints an unsigned integer.
- `%x`: Prints a number in hexadecimal (lowercase).
- `%X`: Prints a number in hexadecimal (uppercase).
- `%%`: Prints a literal percent sign.

## How to Use

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/ft_printf.git
   ```

2. **Compile the project with your source files:**

   ```bash
   gcc -Wall -Wextra -Werror ft_printf.c <your_project_files.c> -o your_program
   ```

3. **Include `ft_printf.h` in your source files:**

   ```c
   #include "ft_printf.h"
   ```

4. **Call `ft_printf` in your code:**

   ```c
   ft_printf("Hello, %s! You are %d years old.
", "Alice", 25);
   ```

## Project Files

- `ft_printf.c`: Contains the `ft_printf` function and its logic.
- `ft_printf.h`: Header file with function prototypes.
- `utils.c`: Contains helper functions used within `ft_printf`.

## Restrictions

- No use of standard library functions like `printf`.
- Floating point numbers and `*` width specifier are not supported.
- Must handle variadic arguments using `va_list`, `va_start`, and `va_end`.

## Example

You can test `ft_printf` with a simple main function:

```c
#include "ft_printf.h"

int main(void)
{
    ft_printf("Character: %c\n", 'A');
    ft_printf("String: %s\n", "Hello, World!");
    ft_printf("Pointer: %p\n", &main);
    ft_printf("Integer: %d\n", 42);
    ft_printf("Unsigned: %u\n", 3000000000U);
    ft_printf("Hex (lowercase): %x\n", 255);
    ft_printf("Hex (uppercase): %X\n", 255);
    return 0;
}
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author

- Kamal Moundir

Feel free to contribute or report any issues!
