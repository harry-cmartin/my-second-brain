
# **HashSet e HashMap: Entendendo as Diferenças e Funcionamento em Java**

O HashSet e o HashMap são estruturas de dados em Java que utilizam hashing para armazenar e recuperar elementos rapidamente. A principal diferença é que o HashSet armazena apenas valores únicos, enquanto o HashMap armazena pares de chave e valor. 

## **O Mecanismo de Hashing (Como funcionam por trás)**

Ambos usam uma tabela de dispersão (hash table): 

   1. O Hash Code: Quando você adiciona um objeto, o Java chama o método .hashCode() desse objeto. Isso gera um número inteiro.
   2. O "Bucket": Esse número é usado para determinar em qual "balde" (bucket) da memória o dado será guardado.
   3. Colisões: Se dois objetos diferentes gerarem o mesmo hash code, eles serão colocados no mesmo bucket (formando uma lista). Nesse caso, o Java usa o método .equals() para verificar qual é o objeto correto.
   4. Desempenho: O acesso aos elementos é feito em tempo constante, ou seja, $\mathcal{O}(1)$ no melhor dos casos. 

------------------------------
## **HashSet**

* O que é: Uma coleção que implementa a interface Set.
* Objetivo: Armazenar coleções de objetos únicos (não permite duplicatas).
* Como funciona: O HashSet é construído utilizando um HashMap internamente! Cada elemento que você adiciona ao HashSet vira uma chave no HashMap, e o Java atribui a todos eles um valor fictício constante (geralmente chamado de PRESENT).
* Ordem: Não garante nenhuma ordem específica dos elementos.
* Exemplo:

```java

    HashSet<String> frutas = new HashSet<>();
    frutas.add("Maçã");
    frutas.add("Banana");
    frutas.add("Maçã"); // Esta linha é ignorada, pois "Maçã" já existe!

```

------------------------------
## **HashMap**

* O que é: Uma estrutura que implementa a interface Map (funciona como um dicionário).
* Objetivo: Associar dados a um identificador específico (pares de chave e valor).
* Como funciona: As chaves devem ser únicas. Se você inserir um valor com uma chave que já existe, ele sobrescreverá o valor antigo. Os valores associados podem ser duplicados.
* Ordem: Não garante a ordem das chaves.
* Exemplo:


```java
HashMap<Integer, String> contatos = new HashMap<>();
contatos.put(101, "João");
contatos.put(102, "Maria");

String nome = contatos.get(101); // Retorna "João"

```

------------------------------
## Quando usar qual?

* Use HashSet quando você precisa garantir que não existam elementos repetidos em uma lista e precisa verificar rapidamente se um item existe nela. 
* Use HashMap quando você precisa buscar, atualizar ou remover dados associados a um identificador único (Ex: ID do usuário -> Objeto do usuário). 

------------------------------


#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |