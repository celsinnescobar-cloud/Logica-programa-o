# Logica programação
Curso de Lógica de Programação em Python

---

# Calculadora em Python e Shell Script

Este repositório contém uma aplicação simples de uma calculadora desenvolvida em **Python** com automação de execução via **Shell Script (`.sh`)**.

O projeto realiza as operações matemáticas básicas (Soma, Subtração, Multiplicação e Divisão) contando com tratamento de exceções para entradas inválidas e divisão por zero.


---

## Estrutura do Projeto

* `calculadora.py` - Script principal em Python contendo a lógica da calculadora.
* `calculadora.sh` - Script em Shell (Bash) para inicialização automatizada da calculadora.

---


## Como Executar o Projeto (Passo a Passo Detalhado)

Siga as instruções abaixo de acordo com o seu sistema operacional para abrir o terminal e rodar o projeto.

---

### Passo 1: Abrir o Terminal

* **No Linux:**
  * Pressione o atalho de teclado: `Ctrl + Alt + T`
  * *Ou:* Abra o menu de aplicativos, digite **Terminal** e clique no ícone para abrir.



* **No Windows (usando Git Bash ou WSL):**
  * Abra o menu Iniciar, digite **Git Bash** (ou **Ubuntu** se usar WSL) e pressione a tecla **Enter**.

---

### Passo 2: Navegar até a pasta dos arquivos

Antes de executar, você precisa estar na pasta onde baixou ou salvou os arquivos `calculadora.py` e `calculadora.sh`.

1. Digite o comando `cd` seguido do nome/caminho da pasta.
   * *Exemplo (se esteve na pasta Downloads):*
     ```bash
     cd Downloads
     ```
2. Pressione a tecla **Enter**.
3. *(Dica)* Para ter certeza de que está na pasta certa, digite `ls` e pressione **Enter**. O terminal listará os arquivos salvos ali.

---

### Passo 3: Dar permissão de execução ao Script Shell

No Linux, scripts `.sh` precisam de permissão explícita para serem rodados.

1. Digite o comando:
   ```bash
   chmod 744 calculadora.sh


2. **Executando o Script**
No terminal, dentro da pasta do projeto digite:
   ```bash
   ./calculadora.sh

E após tecle Enter.



---


# Explicação do Código Python (calculadora.py)


O código executa duas rodadas de cálculos através de uma estrutura de repetição e garante que entradas incorretas não interrompam a aplicação.


**Principais Pontos da Implementação:**
Laço de Repetição (for i in range(2)):
   → Controla a execução do programa para rodar o fluxo da calculadora 2 vezes seguidas.

Entrada de Dados e Validação (try / except ValueError):
   → Utiliza a função float() para aceitar números inteiros e decimais (ex: 10 ou 5.5).

   → Caso o usuário digite letras ou caracteres inválidos, o bloco captura a exceção ValueError, exibe uma mensagem orientativa e usa o continue para reiniciar o ciclo com segurança.



**Operações Matemáticas:**

Executa diretamente os cálculos de Soma (+), Subtração (-) e Multiplicação (*).


**Tratamento de Divisão por Zero (try / except ZeroDivisionError):**

Realiza a Divisão (/) dentro de um bloco de teste try.

Se o segundo número for 0, o código captura o erro ZeroDivisionError e exibe a mensagem de aviso "Divisão: Não é possível dividir um número por zero!", evitando que o programa quebre.