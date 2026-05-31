# **Conceitos de POO**


Programação orientada a objetos (POO, ou OOP segundo as suas siglas em inglês) é um paradigma de programação baseado no conceito de "objetos", que podem conter dados na forma de campos, também conhecidos como atributos, e códigos, na forma de procedimentos, também conhecidos como métodos.

Como se trata de um contexto análogo ao mundo real, tudo no qual nos referimos são objetos, exemplo: Conta bancária, Aluno, Veículo, Transferência etc.

A programação orientada a objetos é bem requisitada no contexto das aplicações mais atuais no mercado devido a possibilidade de reutilização de código e a capacidade de representação do sistema ser muito mais próximo do mundo real.

Para uma linguagem ser considerada orientada a objetos, esta deve seguir o que denominamos como **Os quatro pilares da orientação a objetos**:

------------------------------------------------------------------------------------------------------------------------------------

- Encapsulamento: Nem tudo precisa estar visível, grande parte do nosso algoritmo pode ser distribuído em métodos com finalidades específicas que complementa uma ação em nossa aplicação.

Exemplo: Ligar um veículo exige muitas etapas para a engenharia, mas o condutor só visualiza a ignição, dar a partida e a “magia” acontece.

```java
public class SistemaIgnicao {

    // Método PÚBLICO: É a única coisa que o condutor (usuário) vê e interage.
    public void darPartida() {
        System.out.println("Girando a chave...");
        verificarBateria();
        injetarCombustivel();
        gerarFaisca();
        System.out.println("A magia acontece: Motor ligado! Vrum!");
    }

    // Métodos PRIVADOS: A complexidade da engenharia fica encapsulada (escondida).
    private void verificarBateria() {
        System.out.println("- Engenharia interna: Verificando tensão da bateria...");
    }

    private void injetarCombustivel() {
        System.out.println("- Engenharia interna: Bomba de combustível acionada...");
    }

    private void gerarFaisca() {
        System.out.println("- Engenharia interna: Velas de ignição disparando...");
    }
}

```

------------------------------------------------------------------------------------------------------------------------------------

- Abstração: É a indisponibilidade para determinar a lógica de um ou vários comportamentos em um objeto.

Exemplo: Veículo determina duas ações como acelerar e frear, logo estes comportamentos deverão ser abstratos pois existem mais de uma maneira de se realizar a mesma operação. ver Polimorfismo.


```java


// ABSTRAÇÃO: A classe é 'abstract' porque é um conceito genérico, não um objeto final.
public abstract class Veiculo {
    
    // HERANÇA (Propriedades comuns): Esses atributos serão herdados pelos filhos.
    protected String placa;
    protected String chassi;
    protected int anoFabricacao;

    public Veiculo(String placa, String chassi, int anoFabricacao) {
        this.placa = placa;
        this.chassi = chassi;
        this.anoFabricacao = anoFabricacao;
    }

    // ABSTRAÇÃO (Métodos): Determinam a ação, mas a lógica (o corpo do método) não existe aqui.
    public abstract void acelerar();
    public abstract void frear();
}

```

------------------------------------------------------------------------------------------------------------------------------------

- Herança: Características e comportamentos comuns podem ser elevados e compartilhados através de uma hierarquia de objetos.

Exemplo: Um Carro e uma Motocicleta possuem propriedades como placa, chassi, ano de fabricação e métodos como acelerar, frear. Logo para não ser um processo de codificação redundante, podemos desfrutar da herança criando uma classe Veiculo para que seja herdada por Carro e Motocicleta.

```java

// HERANÇA: Carro herda as propriedades de Veiculo
public class Carro extends Veiculo {

    public Carro(String placa, String chassi, int anoFabricacao) {
        super(placa, chassi, anoFabricacao); // Repassa os dados para a classe pai
    }


}

```


------------------------------------------------------------------------------------------------------------------------------------


- Polimorfismo: São as inúmeras maneiras de se realizar uma mesma ação.

Exemplo: Veículo determina duas ações como acelerar e frear, primeiramente precisamos identificar se estaremos nos referindo a Carro ou Motocicleta para determinar a lógica de aceleração e frenagem dos respectivos veículos.

```java

// HERANÇA: Carro herda as propriedades de Veiculo
public class Carro extends Veiculo {

    public Carro(String placa, String chassi, int anoFabricacao) {
        super(placa, chassi, anoFabricacao); // Repassa os dados para a classe pai
    }

    // POLIMORFISMO: A forma específica do Carro realizar a ação
    @Override
    public void acelerar() {
        System.out.println("CARRO: Acelerando ao pressionar o pedal com o pé direito.");
    }

    // POLIMORFISMO: A forma específica do Carro realizar a ação
    @Override
    public void frear() {
        System.out.println("CARRO: Freando ao acionar o pedal de freio nas 4 rodas.");
    }
}

```

```java


// HERANÇA: Motocicleta herda as propriedades de Veiculo
public class Motocicleta extends Veiculo {

    public Motocicleta(String placa, String chassi, int anoFabricacao) {
        super(placa, chassi, anoFabricacao);
    }

    // POLIMORFISMO: A forma específica da Moto realizar a ação
    @Override
    public void acelerar() {
        System.out.println("MOTOCICLETA: Acelerando ao girar a manopla direita com a mão.");
    }

    // POLIMORFISMO: A forma específica da Moto realizar a ação
    @Override
    public void frear() {
        System.out.println("MOTOCICLETA: Freando ao apertar o manete direito e pisar no pedal.");
    }
}

```

#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |
