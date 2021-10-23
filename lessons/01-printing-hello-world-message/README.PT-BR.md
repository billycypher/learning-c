# Olá, mundo!

[:us: Read this in English](README.md)

Esse foi nosso primeiro projeto. O que esse programa faz é imprimir a frase "hello, world" e pular uma linha no terminal.

A primeira coisa que fizemos foi incluir a biblioteca padrão de entrada e saída `stdio.h`. Não conseguiriamos utilizara função `printf` sem ela e é ela que imprime as coisas.

Depois, declaramos a função `main` que é necessária pro compilador saber por onde começar a executar os códigos. Ela precisa retornar um inteiro (retorno do tipo `int`), então passamos o valor `0` como retorno, pois qualquer valor diferente de `0` é entendido como um erro.

Por último, adicionamos a função `printf` que vai receber 2 argumentos, nesse caso. 

O primeiro é uma string que define o formato. Nesse caso, foi `"%s\n"` que diz a função:

1. `%s`: espero que o próximo argumento seja uma string.
1. `\n`: quando for imprimir esse caractere pule uma linha.

O segundo argumento é o nosso `"hello, world!"`

# Como compilar?

Para compilar, você precisa do clang instalado em sua máquina e rodar:

```sh
clang --pedantic -std=c89 ./main.c -o program && ./program
```

ou, se tiver _make_ instalado, basta rodar de dentro dessa pasta:

```sh
make && make run
```
