# O que é uma API (Interface de Programação de Aplicativos)?

Uma API, ou interface de programação de aplicativos, é um conjunto de regras ou protocolos que permitem que aplicativos de software se comuniquem entre si para trocar dados, recursos e funcionalidades.

As APIs simplificam e aceleram o desenvolvimento de software e aplicações, permitindo que os desenvolvedores integrem dados, serviços e recursos de outras aplicações, em vez de desenvolvê-los do zero. As APIs também oferecem aos proprietários de aplicativos uma maneira simples e segura de disponibilizar os dados e as funções dos aplicativos para os departamentos da organização. Os proprietários de aplicações também podem compartilhar ou comercializar dados e funções com parceiros de negócios ou terceiros.

As APIs permitem o compartilhamento apenas das informações necessárias, mantendo ocultos outros detalhes internos do sistema, o que auxilia na segurança do sistema. Os servidores ou dispositivos não precisam expor totalmente os dados: as APIs permitem o compartilhamento de pequenos pacotes de dados, relevantes para a solicitação específica.

A documentação de API funciona como um manual técnico que fornece detalhes sobre uma API e informações para os desenvolvedores sobre como trabalhar com essa API e seus serviços. Uma documentação bem elaborada promove uma experiência melhor com a API e, em geral, contribui para o sucesso da API.

## Como funcionam as APIs?

É útil pensar na comunicação da API em termos de solicitação e resposta entre um cliente e um servidor. O aplicativo que envia a solicitação é o cliente e o servidor fornece a resposta. A API é a ponte que estabelece a conexão entre eles.

Uma maneira simples de entender como as APIs funcionam é analisar um exemplo comum: o processamento de pagamentos de terceiros. Quando um usuário compra um produto em um site de comércio eletrônico, o site pode pedir ao usuário para "Pagar com PayPal" ou outro tipo de sistema de terceiros. Essa função depende de APIs para fazer a conexão.

Quando o comprador clica no botão de pagamento, uma chamada de API é enviada para recuperar informações. Esta é a solicitação. Essa solicitação é processada de um aplicativo para o servidor web por meio do Uniform Resource Identifier (URI) da API e inclui um verbo de solicitação, cabeçalhos e, às vezes, um corpo de solicitação.

Depois de receber uma solicitação válida da página do produto, a API liga para o programa externo ou servidor web, neste caso, o sistema de pagamento de terceiros. O servidor envia uma resposta à API com as informações solicitadas. A API transfere os dados para o aplicativo que fez a solicitação inicial, neste caso, o site do produto.

Embora a transferência de dados possa variar dependendo do serviço da web usado, todas as solicitações e respostas ocorrem por meio de uma API. Não há visibilidade na interface do usuário, o que significa que as APIs trocam dados dentro do computador ou do aplicativo e aparecem para o usuário como uma conexão contínua.

## Tipos de APIs

As APIs podem ser categorizadas por caso de uso, incluindo APIs de dados, APIs de sistema operacional, APIs remotas e APIs da web.

### APIs da Web

As APIs da web permitem a transferência de dados e funcionalidades pela internet usando o protocolo HTTP. Hoje, a maioria das APIs são APIs da web. APIs da web são um tipo de API remota (o que significa que a API usa protocolos para manipular recursos externos) que expõem os dados e funcionalidades de uma aplicação pela internet.

Os quatro principais tipos de APIs da web são:

- **APIs abertas**: APIs abertas são interfaces de programação de aplicativos de código aberto que você pode acessar com o protocolo HTTP. Também conhecidas como APIs públicas, elas definiram endpoints de API e formatos de solicitação e resposta.
- **APIs de parceiros**: As APIs de parceiros conectam parceiros comerciais estratégicos. Normalmente, os desenvolvedores acessam essas APIs no modo de autoatendimento por meio de um portal público de desenvolvedores de APIs. Ainda assim, eles precisam concluir um processo de integração e obter credenciais de login para acessar APIs de parceiros.
- **APIs internas**: As APIs internas ou privadas permanecem ocultas dos usuários externos. Essas APIs privadas não estão disponíveis para usuários fora da empresa. Em vez disso, as organizações os usam para melhorar a produtividade e a comunicação entre diferentes equipes internas de desenvolvimento.
- **APIs compostas**: APIs compostas combinam vários dados ou APIs de serviço. Eles permitem que os programadores acessem vários endpoints em uma única chamada. APIs compostas são úteis na arquitetura de microsserviços, onde executar uma única tarefa pode exigir informações de várias fontes.

### Outros tipos de APIs

Tipos menos comuns de APIs incluem:

- **APIs de dados (ou de banco de dados)**, usadas para conectar aplicações a sistemas de gerenciamento de banco de dados.
- **APIs do sistema operacional (ou locais)**, usadas para definir como as aplicações utilizam serviços e recursos do sistema operacional.
- **APIs remotas**, usadas para definir como aplicações em dispositivos diferentes interagem.

## Exemplos de API

Como as APIs permitem que as organizações abram o acesso a seus recursos e, ao mesmo tempo, mantenham a segurança e o controle, elas se tornaram um aspecto valioso dos aplicativos comerciais e pessoais modernos. Aqui estão alguns exemplos de API que os usuários frequentemente encontram:

- **Logins universais**: Um exemplo popular de API é a função que permite que as pessoas façam login em sites usando seus detalhes de login do perfil do Facebook, X ou Google. Esse recurso conveniente permite que qualquer site use uma API de um dos serviços mais populares para autenticação rápida. Esse recurso ajuda a economizar o tempo e o incômodo dos usuários de configurar um novo perfil para cada aplicativo Web ou nova associação.
- **Internet das coisas (IoT)**: Esses “dispositivos inteligentes” oferecem funcionalidade adicional, como telas sensíveis ao toque habilitadas para internet e coleta de dados, por meio de APIs. Por exemplo, uma geladeira inteligente pode se conectar a aplicativos de receita ou fazer e enviar anotações para celulares por mensagem de texto. As câmeras internas se conectam a vários aplicativos para que os usuários possam ver o conteúdo da geladeira de qualquer lugar.
- **Comparações de reservas de viagens**: Os sites de reserva de viagens agregam milhares de voos, apresentando as opções mais baratas para cada data e destino. As APIs permitem esse serviço, fornecendo aos usuários do aplicativo acesso às informações mais recentes sobre disponibilidade de hotéis e companhias aéreas. Este acesso está disponível através de um navegador web ou da própria aplicação da empresa de reservas de viagens. Com uma troca autônoma de dados e solicitações, as APIs reduzem drasticamente o tempo e o esforço envolvidos na verificação de voos ou acomodações disponíveis.
- **Aplicativos de navegação**: Os aplicativos de navegação usam APIs principais que exibem mapas estáticos ou interativos. Esses aplicativos também usam outras APIs e recursos para fornecer aos usuários direções, limites de velocidade, pontos de interesse, avisos de trânsito e muito mais. Os usuários se comunicam com uma API ao traçar rotas de viagem ou rastrear itens em movimento, como um veículo de entrega.
- **Redes sociais**: As empresas de mídia social usam APIs para permitir que outras entidades compartilhem e incorporem conteúdo apresentado em aplicativos de mídia social em seus próprios sites. Por exemplo, a API do Instagram permite que as empresas incorporem sua grade do Instagram em seu site e que a grade seja atualizada automaticamente à medida que os usuários adicionam novas publicações.
- **Aplicações SaaS**: As APIs são parte integrante do crescimento dos produtos de software como serviço (SaaS). Plataformas como CRMs (ferramentas de gerenciamento de relacionamento com o cliente) geralmente incluem várias APIs integradas, que permitem que as empresas se integrem a aplicações que elas já usam, como mensagens, redes sociais e aplicativos de e-mail. Essa integração reduz drasticamente o tempo gasto alternando entre aplicativos para tarefas de vendas e marketing. Ele também ajuda a reduzir ou evitar silos de dados que possam existir entre departamentos que usam aplicativos diferentes.

## Protocolos API, estilos arquitetônicos e linguagens

Tradicionalmente, API se referia a uma interface conectada a uma aplicação criada com qualquer linguagem de programação de baixo nível, como JavaScript. No entanto, as APIs modernas variam em suas arquiteturas e uso de formatos de dados. Elas geralmente são construídas para HTTP, resultando em interfaces amigáveis para os desenvolvedores que são facilmente acessíveis e amplamente compreendidas por aplicações escritas em Java, Ruby, Python e muitas outras linguagens.

À medida que o uso de APIs da web aumentou, isso levou ao desenvolvimento e uso de determinados protocolos, estilos, padrões e linguagens. Essas estruturas fornecem aos usuários um conjunto de regras definidas, ou especificações de API, que criam tipos de dados, comandos e sintaxe aceitos. Em vigor, esses protocolos de API facilitam a troca de informações padronizada.

- **SOAP (simple object access protocol)**: SOAP é uma especificação leve de protocolo de mensagens baseada em XML que permite que endpoints enviem e recebam dados por meio de diversos protocolos de comunicação, incluindo SMTP (protocolo de transferência de correio simples) e HTTP (protocolo de transferência de hipertexto). SOAP é independente, o que permite que APIs SOAP compartilhem informações entre aplicações ou componentes de software que rodam em ambientes diferentes ou que foram escritos em linguagens diferentes.
- **Chamada de procedimento remoto (RPC)**: A chamada de procedimento remoto (RPC) é um protocolo que fornece o paradigma de comunicação de alto nível usado no sistema operacional. O RPC pressupõe a existência de um protocolo de transporte de baixo nível, como o protocolo de controle de transmissão/Internet Protocol (TCP/IP) ou o protocolo de datagrama de usuário (UDP), para transportar os dados da mensagem entre programas de comunicação. O RPC implementa um sistema lógico de comunicação cliente-servidor projetado especificamente para dar suporte a aplicativos de rede. O protocolo RPC permite que os usuários trabalhem com procedimentos remotos como se fossem locais.
- **XML-RPC (XML- chamada de procedimento remoto)**: O protocolo XML-RPC depende de um formato XML específico para transferir dados. O XML-RPC é mais antigo que o SOAP, porém mais simples e relativamente leve, pois usa largura de banda mínima.
- **JSON-RPC**: Assim como o XML-RPC, o JSON-RPC é uma chamada de procedimento remoto, que usa JSON (JavaScript Object Notation) em vez de XML. JSON é um formato leve para troca de dados que é simples de analisar e usa pares nome/valor e listas ordenadas de valores. Como o JSON usa estruturas de dados universais, ele pode ser usado com qualquer linguagem de programação.
- **gRPC**: O gRPC é uma framework RPC de alto desempenho e de código aberto desenvolvida inicialmente pelo Google. O gRPC usa o protocolo de rede HTTP/2 e o formato de dados Protocol Buffers e é comumente usado para conectar serviços em uma arquitetura de microsserviços.
- **WebSocket**: As APIs do WebSocket permitem a comunicação bidirecional entre o cliente e o servidor. Esse tipo de API não exige o estabelecimento de uma nova conexão para cada comunicação - uma vez estabelecida a conexão, ela permite a troca contínua. Isso torna as APIs Web Socket ideais para comunicação em tempo real.
- **REST (transferência de estado representacional)**: REST é um conjunto de princípios de arquitetura de API da web. As APIs REST — também conhecidas como APIs RESTful — são APIs que aderem a certas restrições arquitetônicas REST. As APIs REST usam solicitações HTTP como GET, PUT, HEAD e DELETE para interagir com recursos. O REST disponibiliza dados como recursos, com cada recurso representado por um URI exclusivo. Os clientes solicitam um recurso fornecendo seu URI. APIs REST são sem estado, elas não salvam dados do cliente entre solicitações. É possível construir APIs RESTful com protocolos SOAP, mas os profissionais geralmente veem os dois padrões como especificações concorrentes.
- **GraphQL**: GraphQL é uma linguagem de consulta de código aberto e uma infraestrutura de tempo de execução no servidor que especifica como os clientes devem interagir com as APIs. O GraphQL permite que os usuários façam requisições à API com apenas algumas linhas, em vez de acessar endpoints complexos com muitos parâmetros. Esse recurso pode tornar mais fácil gerar e responder a consultas de API, especialmente as mais complexas ou específicas que direcionam múltiplos recursos.

