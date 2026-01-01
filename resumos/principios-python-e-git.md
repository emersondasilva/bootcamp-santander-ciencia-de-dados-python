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

## 🔄 Conversão de Tipos em Python

### 🔹 O que é conversão de tipos?

Em alguns cenários, é necessário converter o tipo de uma variável para manipulá-la corretamente. Isso ocorre, por exemplo, quando um valor é recebido como string, mas precisa ser utilizado em uma operação matemática.

### 🔢 Conversões mais comuns

#### 🔸 Inteiro para ponto flutuante

```python
numero = 10
numero_float = float(numero)
```
#### 🔸 Ponto flutuante para inteiro

```python
valor = 9.7
valor_int = int(valor)
```
A conversão de ```float``` para ```int``` remove as casas decimais, não arredonda.

#### 🔸 Conversão por divisão

```python
resultado = 10 / 3
```
O resultado de uma divisão em Python sempre será float.

#### 🔸 Numérico para string

```python
idade = 25
idade_str = str(idade)
```
#### 🔸 String para número

```python
numero = int("10")
valor = float("3.14")
```
## ⚠️ Erro de conversão

Ocorre quando tentamos converter um valor incompatível:

```python
int("Python")
```
Gera um erro do tipo:

```
ValueError
```
## ⌨️ Funções de Entrada e Saída

### 🔹 Função ```input()```

A função ```input()``` é utilizada para ler dados da entrada padrão (teclado).

Características:


* Sempre retorna uma ```string```
* Pode exibir uma mensagem ao usuário

Exemplo:

```python
nome = input("Digite seu nome: ")
```
### 🔄 Convertendo o valor de entrada

Como ```input()``` retorna ```string```, é comum realizar conversão:

```python
idade = int(input("Digite sua idade: "))
```
## 🖨️ Função ```print()```

A função ```print()``` exibe informações na saída padrão (tela).

Exemplo simples:

```python
print("Olá, mundo!")
```
### 🔧 Parâmetros da função ```print()```

```python
print("Python", "é", "incrível", sep=" ", end="!")
```
Principais parâmetros:

* ```sep``` → separador entre os valores
* ```end``` → final da linha
* ```file``` → destino da saída
* ```flush``` → força a limpeza do buffer

# 🔧 Versionamento de Código com Git e GitHub

## 🎯 Objetivo

Introduzir os conceitos de versionamento de código e apresentar as ferramentas Git e GitHub, utilizadas para controle de versões e colaboração em projetos de software.

## 📌 O que é Versionamento de Código?

Versionamento de código é o processo de registrar, organizar e controlar as alterações feitas em arquivos ao longo do tempo.

Permite:

* Acompanhar histórico de mudanças
* Recuperar versões anteriores
* Trabalhar em equipe com segurança
* Evitar perda de código

## 🗂️ Sistemas de Controle de Versão (VCS)

Um VCS (Version Control System):

* Registra alterações nos arquivos
* Identifica autor, data e conteúdo das mudanças
* Controla diferentes versões de um projeto

### Tipos de VCS

#### 🔹 Centralizado (CVCS)

* Um servidor central armazena o histórico
* Exemplo: CVS, Subversion

#### 🔹 Distribuído (DVCS)

* Cada clone possui o histórico completo
* Permite trabalhar offline
* Maior segurança

Exemplos:
* Git
* Mercurial

## 🧠 O que é Git?

Git é um sistema de controle de versão distribuído.

Características:

* Gratuito e open source
* Leve e rápido
* Forte suporte a branches e merges
* Muito utilizado em projetos open source e corporativos

### 📜 Breve histórico do Git

* Criado em 2005 por Linus Torvalds
* Desenvolvido após a perda da licença do BitKeeper
* Criado para gerenciar o código do kernel Linux

## 🌐 O que é GitHub?

GitHub é uma plataforma de hospedagem de código que utiliza Git.

Permite:

* Armazenar repositórios remotos
* Colaboração entre desenvolvedores
* Controle de versões
* Issues, Pull Requests e documentação

📌 **Git ≠ GitHub**  
Git é a ferramenta de versionamento  
GitHub é a plataforma que hospeda repositórios Git

## 🔁 Fluxo básico do Git

```bash
git clone    #Clona um repositório remoto
git add      #Adiciona arquivos para o commit
git commit   #Registra as alterações
git pull     #Atualiza o repositório local
git push     #Envia alterações para o repositório remoto
```
## 🧪 Principais comandos Git

### 🔹 Inicializar um repositório

```bash
git init
```

### 🔹 Ver status dos arquivos

```bash
git status
```

### 🔹 Adicionar arquivos ao commit

```bash
git add arquivo.md
git add pasta/
```

### 🔹 Criar um commit

```bash
git commit -m "mensagem descritiva"
```

### 🔹 Enviar alterações para o GitHub

```bash
git push
```

### 🔹 Atualizar repositório local

```bash
git pull
```

## 🌿 Trabalhando com Branches

Branches são ramificações do projeto.

Permitem: 

* Desenvolver novas funcionalidades
* Testar código sem afetar a branch principal

Comandos básicos:

```bash
git branch
git checkout -b nova-branch
git branch -d nome-da-branch
```

## 🔐 Autenticação no GitHub

O GitHub não aceita mais senha para operações Git.

Formas de autenticação: 

* Token de acesso (PAT)
* Chave SSH

📌 Recomendado:

* Usar Token ou SSH
* Ativar autenticação em dois fatores (2FA)

## 📚 Boas práticas com Git

* Commits pequenos e frequentes
* Mensagens claras e objetivas
* Versionar apenas o que faz parte do projeto
* Manter o repositório organizado

## ✅ Conclusão do Módulo 01

Neste módulo foram abordados os fundamentos essenciais para o início do desenvolvimento com Python e o uso de versionamento de código, incluindo:

* Introdução ao Python e sua história
* Configuração do ambiente de desenvolvimento
* Tipos de dados
* Modo interativo
* Variáveis e constantes
* Conversão de tipos
* Entrada e saída de dados
* Conceitos de Git e GitHub
* Fluxo básico de versionamento

Esses conhecimentos formam a base necessária para avançar nos estudos de Ciência de Dados com Python e no desenvolvimento de projetos versionados.