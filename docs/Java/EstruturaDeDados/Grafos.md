# **Grafos**

Um grafo é uma estrutura de dados não linear formada por um conjunto de **vértices** (ou nós) conectados por **arestas** (linhas ou conexões). Se você parar para pensar, a árvore que vimos anteriormente é, na verdade, um tipo específico de grafo (um grafo conectado e sem ciclos). No entanto, enquanto as árvores possuem uma hierarquia rígida de "pai e filho", os grafos são completamente livres: qualquer nó pode se conectar a qualquer outro nó, criando uma teia complexa de interações.

## **Onde isso é aplicado?**

Os grafos são possivelmente a estrutura de dados mais importante para modelar o mundo real. Sempre que houver a necessidade de mapear **relacionamentos**, um grafo é a melhor escolha. Por exemplo:

* **Redes Sociais:** No LinkedIn ou Facebook, cada usuário é um vértice. Quando você adiciona alguém como amigo, uma aresta é criada entre vocês. O algoritmo que sugere "Pessoas que você talvez conheça" navega por esse grafo procurando vértices que estão a "dois pulos" de distância de você.
* **GPS e Mapas:** No Google Maps, cada cruzamento ou cidade é um vértice e as ruas são as arestas. O aplicativo calcula a melhor rota varrendo esse grafo.
* **Sistemas de Recomendação:** Lojas como Amazon ou serviços como Netflix usam grafos (comprador conectado a produto) para deduzir que "pessoas que compraram o produto A também compraram o B".

```java
package Grafos;

import java.util.*;

public class Grafo {
    
    // Usando o conceito de "Lista de Adjacência" para representar o grafo.
    // Cada vértice (chave) aponta para uma lista de vértices conectados a ele.
    private Map<Integer, List<Integer>> adjacencias;

    public Grafo() {
        this.adjacencias = new HashMap<>();
    }

    // Adiciona um novo vértice (nó) isolado ao grafo
    public void adicionarVertice(int vertice) {
        adjacencias.putIfAbsent(vertice, new ArrayList<>());
    }

    // Adiciona uma aresta (conexão) entre dois vértices
    public void adicionarAresta(int origem, int destino) {
        // Garante que ambos os vértices existam no grafo
        adicionarVertice(origem);
        adicionarVertice(destino);
        
        // Como é um grafo não direcionado (mão dupla), conectamos ambos os lados
        adjacencias.get(origem).add(destino);
        adjacencias.get(destino).add(origem); 
    }

    // Método principal 1: Imprimir a estrutura visualmente
    public void imprimirGrafo() {
        for (Integer vertice : adjacencias.keySet()) {
            System.out.print("Vértice " + vertice + " está conectado a: ");
            System.out.println(adjacencias.get(vertice));
        }
    }

    // Método principal 2: Busca em Largura (BFS - Breadth-First Search)
    // Olha só quem voltou: usamos uma FILA para ajudar na busca!
    public void buscaEmLargura(int inicio) {
        if (!adjacencias.containsKey(inicio)) return;

        Set<Integer> visitados = new HashSet<>();
        Queue<Integer> fila = new LinkedList<>();

        fila.add(inicio);
        visitados.add(inicio);

        System.out.print("Caminho percorrido (BFS): ");
        
        while (!fila.isEmpty()) {
            int verticeAtual = fila.poll(); // Remove o primeiro da fila
            System.out.print(verticeAtual + " ");

            // Explora todos os vizinhos do vértice atual
            for (int vizinho : adjacencias.get(verticeAtual)) {
                if (!visitados.contains(vizinho)) {
                    visitados.add(vizinho);
                    fila.add(vizinho); // Coloca o vizinho no fim da fila
                }
            }
        }
        System.out.println();
    }
}

```

## **Grafos Direcionados vs Não Direcionados**

Na implementação acima, nós adicionamos a conexão de "A para B" e de "B para A". Isso é um **Grafo Não Direcionado**, o que faz sentido para uma amizade no Facebook (se eu sou seu amigo, você obrigatoriamente é meu amigo).

Porém, existem os **Grafos Direcionados** (Digraphs). Pense no Instagram ou Twitter/X: você pode seguir uma celebridade, mas ela não necessariamente segue você de volta. A conexão é uma rua de mão única.

Além da direção, as arestas de um grafo podem ter **Pesos** (Weighted Graphs). No Google Maps, a aresta entre dois vértices (cruzamentos) possui um peso que representa a distância em quilômetros ou o tempo em minutos.

## **Algoritmos de Busca: Juntando tudo**

Navegar em grafos exige muito cuidado porque, ao contrário das árvores, os grafos podem ter ciclos (um caminho que dá voltas infinitas). Por isso, sempre precisamos manter um registro dos nós já `visitados` no código, como você pode ver na função `buscaEmLargura`.

Curiosamente, as estruturas que vimos antes são a alma da navegação de grafos:

* **Busca em Largura (BFS):** Utiliza uma **Fila (Queue)**. Ele explora todos os vizinhos imediatos antes de ir mais longe. É excelente para encontrar o caminho mais curto em grafos sem peso. Sua complexidade de tempo é de $O(V + E)$ (Vértices + Arestas).
* **Busca em Profundidade (DFS):** Utiliza uma **Pilha (Stack)** ou a pilha de chamadas da recursão. Ele vai o mais longe possível em um caminho antes de dar um passo para trás e tentar o próximo.

Para encontrar o caminho mais curto e rápido considerando *pesos* (como o GPS faz para driblar o trânsito), o mundo utiliza algoritmos mais complexos baseados na Busca em Largura, sendo o **Algoritmo de Dijkstra** o mais famoso e amplamente implementado em serviços de roteamento global.



#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |