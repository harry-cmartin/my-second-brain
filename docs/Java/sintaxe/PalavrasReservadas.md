
# **Palavras Reservadas em Java**

Palavras reservadas são identificadores de uma linguagem que já possuem uma finalidade específica, portanto não podem ser utilizados para nomear variáveis, classes, métodos ou atributos.

A linguagem Java possui 52 palavras reservadas. Todas essas palavras são classificadas em grupos e escritas com letra minúscula, sendo identificadas com uma cor especial pela maioria das IDE's. Abaixo temos a lista de palavras agrupadas por sua finalidades.




### **Modificadores de acesso**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>private</code></td>
      <td style="padding: 10px 15px;">Permite o acesso a membros apenas dentro da própria classe onde foram declarados.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>protected</code></td>
      <td style="padding: 10px 15px;">Permite o acesso por classes localizadas no mesmo pacote e por qualquer subclasse (mesmo em pacotes diferentes).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>public</code></td>
      <td style="padding: 10px 15px;">Permite o acesso livre a partir de qualquer outra classe no projeto.</td>
    </tr>
  </tbody>
</table>

### **Modificadores de classes, variáveis ou métodos**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>abstract</code></td>
      <td style="padding: 10px 15px;">Indica uma classe que não pode ser instanciada diretamente ou um método que não possui corpo e precisa ser obrigatoriamente implementado por uma subclasse concreta.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>class</code></td>
      <td style="padding: 10px 15px;">Especifica a declaração e o início de uma classe Java.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>extends</code></td>
      <td style="padding: 10px 15px;">Indica o mecanismo de herança, especificando a superclasse que a subclasse atual está estendendo.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>final</code></td>
      <td style="padding: 10px 15px;">Impede que uma classe seja herdada, que um método seja sobrescrito (overridden) ou torna o valor de uma variável constante (imutável).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>implements</code></td>
      <td style="padding: 10px 15px;">Indica quais contratos de interfaces uma classe irá assinar e implementar.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>interface</code></td>
      <td style="padding: 10px 15px;">Especifica a declaração de uma estrutura de interface, que define um contrato com assinaturas de métodos abstratos.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>native</code></td>
      <td style="padding: 10px 15px;">Sinaliza que a implementação interna do método foi escrita em outra linguagem dependente de plataforma (geralmente C ou C++).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>new</code></td>
      <td style="padding: 10px 15px;">Cria e aloca dinamicamente na memória uma nova instância de um objeto, invocando o seu respectivo construtor.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>static</code></td>
      <td style="padding: 10px 15px;">Associa a variável ou método diretamente ao escopo da classe, e não às suas instâncias individuais.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>strictfp</code></td>
      <td style="padding: 10px 15px;">Garante que os cálculos matemáticos com números de ponto flutuante sejam executados de forma rigorosa e padronizada (IEEE 754) em qualquer plataforma de hardware.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>synchronized</code></td>
      <td style="padding: 10px 15px;">Cria uma trava de concorrência que impede que múltiplas threads acessem um mesmo método ou bloco de código de forma simultânea.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>transient</code></td>
      <td style="padding: 10px 15px;">Informa que um campo de dados específico deve ser ignorado durante o processo de serialização do objeto.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>volatile</code></td>
      <td style="padding: 10px 15px;">Sinaliza ao compilador que a variável pode ter seu valor modificado concorrentemente por múltiplas threads, forçando leituras/escritas direto na memória principal em vez de caches.</td>
    </tr>
  </tbody>
</table>

