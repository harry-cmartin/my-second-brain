

# **Tipos e Variáveis**

## **Tipos de dados**


No Java, existem algumas palavras reservadas para a representação dos tipos de dados básicos que precisam ser manipulados para a construção de programas. Estes tipos de dados são conhecidos como tipos primitivos (Primitive Types).

!!!Atenção
    Os oito tipos primitivos em Java são: **int**, **byte**, **short**, **long**, **float**, **double**, **boolean** e **char**. Esses tipos não são considerados objetos e representam valores brutos. Em geral, variáveis locais de tipos primitivos possuem seus valores armazenados diretamente na memória associada à execução do método (stack frame).

    Tabela de Tipos Primitivos e seus valores:

<center>

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 15px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 15%;">Tipo</th>
      <th style="padding: 12px 15px; width: 15%;">Memória</th>
      <th style="padding: 12px 15px; width: 35%;">Valor Mínimo</th>
      <th style="padding: 12px 15px; width: 35%;">Valor Máximo</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>byte</code></td>
      <td style="padding: 10px 15px;">1 byte</td>
      <td style="padding: 10px 15px;">-128</td>
      <td style="padding: 10px 15px;">127</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>short</code></td>
      <td style="padding: 10px 15px;">2 byte</td>
      <td style="padding: 10px 15px;">-32.768</td>
      <td style="padding: 10px 15px;">32.767</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>int</code></td>
      <td style="padding: 10px 15px;">4 bytes</td>
      <td style="padding: 10px 15px;">-2.147.483.648</td>
      <td style="padding: 10px 15px;">2.147.483.647</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>long</code></td>
      <td style="padding: 10px 15px;">8 bytes</td>
      <td style="padding: 10px 15px;">-9.223.372.036.854.775.808</td>
      <td style="padding: 10px 15px;">9.223.372.036.854.775.807</td>
    </tr>
  </tbody>
</table>
</center>

Os tipos primitivos que podem conter partes fracionárias podem ser representados por dois tipos:

<center>
<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 15px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 15%;">Tipo</th>
      <th style="padding: 12px 15px; width: 15%;">Memória</th>
      <th style="padding: 12px 15px; width: 25%;">Mínimo</th>
      <th style="padding: 12px 15px; width: 25%;">Máximo</th>
      <th style="padding: 12px 15px; width: 20%;">Precisão</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>float</code></td>
      <td style="padding: 10px 15px;">4 bytes</td>
      <td style="padding: 10px 15px;">-3,4028E + 38</td>
      <td style="padding: 10px 15px;">3,4028E + 38</td>
      <td style="padding: 10px 15px;">6 - 7 dígitos</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>double</code></td>
      <td style="padding: 10px 15px;">8 bytes</td>
      <td style="padding: 10px 15px;">-1,7976E + 308</td>
      <td style="padding: 10px 15px;">1,7976E + 308</td>
      <td style="padding: 10px 15px;">15 dígitos</td>
    </tr>
  </tbody>
</table>


</center>

!!!Dica
    O tipo primitivo <code>var</code> é uma adição mais recente ao Java, introduzida no Java 10. Ele permite a inferência de tipo para variáveis locais, ou seja, o compilador deduz o tipo da variável com base no valor atribuído a ela. Isso torna o código mais conciso e legível, sem perder a segurança de tipos estáticos do Java.

<center>

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 15px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 20%;">Família</th>
      <th style="padding: 12px 15px; width: 25%;">Tipo Primitivo</th>
      <th style="padding: 12px 15px; width: 30%;">Wrapper Class</th>
      <th style="padding: 12px 15px; width: 25%;">Tamanho</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;">LÓGICO</td>
      <td style="padding: 10px 15px;"><code>boolean</code></td>
      <td style="padding: 10px 15px;"><code>Boolean</code></td>
      <td style="padding: 10px 15px;">1 bit</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;">LITERAIS</td>
      <td style="padding: 10px 15px;"><code>char</code></td>
      <td style="padding: 10px 15px;"><code>Character</code></td>
      <td style="padding: 10px 15px;">1 byte</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"></td>
      <td style="padding: 10px 15px;">-</td>
      <td style="padding: 10px 15px;"><code>String</code></td>
      <td style="padding: 10px 15px;">1 byte/cada</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;">INTEIROS</td>
      <td style="padding: 10px 15px;"><code>byte</code></td>
      <td style="padding: 10px 15px;"><code>Byte</code></td>
      <td style="padding: 10px 15px;">1 byte</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"></td>
      <td style="padding: 10px 15px;"><code>short</code></td>
      <td style="padding: 10px 15px;"><code>Short</code></td>
      <td style="padding: 10px 15px;">2 bytes</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"></td>
      <td style="padding: 10px 15px;"><code>int</code></td>
      <td style="padding: 10px 15px;"><code>Integer</code></td>
      <td style="padding: 10px 15px;">4 bytes</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"></td>
      <td style="padding: 10px 15px;"><code>long</code></td>
      <td style="padding: 10px 15px;"><code>Long</code></td>
      <td style="padding: 10px 15px;">8 bytes</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;">REAIS</td>
      <td style="padding: 10px 15px;"><code>float</code></td>
      <td style="padding: 10px 15px;"><code>Float</code></td>
      <td style="padding: 10px 15px;">4 bytes</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"></td>
      <td style="padding: 10px 15px;"><code>double</code></td>
      <td style="padding: 10px 15px;"><code>Double</code></td>
      <td style="padding: 10px 15px;">8 bytes</td>
    </tr>
  </tbody>
</table>
</center>

Em Java, uma wrapper class (classe empacotadora) é uma classe especial que "embrulha" um tipo de dado primitivo (como int, double, boolean) e o transforma em um objeto. Isso é essencial pois a Orientação a Objetos exige o uso de objetos em muitos cenários.
O Java facilita a sua vida convertendo automaticamente um tipo primitivo para o seu objeto wrapper (e vice-versa) através de dois processos chamados autoboxing e unboxing.

- Por que precisamos delas?Coleções (Collections): Estruturas de dados como ArrayList ou HashMap só trabalham com objetos, e não com dados primitivos. Para guardar números em uma lista, você precisa da versão Wrapper.

- Métodos utilitários: Elas oferecem métodos muito úteis para conversão de dados. Por exemplo, para transformar um texto (String) em um número inteiro (int), você usa o método da classe Wrapper:int idade = Integer.parseInt("25");

### **Declarando Variáveis**

```java

    int[] idade = new int[4]; // Declaração de um array de inteiros
    char[] letras = new char[5]; // Declaração de um array de caracteres
    
    double salario = 5000.50; // Declaração de um número decimal
    boolean isAtivo = true; // Declaração de um valor booleano
    char letra = 'A'; // Declaração de um caractere
    String nome = "João"; // Declaração de uma string
    var numero = 42; // Declaração usando inferência de tipo (Java 10+)
    short pequenoNumero = 100; // Declaração de um número curto
    long grandeNumero = 123456789L; // Declaração de um número longo
    byte byteValor = 127; // Declaração de um número byte
    float valorFloat = 3.14f; // Declaração de um número float


```

#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |