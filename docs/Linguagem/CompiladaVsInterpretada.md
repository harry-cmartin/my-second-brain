
## **Linguagens de Programação: Compilada vs Interpretada**


## Python

Na interpretada há um interpratador nativo da linguagem que traduz o codigo em Runtime para instrucoes que o SO entende, que manda para o hardware, processo é mais lento, Obs: o python por baixo dos panos gera um bytecode invisivel .pyc

O interpretador lê o seu código sequencialmente. Ele analisa o comando, traduz para instruções que o sistema operacional entende e já manda executar, tudo em tempo real, consumindo recursos.

## C

Na compilada, o compilador compila o código direto para o código de maquina (binário), copila o código inteiro e não vai fazendo em tempo de execução, no C por exemplo gera o executavel do código, essa abordagem só funciona em arquiteturas definidas, se a arquitetura do processador for diferente não consegue entender.

## Java

Resolve o problema usando uma abordagem de duas etapas, combinando compilação e interpretação/JIT.

**1. A Fase de Desenvolvimento: O que é o Bytecode?** Quando você compila um código Java, o compilador não gera um código de máquina para o seu Windows, Mac ou Linux. Ele gera o **Bytecode**.

- **O que é o Bytecode em si?** É um código intermediário, um conjunto de instruções altamente otimizadas que se parecem com código de máquina, mas **não são feitas para um processador físico**. Elas são feitas para um "processador imaginário", que é a Virtual Machine. É por isso que arquivos `.class` ou pacotes que usamos em projetos Java podem ser movidos de um computador para outro sem precisar recompilar.
    

**2. A Fase de Execução (Runtime): A Máquina Virtual (JVM)** Quando você vai rodar o programa, entra em cena a JVM (Java Virtual Machine). Como a imagem mostra dentro da caixa amarela, a JVM recebe o Bytecode e tem duas ferramentas para lidar com ele:

- **Interpreter (Interpretador):** A JVM pode simplesmente ler o bytecode linha por linha e traduzir para o Sistema Operacional na hora, parecido com o que o Python faz.
    
- **JIT Compiler (Just-in-Time):** Aqui está a "mágica" do desempenho. A JVM é inteligente; ela percebe quais partes do seu bytecode são executadas muitas vezes (os chamados _hot spots_). Em vez de ficar interpretando essas mesmas linhas repetidamente, o JIT Compiler entra em ação **durante a execução** e compila aquele trecho específico de bytecode diretamente para Código de Máquina puro.
    

O resultado disso é que o Java consegue a portabilidade ("Escreva uma vez, rode em qualquer lugar" graças ao Bytecode) e ainda atinge um desempenho muito alto (graças ao JIT Compiler transformando o código em linguagem de máquina nativa em tempo real). O sistema operacional e o hardware final recebem apenas as instruções mastigadas e prontas para o processador físico.



## Bibliografia 

>  

## Histórico de Versões

| Versão |    Data    | Descrição            | Autor(es)                                    | Revisor(es) |
| ------ | :--------: | -------------------- | -------------------------------------------- | ----------- |
| 1.0    | 30/05/2026 | Criação do documento | [Harryson](https://github.com/harry-cmartin) |             |
