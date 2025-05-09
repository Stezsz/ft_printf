# ft_printf – 42 School Project

`ft_printf` is a project that replicates the behavior of the standard C `printf` function.
It aims to deepen understanding of **variadic functions**, **format string parsing**, and **low-level output handling**.

---

## Main Objectives

- Recode a simplified version of `printf`.
- Learn how to handle **variadic arguments** using `stdarg.h`.
- Parse format specifiers and convert different types.
- Manage output through low-level file descriptors using `write`.
- Handle **flags, field widths, precision, and conversions**.

---

## Supported Conversions

The following conversion specifiers are implemented:

| Specifier | Description               |
|-----------|---------------------------|
| `%c`      | Character                 |
| `%s`      | String                    |
| `%p`      | Pointer (memory address)  |
| `%d` / `%i` | Signed integer          |
| `%u`      | Unsigned integer          |
| `%x` / `%X` | Hexadecimal (lower/upper) |
| `%%`      | Percent sign              |

---

## Technical Requirements

- You must not use the real `printf` (or `sprintf`, `snprintf`, etc.).
- The function must handle **buffered output** using only `write`.
- All flags must behave identically to the real `printf` (for the supported specifiers).
- Memory management must be efficient and leak-free.
- Code must follow the **42 Norm (Norminette)**.
- A working `Makefile` must be provided to compile the library.

---

## Example Usage

```c
#include "ft_printf.h"

int main(void)
{
    ft_printf("Hello %s! You have %d new messages.\n", "Alice", 5);
    ft_printf("Memory address: %p\n", (void *)main);
    ft_printf("Hex: %x | Unsigned: %u\n", 255, 255);
    return (0);
}
```

---

## Conclusion

`Libft` acts as a **personal C toolkit**, essential for all upcoming 42 projects.
It teaches discipline, good coding practices, and provides a solid understanding of C programming fundamentals.

---

> ✅ **Final Grade: 100/100**
> Project made at [42 School](https://www.42lisboa.com/pt/)
> 👤 Author: Stephan Rodrigues Lassaponari ([@Stezsz](https://github.com/Stezsz))
