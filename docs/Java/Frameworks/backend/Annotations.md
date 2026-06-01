
## **Anotações: Spring Boot vs Quarkus**


Essa transição do Spring para o Quarkus é um momento de muito aprendizado. A principal diferença conceitual aqui é que o Spring criou o seu próprio ecossistema de anotações, enquanto o **Quarkus utiliza os padrões oficiais do Java/Jakarta EE** (como o JAX-RS para web e o CDI para injeção de dependências).

Isso significa que o que você vai aprender no Quarkus serve para qualquer outro framework que siga o padrão do mercado.

Aqui está a tabela de equivalência baseada nas categorias que você trouxe:

| **Spring Boot**                                 | **Quarkus (Jakarta EE / MicroProfile)**  | **O que faz na prática**                                                                                     |
| ----------------------------------------------- | ---------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **@SpringBootApplication**                      | _(Não é necessário)_                     | Inicializa a aplicação. O Quarkus faz o escaneamento e a montagem das rotas automaticamente durante o build. |
| **@Configuration**                              | **@Dependent** ou **@ApplicationScoped** | Define uma classe que cria e fornece objetos gerenciados para a aplicação.                                   |
| **@Component** / **@Service** / **@Repository** | **@ApplicationScoped** ou **@Singleton** | Registra a classe no container (CDI) para que ela possa ser injetada em outros lugares.                      |
| **@RestController**                             | **@Path**                                | Indica que a classe é um controlador que vai expor endpoints na web.                                         |
| **@RequestMapping**                             | **@Path**                                | Define a rota principal (URL) daquela classe ou método.                                                      |
| **@GetMapping**                                 | **@GET**                                 | Mapeia uma requisição de leitura HTTP GET.                                                                   |
| **@PostMapping**                                | **@POST**                                | Mapeia uma requisição de criação HTTP POST.                                                                  |
| **@PutMapping**                                 | **@PUT**                                 | Mapeia uma requisição de atualização HTTP PUT.                                                               |
| **@DeleteMapping**                              | **@DELETE**                              | Mapeia uma requisição de exclusão HTTP DELETE.                                                               |
| **@PathVariable**                               | **@PathParam**                           | Captura valores que vêm embutidos na URL (ex: /usuarios/1).                                                  |
| **@RequestParam**                               | **@QueryParam**                          | Captura valores passados após o ponto de interrogação na URL (ex: ?nome=joao).                               |
| **@RequestBody**                                | _(Não é necessário)_ ou **@RestBody**    | Converte o JSON em objeto. No Quarkus, basta declarar o objeto como parâmetro do método.                     |
| **@Autowired**                                  | **@Inject**                              | Pede ao framework para instanciar e injetar a classe automaticamente (Injeção de Dependência).               |
| **@Qualifier**                                  | **@Named** ou **@Identifier**            | Informa exatamente qual implementação usar quando você tem duas classes implementando a mesma interface.     |
| **@Value**                                      | **@ConfigProperty**                      | Puxa um valor do seu application.yml e joga dentro da variável.                                              |
| **@Valid**                                      | **@Valid**                               | Aplica validações estruturais (ex: @NotNull, @Size) antes de aceitar a requisição.                           |
| **@ControllerAdvice**                           |         **@Provider**                               | Registra a classe como um provedor global (ex: para capturar exceções em toda a aplicação).                                              |
| **@ExceptionHandler**                           |          **@ServerExceptionMapper**                                | Mapeia um método para tratar um tipo específico de exceção e retornar a resposta formatada.                                                       |

**Dica de ouro sobre Injeção de Dependência :**

Assim como no Spring moderno, no Quarkus a melhor prática também é não usar o @Inject direto na variável. O ideal é usar a injeção via construtor (se a classe tiver apenas um construtor, o Quarkus injeta tudo automaticamente, sem você precisar digitar o @Inject).


#### Bibliografia 

>  


#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |