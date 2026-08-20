<div align="center">
  <img height=300" alt="images" src="https://github.com/user-attachments/assets/e0f0de23-0e96-414a-972c-9775f839bc40" />
</div>

# 🐛 C Debugging Exercises

A set of small C programs used as an internship exercise, where common C mistakes have been found and fixed, each with a comment explaining the fix.

## 📝 Overview

Eleven standalone `.c` files, each focused on one C concept - pointers, memory allocation, string handling, or file I/O. Every corrected line is marked with an inline comment explaining what was wrong and why the fix works.

## 🧩 Examples

- `1_example.c` - address book: builds a singly linked list of contacts from `addresses.csv`, prints it, then frees it
- `2_example.c` - reads bounded user input with `fscanf` to avoid overflow
- `3_example.c` - hello world, returns `0` to signal success
- `4_example.c` - copies a string into a fixed buffer with `strncpy`, guarding against overflow
- `5_example.c` - allocates a buffer with `malloc`, copies a string into it, then frees it
- `6_example.c` - passes a heap-allocated string to a function; the allocator (not the printer) frees it
- `7_example.c` - builds random strings of increasing length, freeing each buffer to avoid leaks
- `8_example.c` - allocates memory inside a function through a double pointer
- `9_example.c` - passes an `int` by pointer to print it
- `10_example.c` - passes an `int` by pointer to modify it
- `11_example.c` - copies `original_file.txt` to `copied_file.txt` line by line

## 🛠️ Building

```sh
make
```

This compiles every `*_example.c` file into a binary of the same name. Run `make clean` to remove them.

## ▶️ Usage

Run any compiled binary directly, for example:

```sh
./1_example
```

`1_example` expects `addresses.csv` to be present in the same directory.

## 🎯 Task

Fix bad C code.

Below, in the document viewer, you can see more than 10 code files and helper files. Each .c file is left with an error or badly written code. Your task is to fix that code.

You need to download all files and, in each file, find what is wrong with it, comment it why it is bad, and write proper code.

When you will finish fixing code, send all files, with your corrections to your internship manager.

You can use the Makefile to compile the code. While standing in the directory where you have downloaded the code, execute command make.