### REST x SOAP

SOAP e REST representam abordagens diferentes para o design da API, descrevendo regras e padrões de como uma API deve interagir com outros aplicativos. SOAP é um protocolo, enquanto REST é um conjunto de restrições que constituem um estilo arquitetônico. Ambos usam HTTP para trocar informações.

REST é frequentemente considerado uma alternativa mais simples ao SOAP, pois é leve, flexível, transparente e relativamente fácil de usar; o SOAP exige que os usuários escrevam mais código para concluir cada tarefa do que o REST exige.

SOAP é mais determinístico e robusto (devido à verificação de tipo), e seus defensores argumentam que ele é mais fácil de usar por causa do suporte embutido em muitas ferramentas de desenvolvimento. SOAP oferece conformidade embutida, e os desenvolvedores frequentemente o consideram um protocolo mais seguro, mais adequado para situações que exigem rigor na integridade dos dados.

Os sistemas RESTful suportam mensagens em diferentes formatos, como texto simples, HTML, YAML, XML e JSON, enquanto o SOAP permite apenas XML. Cada um tem seus pontos fortes, e a "escolha certa" pode depender do caso de uso. No entanto, a capacidade de oferecer suporte a vários formatos para armazenamento e troca de dados é uma das razões pelas quais o REST é uma escolha predominante para a criação de APIs públicas.

### REST vs. GraphQL

O GraphQL é uma linguagem de consulta e tempo de execução de API que o Facebook desenvolveu internamente em 2012 antes de se tornar de código aberto em 2015. O GraphQL e REST são ambos stateless, usam o modelo cliente/servidor e utilizam HTTP. O GraphQL resolve algumas limitações do REST, como oferecer a capacidade de direcionar recursos específicos com uma única requisição.

As APIs REST seguem uma estrutura fixa e sempre retornam um conjunto de dados completo para um objeto especificado. Se a solicitação for mais complexa, abrangendo vários recursos, por exemplo, o cliente deverá enviar solicitações separadas para cada recurso. Essas limitações podem levar a problemas de busca insuficiente ou excessiva.

Nenhuma das APIs REST ou GraphQL é inerentemente superior. São ferramentas diferentes adequadas para tarefas diferentes. O REST geralmente é mais fácil de implementar e pode ser uma boa opção quando se prefere um protocolo de comunicação simples e armazenável em cache com controles de acesso rigorosos (para sites de comércio eletrônico voltados para o público, como Shopify e GitHub, por exemplo).

As APIs GraphQL permitem a busca de dados mais flexível e eficiente, o que pode melhorar o desempenho do sistema e a facilidade de uso para os desenvolvedores. Esses recursos tornam o GraphQL especialmente útil para criar APIs em ambientes complexos com requisitos de front-end em rápida mudança.

## APIs, serviços da web e microsserviços

### APIs vs. serviços da Web

Um serviço web é um componente de software de internet que facilita transferências de dados em uma rede. Uma vez que um serviço web torna os dados e funcionalidades de uma aplicação acessíveis para outras aplicações, podemos dizer que, essencialmente, todo serviço web é uma API. No entanto, nem toda API é um serviço web.

APIs são qualquer componente de software que serve como intermediário entre dois aplicativos desconectados. Enquanto os serviços da web também conectam aplicativos, eles exigem uma rede para fazer isso. Os serviços da Web geralmente são privados e somente usuários aprovados podem acessá-los.

### APIs, microsserviços e desenvolvimento nativo da nuvem

Microsserviços são um estilo arquitetônico que divide uma aplicação em componentes menores e independentes, frequentemente conectados por APIs REST. Criar uma aplicação como uma coleção de serviços separados permite que os desenvolvedores trabalhem em um componente da aplicação independentemente dos outros, e torna as aplicações mais fáceis de testar, manter e escalar.

A arquitetura de microsserviços se tornou mais comum com o avanço da computação em nuvem e, juntamente com contêineres e Kubernetes, é fundamental para o desenvolvimento de aplicações nativas da nuvem.

## Benefícios da API

As APIs simplificam o design e desenvolvimento de novas aplicações e serviços, bem como a integração e gerenciamento dos já existentes. Elas também oferecem benefícios significativos para desenvolvedores e organizações em geral.

- **Colaboração aprimorada**: A empresa média usa quase 1.200 aplicações em nuvem, muitas das quais estão desconectadas. As APIs permitem integração para que essas plataformas e aplicações possam se comunicar entre si sem dificuldades. Por meio dessa integração, as empresas podem automatizar fluxos de trabalho e melhorar a colaboração no local de trabalho. Sem APIs, muitas empresas não teriam conectividade, criando silos de informação que comprometem a produtividade e o desempenho.
- **Inovação acelerada**: As APIs oferecem flexibilidade, permitindo que as empresas façam conexões com novos parceiros de negócios e ofereçam novos serviços ao seu mercado atual. Essa flexibilidade também permite que as empresas acessem novos mercados, o que pode aumentar os retornos e impulsionar a transformação digital. Por exemplo, a empresa Stripe começou como uma API com apenas sete linhas de código. Desde então, a empresa trabalhou com muitas das maiores corporações do mundo. A Stripe diversificou para oferecer empréstimos e cartões corporativos, e recebeu uma avaliação recente de USD 65 bilhões.
- **Monetização dos dados**: Muitas empresas optam por oferecer APIs sem custo, pelo menos inicialmente, para construir uma audiência de desenvolvedores em torno de sua marca e estabelecer relacionamentos com parceiros em potencial. Se a API concede acesso a ativos digitais valiosos, a empresa a monetiza vendendo o acesso. Essa prática é chamada de economia de APIs. Quando a AccuWeather lançou seu portal de desenvolvedor com autoatendimento para vender uma ampla gama de pacotes de APIs, levou apenas 10 meses para atrair 24.000 desenvolvedores, vendendo 11.000 chaves de API. Essa iniciativa ajudou a construir uma comunidade próspera no processo.
- **Segurança do sistema**: As APIs separam a aplicação solicitante da infraestrutura do serviço que responde e oferecem camadas de segurança entre os dois durante a comunicação. Por exemplo, chamadas de API normalmente exigem credenciais de autenticação. Cabeçalhos HTTP, cookies ou strings de consulta podem fornecer segurança adicional durante a troca de dados. Um API gateway pode controlar o acesso para minimizar ainda mais as ameaças à segurança.
- **Segurança e privacidade do usuário**: As APIs fornecem proteção adicional dentro de uma rede. Eles também podem fornecer outra camada de proteção para usuários pessoais. Quando um site solicita a localização de um usuário (uma API de localização fornece essas informações), o usuário pode decidir se deseja permitir ou negar essa solicitação. Muitos navegadores da web e sistemas operacionais de desktop e móveis têm estruturas de permissão integradas. Quando um aplicativo precisa acessar arquivos por meio de uma API, sistemas operacionais como iOS, macOS, Windows e Linux usam permissões para esse acesso.



## Bibliografia 

>  

## Histórico de Versões

| Versão |    Data    | Descrição            | Autor(es)                                    | Revisor(es) |
| ------ | :--------: | -------------------- | -------------------------------------------- | ----------- |
| 1.0    | 18/06/2026 | Criação do documento | [Harryson](https://github.com/harry-cmartin) |             |
