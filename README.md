Learning asm x64 for Linux
==========================

Repository created in order to learn basics of Assembly x64 for Linux

Preparation
-----------

Install NASM:

```
$ sudo pacman -S nasm
```

**The Netwide Assembler (NASM)** is an assembler and disassembler for the Intel x86 architecture.

Compiling and running the programs
----------------------------------

Go into directory with task and type `make`. To clean generated files type `make clean`. To run the program, simply call it from the local dir - e.g. `./hello`.

References
----------

### Assembly
- https://github.com/0xAX/asm
- http://0xax.github.io/categories/assembly/
- http://cs.lmu.edu/~ray/notes/gasexamples/
- http://stackoverflow.com/questions/721583/what-is-the-best-way-to-learn-x86-assembly-on-a-linux-platform
- http://stackoverflow.com/questions/836946/basic-yet-thorough-assembly-tutorial-linux
- https://www.tutorialspoint.com/assembly_programming/
- http://helion.pl/ksiazki/praktyczny-kurs-asemblera-wydanie-ii-eugeniusz-wrobel,pkase2.htm

### Makefile
- [A simple Makefile tutorial](http://www.cs.colby.edu/maxwell/courses/tutorials/maketutor/)
- [Makefiles - tutorial by example](http://mrbook.org/blog/tutorials/make/)
- [Makefiles - Computer Science II](https://www.cs.umd.edu/class/fall2002/cmsc214/Tutorial/makefile.html)
- [Unix Makefile Tutorial](http://www.tutorialspoint.com/makefile/)
- [Makefile tutorial](http://makefiletutorial.com/)

### Others
- [How to make a Computer Operating System?](https://github.com/SamyPesse/How-to-Make-a-Computer-Operating-System)
- [BareMetal - a 64-bit OS for x86-64 based computers](https://github.com/ReturnInfinity/BareMetal-OS)
