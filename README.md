# 📚 Libft

**Your very first own library — 42 School**

Libft is the first project in the 42 Common Core curriculum. The goal of this project is to recreate a collection of standard C library functions, along with additional utility functions, to build a personal C library that can be reused in future projects.

The project focuses on understanding how C works under the hood, improving memory management skills, and developing a deeper understanding of pointers, strings, and data structures.

---

## 🛠️ Technologies

- **Language:** C
- **Compiler:** `cc`
- **Build System:** Makefile
- **Standard:** C89 / C99 (depending on the 42 subject requirements)
- **Allowed Functions:** Depends on the function being implemented and the project requirements.

---

## 📖 Functions

The library is divided into several categories.

### 1. Libc Functions

Reimplementations of standard C library functions.

- `ft_isalpha` – Checks whether a character is alphabetic.
- `ft_isdigit` – Checks whether a character is a digit.
- `ft_isalnum` – Checks whether a character is alphanumeric.
- `ft_isascii` – Checks whether a character belongs to the ASCII character set.
- `ft_isprint` – Checks whether a character is printable.
- `ft_strlen` – Calculates the length of a string.
- `ft_memset` – Fills memory with a constant byte.
- `ft_bzero` – Sets a memory area to zero.
- `ft_memcpy` – Copies memory from one location to another.
- `ft_memmove` – Copies memory while handling overlapping regions.
- `ft_strlcpy` – Copies a string with size limitations.
- `ft_strlcat` – Concatenates strings with size limitations.
- `ft_toupper` – Converts a lowercase character to uppercase.
- `ft_tolower` – Converts an uppercase character to lowercase.
- `ft_strchr` – Finds the first occurrence of a character.
- `ft_strrchr` – Finds the last occurrence of a character.
- `ft_strncmp` – Compares two strings up to a specified length.
- `ft_memchr` – Searches for a byte in memory.
- `ft_memcmp` – Compares two memory areas.
- `ft_strnstr` – Locates a substring within a string.
- `ft_atoi` – Converts a string to an integer.
- `ft_calloc` – Allocates and initializes memory.
- `ft_strdup` – Duplicates a string.

### 2. Additional Functions

Utility functions that extend the functionality of the standard C library.

- `ft_substr` – Extracts a substring from a string.
- `ft_strjoin` – Concatenates two strings into a new allocation.
- `ft_strtrim` – Removes specified characters from the beginning and end of a string.
- `ft_split` – Splits a string using a delimiter.
- `ft_itoa` – Converts an integer into a string.
- `ft_strmapi` – Applies a function to each character of a string.
- `ft_striteri` – Applies a function to each character using its index.
- `ft_putchar_fd` – Writes a character to a file descriptor.
- `ft_putstr_fd` – Writes a string to a file descriptor.
- `ft_putendl_fd` – Writes a string followed by a newline.
- `ft_putnbr_fd` – Writes an integer to a file descriptor.

### 3. Bonus Functions

Linked-list manipulation functions.

- `ft_lstnew` – Creates a new list node.
- `ft_lstadd_front` – Adds a node to the beginning of a list.
- `ft_lstsize` – Counts the number of nodes in a list.
- `ft_lstlast` – Returns the last node of a list.
- `ft_lstadd_back` – Adds a node to the end of a list.
- `ft_lstdelone` – Deletes a single node.
- `ft_lstclear` – Deletes an entire list.
- `ft_lstiter` – Applies a function to each node.
- `ft_lstmap` – Creates a new list by applying a function to each node.

---

## ⚙️ Compilation

To compile the library, clone the repository and navigate into its directory:

```bash
git clone YOUR_REPOSITORY_URL
cd libft
```

Compile the mandatory functions:

```bash
make
```

Compile the bonus functions:

```bash
make bonus
```

Remove object files:

```bash
make clean
```

Remove object files and the compiled library:

```bash
make fclean
```

Recompile everything:

```bash
make re
```

---

## 📦 Usage

To use Libft in another C project, include the header file and link the compiled library.

```c
#include "libft.h"

int main(void)
{
    char *str;

    str = ft_strdup("Hello, 42!");
    if (!str)
        return (1);

    ft_putstr_fd(str, 1);
    ft_putchar_fd('\n', 1);
    free(str);

    return (0);
}
```

Compile your program with:

```bash
cc main.c -I includes -L. -lft -o program
```

---

## 🧠 What I Learned

Through this project, I gained practical experience with:

- Reimplementing standard C library functions.
- Working with pointers and memory addresses.
- Dynamic memory allocation and deallocation.
- String manipulation and memory operations.
- Understanding linked lists and data structures.
- Writing clean, reusable, and modular C code.
- Using Makefiles to automate compilation.
- Following the 42 Norm coding standards.

---

## 👤 gvasylie

---

*This project was developed as part of the 42 School Common Core curriculum.*
