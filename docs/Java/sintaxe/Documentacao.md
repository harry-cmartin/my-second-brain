# **Documentação Java - Sintaxe**

## *Tags*


Quais as informações que obtemos através de classes documentadas na linguagem ? Java Documentation é composto por tags que representam dados relevantes para a compreensão da proposta de uma classe e os conjunto de seus métodos e atributos conforme tabela abaixo:

| Tag        | Descrição                                               |
| ---------- | ------------------------------------------------------- |
| `@author`  | Autor / Criador                                         |
| `@version` | Versão do recurso disponibilizado                       |
| `@since`   | Versão ou data de início da disponibilização do recurso |
| `@param`   | Descrição dos parâmetros dos métodos criados            |
| `@return`  | Definição do tipo de retorno de um método               |
| `@throws`  | Indica que o método pode lançar uma exceção             |

## **Exemplo Completo**

=== "Código Java"

    ```java
    /**
     * <h1>Calculadora</h1>
     * A Calculadora realiza operações matemáticas entre números inteiros
     * <p>
     * <b>Note:</b> Leia atentamente a documentação desta classes
     * para desfrutar dos recursos oferecidos pelo autor
     *
     * @author  Harryson Campos
     * @version 1.0
     * @since   01/01/2026
     */
    public class Calculadora {
        /**
         * Este método é utilizado para somar dois números inteiros
         * @param numeroUm este é o primeiro parâmetro do método
         * @param numeroDois este é o segundo parâmetro do método
         * @return int o resultado deste método é a soma dos dois números.
         */
        public int somar(int numeroUm, int numeroDois) {
            return  numeroUm + numeroDois;
        }
    }
    ```

=== "Pop-up no VS Code"

    Esta é a forma como o VS Code exibe a leitura do comentário estruturado com Javadoc quando alguém tenta usar a função.

    ![Documentacao](../../../assets/images/DocumentacaoPopup.jpg)

## **Tipos de Comentários**

=== "In line"

    ```java
    // Olá, eu sou um comentário em uma única linha
    ```
=== "Multi Line"

    ```java
    /* Olá,
    * Eu sou um comentario
    * que posso ser mais detalhadod
    * quando necessário
    */
    ```
=== "Docs"

    ```java
    /** 
     * Estas duas estrelinhas acima
     * é para identificar que você
     * pretende elaborar um comentário
     * a nível de documentação.
     * Que incrível !!!
     */
    ```





#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |