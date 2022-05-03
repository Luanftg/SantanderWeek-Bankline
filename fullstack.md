# Aula 02 - Preparando o Ambiente de Desenvolvimento - 03/05/2022

## Histórico da Linguagem Java

![James Goslin](https://static.javatpoint.com/images/j1.jpg)
- 1991: Sun Microsystem = Pesquisa "Green" resulta no desenvolvimento da linguagem C e C++ (James Gosling a batizou de Oak-carvalho)

## Orientação a Obejtos

<b>Um objeto é uma abstração do mundo real composto por:</b>

- Identificador (nome)
- Atributos (propriedades)
- Métodos (comportamentos)

<b>Uma classe é descrita em um arquivo de extensão: `.java`.</b>

- Instanciar (`new`) = cria um objeto a partir da estrutura definida em uma classe
- Comportamntosa (behavior) = A parte comportamental que define as ações ou métodos que um objeto dispõe
- Caracterpisticas (states) = Atributos ou propiedades representam o estado do objeto
- Identificador (identity) = Proposito existencial aos objetos que serão criados.

![Representação de diagrama de Classse e Objeto](http://theclub.com.br/Restrito/Revistas/201208/ling01.jpg)
[Image 1 - TheClub](http://theclub.com.br/Restrito/Revistas/201208/ling1208.aspx)

## Tecnologias associadas a Java

- Java JDK
- IDE
- [Hibernate](https://hibernate.org/) - Framework baseado no conceito de [ORM](https://hibernate.org/orm/) para a persistência de banco de dados relacional
- [Spring Framework](https://spring.io/) - Plataforma de aplicações baseado nos padrões de projeto de [INVERSÃO DE CONTROLE e INJEÇÃO DE DEPENDÊNCIAS](https://www.baeldung.com/inversion-control-and-dependency-injection-in-spring)
- Postgres - Banco de Dados relacional para projetos de grande porte
- Swagger - Ferramenta de documentação de API
- GitHub - repositório e gestor de versionamento de código
- Maven - Sistema para gestão de dependências e distribuição de aplicações
- REST- Arquitetura REST para transferência de dados representativos como JSON
- HEROKU - Plataforma de hospedagem de applicações

## Arquitetura

O Projeto <b>BANKLINE</b> será desenvolvido na arquitetura Spring Framework + Springboot estruturado no padrão [MVC (Model View Controller)](https://www.lewagon.com/pt-BR/blog/o-que-e-padrao-mvc) para promover uma API REST para movimentações financeiras simples

### Spring FrameWork

- Inversion of Control = redireciona o fluxo de execução de um código retirando parcialmente o controle sobre ele e delegando-o para um container. PRetende minimizar o acoplamento do código
- Dependency injection = É um padrão de desenvolvimento com a finalidade de manter baixo o nível de acoplamento entre módulos de um sistema
  - [BEANS](https://www.devmedia.com.br/introducao-aos-javabeans/8621) = objeto que é instanciado, montado e gerenciado por um container através do principio da inversão de controle
  - [SCOPES](https://www.w3schools.com/java/java_scope.asp) = vai cuidar da abrangência na qual o ecurso está disponível.
  - [AUTOWIRED](https://medium.com/@leonardogiuliani/autowired-e-a-inje%C3%A7%C3%A3o-de-depend%C3%AAncia-do-spring-d8864cc9af50) = Capacidade de obter recurso disponível pelo container

![Spring Framework Runtime](https://miro.medium.com/max/1284/1*7hCFiOlF9bOIv-MlBpFgeA.gif)
[Image2 - Spring Framework](https://medium.com/@michellibrito/spring-framework-e9e907582c7)

### Springboot

Leque de componentes e funcionalidades em cima do Spring Framework. Configura automaticamente as dependências.

- Starters =  são dependências que agrupam outras dependências com um propósito comum.
  - `data-jpa` = Integração ao banco de dados via JPA - Hibernate
  - `data-mongodb` = Mongo DB
  - `web` = Inclusão do container Tomcat para aplicações REST
  - `web-services` = Web Services baseado na arquitetura SOAP 
  - `batch` = Implementações de JOBs de processos
  - `test` = Disponibilização de recursos para testes unitários como JUnit
  - `openfeign` = Client HTTP baseado em interfaces
  - `actuator` = Gerenciamento de monitoramento de aplicações

#### REFERÊNCIAS

[History of Java](https://www.javatpoint.com/history-of-java)
[SPRING VS JAVA EE](https://www.alura.com.br/artigos/java-ee-versus-spring-retomando-a-discussao)