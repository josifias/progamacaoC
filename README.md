# 🚀 Minhas Primeiras Linhas em C++

Este repositório marca o início oficial dos meus estudos em programação! Hoje, dia 17 de maio de 2026, escrevi e executei meus primeiros códigos nesta linguagem.

## 📌 O que eu aprendi hoje:
* **Configuração de Ambiente:** Configurei o Visual Studio Code para compilar arquivos `.c` e `.cpp`.
* **Sintaxe Básica:** Entendi a estrutura inicial de um programa em C++ (incluindo bibliotecas e a função principal `main`).
* **Saída de Dados:** Consegui fazer o clássico "Olá Mundo" aparecer no terminal.
* **Organização:** Aprendi a diferença entre o arquivo de código (`.c`) e o arquivo executável (aquele com ícone de lista/engrenagem).

## 🛠️ Ferramentas Utilizadas:
* **Linguagem:** C++
* **Editor:** Visual Studio Code (VS Code)
* **Controle de Versão:** Git & GitHub

---
*Este é um projeto de aprendizado constante. Próximo passo: Entender variáveis e entrada de dados!*
# 🚀 Aprendendo Variáveis e Tipos de Dados em C++

Este repositório foi criado para registrar a minha jornada de aprendizado em programação, focando nos conceitos fundamentais de **variáveis** e **tipos de dados** utilizando a linguagem C++.

## 📌 O que estou aprendendo?

### 1. Variáveis
Entendi que uma variável funciona como uma caixa na memória do computador onde podemos guardar uma informação para usar mais tarde. Em C++, aprendi a:
* **Declarar** uma variável definindo seu tipo obrigatoriamente (Linguagem fortemente tipada).
* **Atribuir** um valor usando o operador `=`.
* **Manipular** os valores armazenados ao longo do código.

### 2. Tipos de Dados em C++
Cada informação guardada tem um tipo específico. Os principais tipos primitivos que estou estudando são:
* `string` / `char`: Para textos e caracteres simples (ex: `"Olá, Mundo!"`, `'A'`).
* `int`: Para números inteiros (ex: `10`, `-5`).
* `float` / `double`: Para números com casas decimais (ex: `19.99`, `3.14`).
* `bool`: Valores lógicos que representam apenas Verdadeiro (`true`) ou Falso (`false`).

## 🛠️ Tecnologias Utilizadas
* **Linguagem de Programação:** C++
* Compilador (ex: GCC / G++)
* Git e GitHub para controle de versão.


# 🚀 Aprendendo Entrada e Saída em Linguagem C

Este repositório contém meus primeiros passos na linguagem C, focando no domínio da manipulação de dados através do terminal. Aprendi a capturar informações do usuário, exibi-las formatadas na tela e gerenciar o comportamento do buffer do teclado.

## 🧠 Conceitos Aprendidos

### 1. Saída de Dados com `printf`
A função `printf` é utilizada para exibir textos e valores na tela. Para mostrar variáveis, aprendi a usar os **especificadores de formato**:
* `%d`: Números inteiros (`int`).
* `%.2f`: Números decimais (`float`), limitando a duas casas decimais.
* `%c`: Um único caractere (`char`).
* `%s`: Textos/Cadeias de caracteres (`strings`).

### 2. Entrada de Dados com `scanf`
A função `scanf` permite que o programa leia o que o usuário digita no teclado:
* É obrigatório o uso do operador `&` antes do nome das variáveis numéricas e de caracteres (ex: `&idade`).
* O `&` **não** é necessário ao ler strings (arrays de `char`), pois o nome da variável já representa seu endereço de memória.

### 3. Gerenciamento do Buffer do Teclado
Um dos maiores aprendizados foi entender como a memória do teclado armazena resíduos (como o caractere `\n` do Enter ou pontuações inesperadas) e como tratá-los:
* **Leitura de nomes compostos**: Uso do formato especial `scanf(" %[^\n]", nome);` para ler textos com espaços.
* **Limpeza universal do buffer**: Uso do laço `while (getchar() != '\n' && getchar() != EOF);` para descartar sujeiras no buffer antes de ler novos caracteres, evitando pulos de linha ou capturas incorretas (como vírgulas de números decimais).

---

## 💻 Exemplo Prático Desenvolvido

O código abaixo resume todos os conceitos aplicados de forma segura:

```c
#include <stdio.h>

int main() {
    int idade;
    float altura;
    char opcao;         
    char nome[30];

    // Lendo um número inteiro
    printf("Digite sua idade: ");
    scanf("%d", &idade);
    printf("Sua idade é: %d\n\n", idade);

    // Lendo uma string com espaços
    printf("Digite seu nome: ");
    scanf(" %[^\n]", nome); 
    printf("Seu nome é: %s\n\n", nome);

    // Lendo um número decimal (usar ponto para separar as casas: ex: 1.75)
    printf("Digite sua altura: ");
    scanf("%f", &altura);
    printf("Sua altura é: %.2f\n\n", altura);

    // Limpando o buffer de forma segura antes de ler um caractere
    while (getchar() != '\n' && getchar() != EOF); 

    // Lendo um caractere único
    printf("Digite sua opção: ");
    scanf(" %c", &opcao);
    printf("Opção escolhida: %c\n", opcao);

    return 0;
}
```

---

## 🛠️ Tecnologias e Ferramentas
* **Linguagem**: C (Padrão ANSI)
* **Compilador**: GCC / GDB
* **Ambiente**: VS Code

---
💡 *“A melhor forma de aprender a programar é praticando todos os dias!”*
