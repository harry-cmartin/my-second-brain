# **Tabelas Hash (Hash Tables)**

Uma Tabela Hash (ou Dicionário/Mapa) é uma estrutura de dados construída com um objetivo bem claro: **velocidade extrema**. Ela funciona baseada em pares de **Chave-Valor** (Key-Value).

Pense nela como um guarda-volumes de um parque de diversões. Quando você entrega sua mochila, o atendente não guarda onde ele quiser e te faz procurar depois. Ele te entrega uma pulseira com o número exato do armário (a Chave). Quando você volta e entrega a pulseira, ele vai direto no armário específico e pega sua mochila (o Valor). Não há necessidade de procurar de um em um; a busca é imediata.

Na computação, usamos uma **Função de Hash** para converter qualquer chave (como uma palavra, um email ou um CPF) em um número inteiro, que será usado como o "número do armário" (o índice em um array) onde o dado será guardado.

## **Onde isso é aplicado?**

As Tabelas Hash são aplicadas em cenários onde você precisa recuperar informações instantaneamente usando um identificador único. A complexidade de tempo de busca ideal de uma Tabela Hash é de incríveis $O(1)$ (tempo constante).

* **Cache de Dados:** Quando você acessa a página de um produto, o servidor precisa carregar foto, preço e estoque do banco de dados (o que é demorado). Sistemas modernos usam Hash Tables na memória RAM para guardar o resultado dessa busca. Se outro usuário acessar o mesmo produto logo depois, o sistema pega o dado do Cache instantaneamente usando o ID do produto como chave.
* **Compiladores e Interpretadores:** Quando você declara uma variável no seu código, a linguagem de programação guarda o nome dela e o valor em uma Tabela Hash (chamada de Tabela de Símbolos) para saber onde achá-la instantaneamente enquanto executa o seu programa.
* **Bancos de Dados NoSQL:** Bancos como o MongoDB ou DynamoDB utilizam conceitos de pares Chave-Valor baseados em Hash para entregar altíssima performance em leituras.

```java


```

## **O Problema das Colisões**

No código acima, temos o método `calcularHash`. Como o array (o nosso guarda-volumes) tem um tamanho limitado, mas as chaves possíveis são infinitas, é matematicamente certo que uma hora **duas chaves diferentes vão gerar o mesmo índice**. Quando o sistema tenta colocar dois valores diferentes na mesma "gaveta", chamamos isso de **Colisão**.

Para resolver isso, usamos um conceito que você já aprendeu: **Listas Encadeadas**. No método `put`, quando ocorre uma colisão, nós não apagamos o valor antigo; nós transformamos aquele índice em uma pequena lista e "penduramos" (encadeamento ou *chaining*) a nova entrada na última. Quando vamos buscar (no método `get`), vamos até o índice e percorremos aquela pequena lista até achar a chave exata.

Se houverem muitas colisões (uma função hash ruim), a estrutura perde sua magia de ser $O(1)$ e vira apenas uma lista lenta de busca $O(n)$. Por isso uma boa matemática por trás do cálculo do Hash é vital. Em versões modernas do Java (a partir do Java 8), se essa pequena lista de colisões ficar muito grande, o próprio Java a converte automaticamente numa **Árvore Red-Black** (que você viu na nossa conversa sobre Árvores) para manter a busca sempre muito rápida.

## **Serviços de Infraestrutura (O ecossistema em larga escala)**

Assim como nas filas de mensagens, ninguém reinventa Tabelas Hash em sistemas distribuídos de larga escala do zero.

Se você tem centenas de servidores precisando acessar dados ultrarrápidos, você utiliza serviços que funcionam como "Tabelas Hash Globais" e ficam hospedados diretamente na memória RAM das máquinas (para serem milhares de vezes mais rápidos que buscar no HD). Os gigantes do mercado para isso são o **Redis** e o **Memcached**. Quase todo grande aplicativo que você utiliza (Twitter, Netflix, Uber) usa o Redis massivamente para armazenar as sessões dos usuários, rankings em tempo real e qualquer dado que não pode esperar os milissegundos de um banco de dados tradicional para carregar.

Implementação em JAVA muito boa [link](https://mauricio.github.io/2020/10/15/implementando-uma-hashtable-em-java.html)

#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |
