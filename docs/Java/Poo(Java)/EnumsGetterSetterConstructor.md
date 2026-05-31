# **Lidando com classes e objetos: Getters, Setters e Construtores em Java**

## **Getters e Setters**

Seguindo a convensão Java Beans

Os métodos "Getters" e "Setters" são utilizados para buscar valores de atributos ou definir novos valores de atributos de instâncias de classes.

- O método Getter retorna o valor do atributo especificado.

- O método Setter define outro novo valor para o atributo especificado.

Vemos o código abaixo da criação de um objeto Aluno com nome e idade:

```java

/arquivo Aluno.java
public class Aluno {
	String nome;
	int idade;
}

//arquivo Escola.java
public class Escola {
	public static void main(String[] args) {
		Aluno felipe = new Aluno();
		felipe.nome="Felipe";
		felipe.idade = 8;
		
		System.out.println("O aluno " + felipe.nome + " tem " + felipe.idade + " anos ");
		//RESULTADO NO CONSOLE
		//O aluno Felipe tem 8 anos 		
	}
}

```

Seguindo a convenção Java Beans, uma classe que contém esta estrutura de estados deverá seguir as regras abaixo:

- Os atributos precisam ter o modificador de acesso ```private```. Ex.: private String nome;

- Como agora os atributos estarão somente a nível de classe, precisaremos dos métodos getX e setX, Ex.: ```getNome()``` e ```setNome(String novoNome)```;

- O método get é responsável por obter o valor atual do atributo, logo ele precisa ser ```public``` retornar um tipo correspondente ao valor, Ex.: ``` public String getNome() {}; ```

- O método set é responsável por definir ou modificador o valor de um atributo em um objeto, logo ele também precisa ser ```public```, receber um parâmetro do mesmo tipo da variável mas não retorna nenhum valor void. Ex.: ```public void setNome(String newNome);```

---

```java


//arquivo Aluno.java
public class Aluno {
	private String nome;
	private int idade;
	
	public String getNome() {
		return nome;
	}
	public void setNome(String newNome) {
		nome = newNome;
	}
	public int getIdade() {
		return idade;
	}
	public void setIdade(int newIdade) {
		this.idade = newIdade;
	}
}
//arquivo Escola.java
public class Escola {
	public static void main(String[] args) {
		Aluno felipe = new Aluno();
		felipe.setNome("Felipe");
		felipe.setIdade(8);
		
		System.out.println("O aluno " + felipe.getNome() + " tem " + felipe.getIdade() + " anos ");	
	}
}

```


---

## **Construtores**

Sabemos que para instanciar um objeto na linguagem Java utilizamos a seguinte estrutura de código:

```java

Classe novoObjeto = new Classe();


```

Desta forma será criado um novo objeto na memória, este recurso também é conhecido como instanciar um novo objeto.

Muitas das vezes já queremos que na criação (instanciação) de um objeto, a linguagem já solicite para quem for criar este novo objeto defina algumas propriedades essenciais. Abaixo iremos ilustrar uma classe Pessoa onde a mesma terá os atributos: Nome, CPF, Endereço



```java

public class Pessoa {
	private String nome;
	private String cpf;
	private String endereco;
	
	public String getNome() {
		return nome;
	}
	public String getCpf() {
		return cpf;
	}
	public String getEndereco() {
		return endereco;
	}
	public void setEndereco(String endereco) {
		this.endereco = endereco;
	}
	//...
	//setters de nome e cpf ?
}

```

Criaremos uma Pessoa mas como não temos o setter para nome e cpf, este objeto não tem como receber estes valores.

```java

public class SistemaCadastro {
	public static void main(String[] args) {
		//criamos uma pessoa no sistema
		Pessoa marcos = new Pessoa();
		
		//definimos o endereço de marcos
		marcos.setEndereco("RUA DAS MARIAS");
		
		//e como definir o nome e cpf do marcos ?
		
		//imprimindo o marcos sem o nome e cpf
		
		System.out.println(marcos.getNome() + "-" + marcos.getCpf());
	}
}


```


Entrando em cena o construtor para criar nossos objetos já com valores requeridos na momento da criação\instanciação (```new```).

```java

public class Pessoa {
	private String nome;
	private String cpf;
	private String endereco;
	
	// método construtor
	// o nome deverá ser igual ao nome da classe
	public Pessoa (String cpf, String nome) {
		this.cpf = cpf;
		this.nome = nome;
	}
	
	//...
	//getters
	//setters
}

```
Alterando o nosso sistema para agora criar o objeto com informações já requeridas conforme definição da ordem dos parâmetros do construtor.

```java

public class SistemaCadastro {
	public static void main(String[] args) {
		//criamos uma pessoa no sistema
		Pessoa marcos = new Pessoa("06724506716","MARCOS SILVA");
		
		//continua ...
		
	}
}

```

Ss contrutores também podem ser usados pra injeção de dependências, ou seja, para criar um objeto já com as dependências necessárias para o seu funcionamento. No spring boot por exemplo, é comum criar um construtor para injetar as dependências necessárias para o funcionamento de um serviço ou controller.

Exemplo:

```java

@Service
public class UserService {
    private final UserRepository userRepository;

    // Construtor para injeção de dependência
    public UserService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }

    // Métodos do serviço...
}

```


#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |
