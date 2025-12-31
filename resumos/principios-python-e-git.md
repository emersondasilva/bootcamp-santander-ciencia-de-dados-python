# Princípios de Python – Introdução e Ambiente de Desenvolvimento

## 🎯 Objetivo do Módulo

Apresentar a linguagem Python, sua origem, características, principais áreas de aplicação e orientar na configuração do ambiente de desenvolvimento para iniciar os estudos e projetos.

## 📚 Introdução ao Python

### 🔹 O que é Python?
Python é uma linguagem de programação de alto nível, interpretada, de tipagem dinâmica e forte, criada com foco em simplicidade, legibilidade e produtividade.

É amplamente utilizada em:

* Ciência de Dados
* Automação
* Desenvolvimento Web
* Inteligência Artificial
* Scripts e tarefas do dia a dia

### 🕰️ Origem e História do Python

* Python nasceu em 1989, criado por Guido van Rossum
* Inicialmente desenvolvido como um hobby
* Inspirado na linguagem ABC, criada no Centro de Pesquisa Holandês (CWI)
* Primeira versão pública lançada em 1991 (v0.9.0)

## 🎯 Objetivos iniciais da linguagem

* Ser simples e intuitiva
* Código aberto
* Código legível, próximo da linguagem humana (inglês)
* Alta produtividade para tarefas cotidianas

## 📈 Evolução da linguagem

* 1991 – Primeira versão pública (0.9.0)
* 1995 – Versão 1.2
* 2000 – Lançamento do Python 2
* 2001 – Criação da Python Software Foundation (PSF)
* 2008 – Lançamento do Python 3
* Atualmente, o Python segue evoluindo na linha 3.x

## 🌎 Onde usar Python
Python é uma linguagem extremamente versátil:

### 🔹 Principais características

* Tipagem dinâmica e forte
* Multiplataforma
* Multiparadigma
* Comunidade grande e ativa
* Curva de aprendizado baixa

### ⚠️ Observação
Não é indicada para desenvolvimento nativo de aplicativos mobile.

## 🖥️ Configuração do ambiente de desenvolvimento

### 🔹 Linux e macOS

Normalmente o Python já vem instalado.  
Para verificar a versão:

```bash
python -V
python3 -V
```

### 🔹 Windows

* [ Acesse o site oficial ](https://www.python.org/)
* Baixe o instalador
* Siga o tutorial de instalação
* Durante a instalação, marque a opção Add Python to PATH

## 🧑‍💻 IDE (Ambiente de Desenvolvimento)

### 🔹 IDE recomendada
Visual Studio Code (VS Code)

### 🔹 Motivos da escolha

* Gratuito
* Suporte a múltiplas linguagens
* Boa performance
* Grande quantidade de extensões

Alternativamente, pode-se usar o PyCharm, mas o VS Code será a minha ferramenta principal.

## 🧱 Tipos de Dados em Python

### 🔹 O que são tipos? 

Os tipos definem:  

* As características de um valor
* O comportamento desse valor
* As operações que podem ser realizadas
* A forma como o valor é armazenado na memória

## ❓ Por que usamos tipos?

* Garantem operações corretas
* Definem o consumo de memória
* Permitem que o interpretador entenda como manipular os dados

## 🔢 Tipos Numéricos

### 🔸 Inteiros (int)

* Representam números inteiros
* Possuem precisão ilimitada

Exemplos:
```python
1
10
-100
```

### 🔸 Ponto flutuante (float)

* Representam números racionais (com casas decimais)

Exemplos
```python
1.5
-10.543
0.76
```
## 🔘 Booleanos e Strings

### 🔸 Booleanos (bool)

Representam valores lógicos:

* ```True```  

* ```False```

Em Python:

* ```True``` equivale a 1
* ```False``` equivale a 0
* Qualquer número diferente de zero é considerado verdadeiro

### 🔸 Strings (str)

Representam textos ou cadeias de caracteres.

Podem ser definidas com:

* Aspas simples
* Aspas duplas
* Aspas triplas

Exemplos:
```python
"Python"
'Python'
"""Python"""
'p'
```
## 🧪 Modo Interativo do Python

### 🔹 O que é o modo interativo?

O modo interativo permite escrever comandos Python diretamente no interpretador e visualizar o resultado imediatamente, sendo muito útil para testes rápidos e aprendizado.

### ▶️ Como iniciar o modo interativo

Iniciando apenas o interpretador:
```bash
python
```
Executando um script e mantendo o interpretador ativo:
```bash
python -i app.py
```

### 🧠 Vantagens do modo interativo

* Execução imediata dos comandos
* Ideal para testes rápidos
* Facilita o aprendizado da linguagem
* Não exige criação de arquivos

## 🔍 Funções ```dir()``` e ```help()```

### 🔹 Função ```dir()```

A função ```dir()``` retorna:  

* Sem argumentos: lista de nomes no escopo atual
* Com argumento: lista de atributos válidos de um objeto

Exemplos:
```python
dir()
dir(100)
```
### 🔹 Função ```help()```

A função ```help()``` invoca o sistema de ajuda integrado do Python, permitindo consultar documentação diretamente no terminal.

Exemplos:
```python
help()
help(100)
```
Essa funcionalidade permite acessar documentação offline, direto no interpretador.

## 🧮 Variáveis e Constantes

### 🔹 Variáveis

Variáveis são utilizadas para armazenar valores que podem ser alterados durante a execução do programa.

Em Python:

* Não é necessário declarar o tipo
* O tipo é inferido automaticamente
* Não é possível criar uma variável sem atribuir um valor

Exemplo:
```python
idade = 25
idade = 30
```
### 🔹 Constantes

Constantes são valores que não devem ser alterados durante a execução do programa. Python não possui palavra reservada para constantes.

A convenção utilizada é:

* Nome da constante em letras maiúsculas
```python
PI = 3.14159
TAXA_JUROS = 0.05
```
### 🧠 Boas práticas

* Utilizar snake_case para nomes de variáveis
* Escolher nomes claros e significativos
* Utilizar letras maiúsculas para constantes
* Evitar nomes genéricos como ```x```, ```y```, ```temp```

