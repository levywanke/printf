
# 0x11. C - printf

This project involves creating your own version of the `printf` function in C, capable of handling various format specifiers and custom conversions.

---

## Table of Contents

1. [Description](#description)
2. [Files Structure](#files-structure)
3. [Features](#features)
4. [Functionality](#functionality)
5. [Usage](#usage)
6. [Examples](#examples)
7. [Installation](#installation)
8. [Testing](#testing)
9. [Contributing](#contributing)
10. [License](#license)

---

## Description

This project implements a custom `printf` function in C, which replicates the functionality of the standard library function `printf`. It supports basic format specifiers (`c`, `s`, `%`) as well as additional custom specifiers (`d`, `i`, `u`, `o`, `x`, `X`, `b`, `S`, `p`, `r`, `R`).

---

## Files Structure

- `main.c`: Main file for testing purposes (not to be pushed to repo).
- `_printf.c`: Implementation of the custom `_printf` function.
- `main.h`: Header file containing function prototypes.
- `helpers.c`: Helper functions used by `_printf.c`.
- `holberton.h`: Additional header file with includes and guards.

---

## Features

- Supports standard format specifiers: `c`, `s`, `%`.
- Handles custom specifiers: `d`, `i`, `u`, `o`, `x`, `X`, `b`, `S`, `p`, `r`, `R`.
- Basic functionality similar to `printf`, excluding buffer handling.

---

## Functionality

The `_printf` function processes format specifiers in a format string and prints formatted output to stdout. It uses variadic arguments (`va_list`) to handle multiple parameters passed to the function.

---

## Usage

To use `_printf`, include `main.h` in your C file and call `_printf` with the desired format string and arguments. Here’s a basic example:

```c
#include "main.h"

int main(void)
{
    _printf("Hello, %s!\n", "World");
    return (0);
}
```

---

## Examples

### Example 1

```c
_printf("Character: %c\n", 'A');
// Output: Character: A

_printf("String: %s\n", "Hello, world!");
// Output: String: Hello, world!
```

### Example 2

```c
_printf("Decimal: %d\n", 42);
// Output: Decimal: 42

_printf("Unsigned: %u\n", 500);
// Output: Unsigned: 500
```

---

## Installation

Compile your project using the following command:

```bash
$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o printf
$ ./printf
```

---

## Testing

Create test cases in separate files to validate `_printf` functionality. Use sample inputs and compare outputs with standard `printf` for accuracy.



## Additional Sections

Depending on your project's complexity or requirements, consider adding:

- **FAQs**: Common questions and answers.
- **Acknowledgements**: Credits to contributors or resources.
- **References**: Links to relevant documentation.