### **Controle de fluxo dentro de um bloco de código**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>break</code></td>
      <td style="padding: 10px 15px;">Força a saída imediata do bloco de código atual (estruturas de repetição como for/while ou blocos switch).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>case</code></td>
      <td style="padding: 10px 15px;">Define uma das ramificações ou opções de valores a serem avaliadas dentro de uma estrutura switch.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>continue</code></td>
      <td style="padding: 10px 15px;">Interrompe a iteração atual da estrutura de repetição e salta diretamente para a avaliação do próximo passo do loop.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>default</code></td>
      <td style="padding: 10px 15px;">Define o bloco padrão de fallback de um switch caso nenhuma das condições 'case' anteriores seja correspondida.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>do</code></td>
      <td style="padding: 10px 15px;">Garante a execução de um determinado bloco de código pelo menos uma vez antes de avaliar a condição no laço while.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>else</code></td>
      <td style="padding: 10px 15px;">Estrutura um bloco alternativo de código para ser processado caso a expressão de um teste condicional 'if' retorne falsa.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>for</code></td>
      <td style="padding: 10px 15px;">Inicia um loop baseado em controle sequencial de variáveis (inicialização, condição e incremento).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>if</code></td>
      <td style="padding: 10px 15px;">Executa um teste lógico booleano para guiar o fluxo da aplicação caso o resultado seja verdadeiro.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>instanceof</code></td>
      <td style="padding: 10px 15px;">Avalia dinamicamente em tempo de execução se um determinado objeto pertence a uma classe específica, superclasse ou interface.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>return</code></td>
      <td style="padding: 10px 15px;">Encerra a execução do método atual, podendo opcionalmente enviar uma variável ou valor como resposta de volta ao chamador.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>switch</code></td>
      <td style="padding: 10px 15px;">Recebe e avalia o valor de uma variável central a fim de testá-la contra múltiplos cenários 'case'.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>while</code></td>
      <td style="padding: 10px 15px;">Executa continuamente um bloco de instruções de código enquanto sua condição booleana associada permanecer verdadeira.</td>
    </tr>
  </tbody>
</table>

### **Tratamento de erros**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>assert</code></td>
      <td style="padding: 10px 15px;">Avalia uma suposição condicional lógica no código; emite um erro do tipo AssertionError caso o teste resulte em falso (usado para depuração).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>catch</code></td>
      <td style="padding: 10px 15px;">Captura e isola uma exceção disparada dentro do bloco 'try' associado para dar o tratamento correto do erro.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>finally</code></td>
      <td style="padding: 10px 15px;">Garante a execução de um bloco de código finalizador ao término de uma estrutura try-catch, independentemente se houve o disparo de exceções ou não.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>throw</code></td>
      <td style="padding: 10px 15px;">Instancia e lança de maneira explícita uma determinada exceção (erro) no fluxo do programa.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>throws</code></td>
      <td style="padding: 10px 15px;">Anexa à assinatura de um método uma declaração indicando que ele pode propagar certas exceções para quem o invocar.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>try</code></td>
      <td style="padding: 10px 15px;">Delineia o início de um bloco sob monitoramento de segurança que possui risco potencial de disparar erros/exceções.</td>
    </tr>
  </tbody>
</table>

### **Controle de pacotes**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>import</code></td>
      <td style="padding: 10px 15px;">Torna visível e acessível classes de pacotes externos ou internos dentro do arquivo atual.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>package</code></td>
      <td style="padding: 10px 15px;">Declara e define a qual diretório lógico/pacote estrutural pertencem as classes contidas no arquivo.</td>
    </tr>
  </tbody>
</table>

### **Primitivos**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>boolean</code></td>
      <td style="padding: 10px 15px;">Tipo de dado primitivo estruturado para receber apenas as condições lógicas true ou false.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>byte</code></td>
      <td style="padding: 10px 15px;">Tipo de dado inteiro primitivo sinalizado (signed) que reserva o espaço de 8 bits em memória.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>char</code></td>
      <td style="padding: 10px 15px;">Tipo primitivo numérico não sinalizado de 16 bits usado exclusivamente para representar um caractere em padrão Unicode.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>double</code></td>
      <td style="padding: 10px 15px;">Tipo numérico de ponto flutuante de precisão dupla sinalizado, ocupando 64 bits em memória.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>float</code></td>
      <td style="padding: 10px 15px;">Tipo numérico de ponto flutuante de precisão simples sinalizado, ocupando 32 bits em memória.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>int</code></td>
      <td style="padding: 10px 15px;">Tipo de dado inteiro primitivo padrão sinalizado que reserva o tamanho estável de 32 bits.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>long</code></td>
      <td style="padding: 10px 15px;">Tipo de dado inteiro estendido e sinalizado ideal para valores massivos, ocupando 64 bits de espaço.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>short</code></td>
      <td style="padding: 10px 15px;">Tipo numérico de dado inteiro sinalizado reduzido, alocando apenas 16 bits (nota: o texto original continha um pequeno equívoco de digitação ao rotular como 32 bits).</td>
    </tr>
  </tbody>
