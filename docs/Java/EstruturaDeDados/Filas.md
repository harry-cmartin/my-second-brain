# **Filas**

Uma fila é uma coleção de itens ordenada baseada no conceito de FIFO (First In First Out). Basicamente signfica que o primeiro a entrar na fila também é o primeiro a sair. Assim como acontece na fila do cinema, por exemplo. E os novos itens sempre são adicionados no final da fila.

## **Onde isso é aplicado?**

A fila é uma estrutura de dados bem útil e usada de várias formas durante o desenvolvimento de software. Por exemplo:

Fila de e-mails: é muito comum sua aplicação gerar e-mails para serem enviados usando uma cloud. Porém esses e-mails não são enviados diretamente. Eles entram em uma fila para serem processados e enviados ao seu destino.

Processamento de pagamentos: Imagine se você compra algo na amazon e por algum motivo o seu pagamento não é processado? Para conseguir lidar com a quantidade de pagamentos e ter a certeza de que ele será processado é possível usar uma fila para controlar isso.


```java

    package Listas;
    import java.util.List;

    public class Filas {
        
        public void enqueue(List<Integer> x , int y){

            if(x != null){
                x.add(0 , y);
            }

        }

        public boolean isEmpty(List<Integer> x){
            return x.isEmpty();
        }

        public void Remove(List<Integer> x){
            x.remove(x.size() - 1);
        }

        public void insereNomeio(List<Integer> x, int y){
            if(x != null){

                int tamanho = x.size();
                System.out.println(tamanho);
                x.add(tamanho/2 , y);

            }

        }

    }


```

## **Serviços**

Vimos que implementar e usar uma fila parece uma tarefa simples, porém usar uma fila em larga escala é uma tarefa bem complexa. Então é comum usar serviços para realizar essa tarefa, existem diversos serviços e formas de fazer como por exemplo o SQS da AWS, o RabbitMQ, o Apache Kafka, entre outros. Esses serviços são usados para criar filas de mensagens e processar essas mensagens de forma assíncrona.

## **Outros tipos de fila**

Também existe um outro tipo de fila chamada de Deque ou fila de duas pontas. Ela permite que você faça operações de remoção e inserção nas duas pontas da fila.


#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |
