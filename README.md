Learning asm x64 for Linux
==========================

Repository created in order to learn basics of Assembly x64 for Linux

Preparation
-----------

Install NASM:

```
$ sudo apt-get install nasm
```

**The Netwide Assembler (NASM)** is an assembler and disassembler for the Intel x86 architecture. 

Compiling and running the programs
----------------------------------

In the beginning, we can create simple hello world program and save it to `hello.asm` file:

```assembly
section .data
    msg db      "hello, world!"

section .text
    global _start
_start:
    mov     rax, 1
    mov     rdi, 1
    mov     rsi, msg
    mov     rdx, 13
    syscall
    mov    rax, 60
    mov    rdi, 0
    syscall
```

Assembly programs can be compiled in the following way:

```
$ nasm -f elf64 -o hello.o hello.asm
$ ld -o hello hello.o
```

When compilation is done, we can run the program:

```
$ ./hello
```

We can also create `Makefile` file with the following content:

```
all:
	nasm -f elf64 -o hello.o hello.asm
	ld -o hello hello.o

clean:
	rm hello hello.o
```

After that, we can use the following command to compile the project:

```
$ make
```

If we want to remove output files (`hello.o` and `hello`), we can just type:

```
$ make clean
```

References
----------
https://github.com/0xAX/asm
