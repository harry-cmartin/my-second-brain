# **Pilhas**

Uma pilha (Stack) é uma coleção de itens ordenada baseada no conceito de LIFO (Last In First Out). Basicamente significa que o *último* a entrar na pilha será o *primeiro* a sair. Pense em uma pilha de pratos em um restaurante: você sempre pega o prato que está no topo e, quando o garçom traz pratos limpos, ele os coloca no topo da pilha. Novos itens sempre são adicionados (push) e removidos (pop) da mesma extremidade.

## **Onde isso é aplicado?**

A pilha é uma estrutura de dados fundamental e aparece em quase tudo que você utiliza no seu computador ou celular. Por exemplo:

* **Função "Desfazer" (Undo):** Quando você está digitando um texto no Word ou programando na sua IDE e aperta `Ctrl + Z`, o sistema está lendo uma pilha. Cada ação que você faz é empilhada. Ao pedir para desfazer, o programa remove (faz o *pop*) da última ação do topo e reverte o estado do arquivo.
* **Histórico do Navegador:** O botão de "Voltar" do seu navegador de internet funciona puramente com o conceito de pilha. Conforme você clica em links, as páginas vão sendo empilhadas. Quando você clica em voltar, a página atual é removida do topo e você volta para a que estava imediatamente abaixo dela.
* **Validação de expressões matemáticas:** Compiladores e calculadoras usam pilhas para verificar se os parênteses `()` ou chaves `{}` de uma expressão ou bloco de código foram abertos e fechados na ordem correta.

```java
package Pilhas;

import java.util.List;

public class Stack {


    public void push(List<Integer> y , int x){

        if(y != null){
            y.add(x);
        }
    }


    public void pop(List<Integer> y){

        if (y != null){
            y.remove(y.size() - 1);
        }else{
            System.out.println("Pilhas.Stack is empty");
        }
    }

    public int numberOfElements(List y){
        return y.size() - 1;
    }


}

```

## **Sistemas e Execução**

A implementação usando uma lista em Java é bem simples, mas o conceito de pilha é a base para o funcionamento de praticamente qualquer linguagem de programação moderna através da **Call Stack** (Pilha de Chamadas).

Quando você roda um programa e a função `A` chama a função `B`, o computador "pausa" a função `A` e coloca todas as variáveis e o estado atual dela em uma pilha na memória RAM. Então, ele executa a função `B`. Quando a `B` termina, o computador faz um *pop* na pilha para recuperar o estado exato da função `A` e continuar de onde parou.

Se você fizer uma função recursiva que chama a si mesma infinitamente, o computador vai empilhar essas chamadas até a memória destinada à pilha acabar, gerando um erro fatal muito famoso entre os desenvolvedores: o **Stack Overflow** (Estouro de Pilha). A pilha tambem é usada para implementar recursao e o algoritmo **Busca em Profundidade** (Depth-First Search - DFS).


#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |

