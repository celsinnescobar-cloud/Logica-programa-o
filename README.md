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


## Como Executar o Script Shell (`calculadora.sh`)

O script `.sh` automatiza as mensagens de início/fim e a execução do programa em Python.


### Pré-requisitos
* Sistema Operacional Linux, macOS ou WSL no Windows.
* `python3` instalado na máquina.


### Passo a Passo:

1. **Atribuir permissão de execução ao script:**
   Antes de rodar pela primeira vez, defina as permissões de acesso ao arquivo `calculadora.sh`:
   ```bash
   chmod 744 calculadora.sh
