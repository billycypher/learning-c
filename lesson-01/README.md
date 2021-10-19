# Hello, World!

[:brazil: Leia isso em português do Brasil](README.PT-BR.md)

This was our first project. What this program does is print the phrase "hello world" and insert a new line in the terminal.

The first thing we did was to include the standard input-output header `stdio.h`. We couldn't use the `printf` function without it and it is resposible for printing the messages.

Then, we declared the `main` function that is needed for the compiler to know where to start executing the code. It needs to return an integer (return of type `int`), so we pass the value `0` as a return, as any value other than `0` is treated as an error.

Lastly, we add the `printf` function that will take 2 arguments in this case.

The first one is a string that defines the format. In this case, it was `"%s\n"` which means:

1. `%s`: expect the next argument to be a string.
1. `\ n`: insert a new line when printting this character .

The second argument is our `" hello, world! "` message.

# How to compile?

First of all, you need _clang_ installed on your machine, then run:

```sh
clang --pedantic -std=c89 ./main.c -o program && ./program
```

or, if you have _make_ installed, just run the binary from this folder:

```sh
make && make run
```