</table>

### **Variáveis de referência**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>super</code></td>
      <td style="padding: 10px 15px;">Palavra-chave utilizada para fazer referência direta a membros, construtores ou comportamentos da superclasse imediata (pai).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>this</code></td>
      <td style="padding: 10px 15px;">Referência direta auto-apontável para a instância específica e corrente do próprio objeto em execução.</td>
    </tr>
  </tbody>
</table>

### **Retorno de um método**

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 10px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 25%;">Palavra Reservada</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição / Finalidade</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>void</code></td>
      <td style="padding: 10px 15px;">Informa formalmente ao compilador que um método executa suas ações sem retornar nenhum dado ou variável de resposta ao chamador.</td>
    </tr>
  </tbody>
</table>



---

### **Escopo de Uso**

<center>

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 15%;">Uso</th>
      <th style="padding: 12px 15px; width: 45%;">Palavras</th>
      <th style="padding: 12px 15px; width: 40%;">Observação</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;">Arquivo</td>
      <td style="padding: 10px 15px;"><code>package</code>, <code>import</code>, <code>static</code></td>
      <td style="padding: 10px 15px;"></td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;">Classe</td>
      <td style="padding: 10px 15px;"><code>public</code> ou <code>protected</code> ou <code>private</code> + <code>final</code> ou <code>abstract</code> + <code>extends</code> ou <code>implements</code></td>
      <td style="padding: 10px 15px;"><strong>private</strong> (em caso de classe interna), <strong>final</strong> ou <strong>abstract</strong> ?</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;">Método</td>
      <td style="padding: 10px 15px;"><code>public</code> ou <code>protected</code> ou <code>private</code> + <code>static</code> ou <code>final</code> ou <code>abstract</code> + <code>void</code> e <code>return</code></td>
      <td style="padding: 10px 15px;"><strong>void</strong> em caso de não ter retorno ou <strong>return</strong> se houver</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;">Atributo</td>
      <td style="padding: 10px 15px;"><code>public</code> ou <code>protected</code> ou <code>private</code> + <code>static</code> ou <code>final</code> + tipo primitivo</td>
      <td style="padding: 10px 15px;">****</td>
    </tr>
  </tbody>
</table>

</center>

### **Palavras "opostas"**

Assim como nas classificações gramaticais da língua portuguesa, existem algumas palavras que são completamente opostas (antônimas) na linguagem Java conforme tabela abaixo:

<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left; margin-top: 15px; margin-bottom: 30px;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 15%;">Palavra</th>
      <th style="padding: 12px 15px; width: 15%;">Palavra</th>
      <th style="padding: 12px 15px; width: 70%;">Explicação</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>package</code></td>
      <td style="padding: 10px 15px;"><code>import</code></td>
      <td style="padding: 10px 15px;">Enquanto <strong>package</strong> determina o diretório real da classe, o <strong>import</strong> informe de onde será importada a classe. Isso porque podemos ter classes de mesmo nome.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>extends</code></td>
      <td style="padding: 10px 15px;"><code>implements</code></td>
      <td style="padding: 10px 15px;">enquanto <strong>extends</strong> determinas que uma classe estende outra classe, <strong>implements</strong> determina que uma classe implementa uma interface, porém nunca o contrário</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px;"><code>final</code></td>
      <td style="padding: 10px 15px;"><code>abstract</code></td>
      <td style="padding: 10px 15px;">enquanto <strong>final</strong> determina fim de alteração de valor ou lógica comportamental, <strong>abstract</strong> em métodos exige que sub-classes precisarão definir comportamento é um método abstrato. NOTA: Se uma classe contém um único método abstrato, toda classe precisa ser.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px;"><code>throws</code></td>
      <td style="padding: 10px 15px;"><code>throw</code></td>
      <td style="padding: 10px 15px;">Esta é uma das situações mais complicadas de compreensão destas duas palavras. Enquanto a <strong>throws</strong> determina que um método pode lançar uma exceção, <strong>throw</strong> é a implementação que dispara a exceção**. Vamos conhecer mais sobre este conceito no assunto Exceções.**</td>
    </tr>
  </tbody>
</table>

</center>




#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |