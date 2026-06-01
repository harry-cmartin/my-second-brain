
# **Árvores**

Uma árvore é uma estrutura de dados não linear e hierárquica, formada por conexões de nós (nodes). Diferente das listas ou filas, onde os dados ficam organizados em uma sequência, na árvore existe um nó principal chamado de "raiz" (root). A partir dessa raiz, a estrutura se ramifica para outros nós "filhos", terminando finalmente nos nós que não têm filhos, chamados de "folhas" (leaves). Pense na árvore genealógica da sua família ou na forma como as pastas estão organizadas no seu sistema operacional, com pastas dentro de pastas.

## **Onde isso é aplicado?**

A árvore é uma das estruturas mais fundamentais da computação e é base para resolver problemas onde a hierarquia e a rápida recuperação de informações são cruciais. Por exemplo:

**Sistemas de Arquivos:** Quando você navega pelo Windows ou Linux, a estrutura de diretórios do sistema é uma grande árvore. O diretório raiz (como o `C:\`) se divide em pastas, que se dividem em subpastas e finalmente nos arquivos (as folhas).

**DOM (Document Object Model):** Sempre que você acessa um site, o seu navegador transforma o código HTML em uma árvore de elementos. O elemento `<html>` é a raiz, se dividindo em `<head>` e `<body>`, que por sua vez contêm textos, imagens e botões. É manipulando essa árvore que o JavaScript consegue alterar o que você vê na tela.

```java
    package Arvores;

    public class TreeNode {

        private int valor;
        private TreeNode esquerda;
        private TreeNode direita;

        public TreeNode(int valor, TreeNode esquerda, TreeNode direita) {
            this.valor = valor;
            this.esquerda = esquerda;
            this.direita = direita;
        }

        public int getValor() {
            return valor;
        }

        public void setValor(int valor) {
            this.valor = valor;
        }

        public TreeNode getEsquerda() {
            return esquerda;
        }

        public void setEsquerda(TreeNode esquerda) {
            this.esquerda = esquerda;
        }

        public TreeNode getDireita() {
            return direita;
        }

        public void setDireita(TreeNode direita) {
            this.direita = direita;
        }
}

```

```java

    package Arvores;

    public class BinaryTree {

        // Adicionado um atributo raiz para controlar o início da árvore corretamente
        private TreeNode raiz;

        public TreeNode getRaiz() {
            return raiz;
        }

        // Método público auxiliar para facilitar a chamada externa sem precisar passar a raiz
        public void add(int valor) {
            if (this.raiz == null) {
                this.raiz = new TreeNode(valor, null, null);
            } else {
                addNode(this.raiz, valor);
            }
        }

        public void addNode(TreeNode head, int valor) {
            // assumindo que nunca terão valores repetidos
            TreeNode novo = new TreeNode(valor, null, null);

            if (head == null) {
                return;
            }

            if (valor > head.getValor()) {
                if (head.getDireita() == null) {
                    head.setDireita(novo);
                    return;
                } else {
                    addNode(head.getDireita(), valor);
                }
            } else if (valor < head.getValor()) {
                if (head.getEsquerda() == null) {
                    head.setEsquerda(novo);
                    return;
                } else {
                    addNode(head.getEsquerda(), valor);
                }
            }
        }

        public TreeNode search(TreeNode head, int valor) {
            if (head == null) {
                return null;
            }

            if (head.getValor() == valor) {
                return head;
            }

            if (valor < head.getValor()) {
                return search(head.getEsquerda(), valor);
            } else if (valor > head.getValor()) {
                return search(head.getDireita(), valor);
            }

            return null;
        }

        // ==========================================
        // IMPLEMENTAÇÃO DA REMOÇÃO
        // ==========================================

        public void remove(int valor) {
            this.raiz = removeNode(this.raiz, valor);
        }

        private TreeNode removeNode(TreeNode head, int valor) {
            if (head == null) {
                return null;
            }

            // 1. Procurar o nó a ser removido
            if (valor < head.getValor()) {
                head.setEsquerda(removeNode(head.getEsquerda(), valor));
            } else if (valor > head.getValor()) {
                head.setDireita(removeNode(head.getDireita(), valor));
            } else {
                // Encontrou o nó! Agora aplica as regras de remoção:

                // Caso 1: Nó folha (não tem filhos)
                if (head.getEsquerda() == null && head.getDireita() == null) {
                    return null;
                }

                // Caso 2: Nó com apenas um filho (à direita ou à esquerda)
                if (head.getEsquerda() == null) {
                    return head.getDireita();
                } else if (head.getDireita() == null) {
                    return head.getEsquerda();
                }

                // Caso 3: Nó com dois filhos
                // Usando a estratégia pedida: buscar o maior valor da subárvore esquerda
                TreeNode maiorEsquerda = buscaMaiorDaEsquerda(head.getEsquerda());
                
                // Copia o valor do substituto para o nó atual
                head.setValor(maiorEsquerda.getValor());
                
                // Remove recursivamente o nó substituto que ficou duplicado na subárvore esquerda
                head.setEsquerda(removeNode(head.getEsquerda(), maiorEsquerda.getValor()));
            }

            return head;
        }

        // Método auxiliar para encontrar o maior elemento à esquerda
        // O maior elemento sempre estará o mais à direita possível daquela subárvore
        private TreeNode buscaMaiorDaEsquerda(TreeNode head) {
            if (head.getDireita() == null) {
                return head;
            }
            return buscaMaiorDaEsquerda(head.getDireita());
        }

        // ==========================================
        // IMPLEMENTAÇÃO DO PRINT
        // ==========================================

        public void printTree() {
            printTreeFormatado(this.raiz, "", true);
        }

        // Método que desenha a árvore no terminal mostrando visualmente a hierarquia
        private void printTreeFormatado(TreeNode no, String prefixo, boolean ehEsquerdo) {
            if (no != null) {
                System.out.println(prefixo + (ehEsquerdo ? "├── " : "└── ") + no.getValor());
                
                // Passa o prefixo para os nós filhos montarem a estrutura de árvore textual
                printTreeFormatado(no.getEsquerda(), prefixo + (ehEsquerdo ? "│   " : "    "), true);
                printTreeFormatado(no.getDireita(), prefixo + (ehEsquerdo ? "│   " : "    "), false);
            }
        }
}


```

## **Busca Binária em Árvore**

O método `buscar` no código acima ilustra um conceito poderoso: a **Busca Binária em Árvore** (Binary Search Tree - BST). Em uma BST, existe uma regra de ouro: para qualquer nó, todos os valores à sua esquerda são *menores* que ele, e todos à sua direita são *maiores*.

Por causa dessa regra, procurar um valor em uma árvore binária de busca é como procurar uma palavra em um dicionário físico: você abre no meio; se a palavra que você quer vem antes no alfabeto, você ignora a segunda metade do livro inteiro. A cada passo na árvore, você descarta metade dos nós restantes, tornando a busca extremamente rápida, com uma complexidade de tempo de $O(\log n)$.

## **Bancos de Dados e Infraestrutura**

Assim como não implementamos sistemas completos de filas do zero, na vida real dificilmente você vai programar uma árvore do zero no seu dia a dia profissional, mas você usará os serviços que dependem delas o tempo todo.

Os **Sistemas de Bancos de Dados** (como PostgreSQL, MySQL, SQL Server) são completamente dependentes de árvores. Quando você cria um "Índice" (Index) em uma tabela para deixar suas consultas SQL mais rápidas, o banco de dados está, na verdade, construindo uma árvore gigantesca por trás dos panos (geralmente uma B-Tree) para armazenar as referências dos seus dados. Sem árvores, os bancos de dados teriam que ler a tabela inteira a cada busca, inviabilizando aplicações modernas.

## **Outros tipos de árvore**

A árvore binária clássica possui um calcanhar de Aquiles: se você inserir dados que já estão em ordem (ex: 1, 2, 3, 4, 5), ela vai crescer apenas para o lado direito, se transformando em uma grande "linha reta" (uma lista encadeada), o que destrói a eficiência da busca binária.

Para evitar isso, existem as **árvores autobalanceadas**, sendo a **Árvore Red-Black (Rubro-Negra)** uma das mais famosas. Uma árvore Red-Black usa um conjunto estrito de regras matemáticas e de cores (onde cada nó recebe uma "cor", vermelha ou preta) para garantir que a árvore se reestruture automaticamente após cada inserção ou remoção. Ela faz "rotações" com os nós para garantir que a árvore nunca fique muito profunda de um lado só. Sistemas modernos, linguagens de programação e até o kernel do sistema operacional Linux usam árvores Red-Black para gerenciar processos e alocação de memória por causa da sua consistência e velocidade garantida.

Outro exemplo comum de árvore autobalanceada é a **Árvore AVL**, que é ainda mais rígida com o seu balanceamento do que a Red-Black, sendo excelente para aplicações onde você faz muito mais buscas do que inserções.


#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |
