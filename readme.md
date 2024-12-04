# Sistema de Controle de Ponto e Acesso 

## Descrição do Projeto
API Rest para controle de ponto e acesso de funcionários, desenvolvida com Spring Boot.

## Estrutura do Projeto: 


  <details align="left">
  <summary></summary> 
    
```	
ControleDeAcesso/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── empresa/
│   │   │           └── controleponto/
│   │   │               ├── ControlePontoAcessoApplication.java
│   │   │               ├── config/
│   │   │               │   ├── SwaggerConfig.java
│   │   │               │   └── SecurityConfig.java
│   │   │               ├── controller/
│   │   │               │   ├── UsuarioController.java
│   │   │               │   └── RegistroPontoController.java
│   │   │               ├── model/
│   │   │               │   ├── Usuario.java
│   │   │               │   ├── RegistroPonto.java
│   │   │               │   ├── TipoUsuario.java
│   │   │               │   └── TipoRegistro.java
│   │   │               ├── repository/
│   │   │               │   ├── UsuarioRepository.java
│   │   │               │   └── RegistroPontoRepository.java
│   │   │               ├── service/
│   │   │               │   ├── UsuarioService.java
│   │   │               │   └── RegistroPontoService.java
│   │   │               ├── dto/
│   │   │               │   ├── UsuarioDTO.java
│   │   │               │   ├── RegistroPontoDTO.java
│   │   │               │   └── AutenticacaoDTO.java
│   │   │               └── exception/
│   │   │                   ├── GlobalExceptionHandler.java
│   │   │                   └── RecursoNaoEncontradoException.java
│   │   │
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── application-dev.properties
│   │       ├── application-prod.properties
│   │       └── application-test.properties
│   │
│   └── test/
│       └── java/
│           └── com/
│               └── empresa/
│                   └── controleponto/
│                       ├── service/
│                       │   ├── UsuarioServiceTest.java
│                       │   └── RegistroPontoServiceTest.java
│                       └── controller/
│                           ├── UsuarioControllerTest.java
│                           └── RegistroPontoControllerTest.java
│
├── .gitignore
├── README.md
└── pom.xml
```

</div> 

</details>

## Tecnologias Utilizadas
- Java 17
- Spring Boot 3.2.1
- Hibernate Envers
- Lombok
- H2 Database
- Swagger/OpenAPI

## Configuração do Ambiente

### Pré-requisitos
- JDK 17
- Maven

### Instalação
1. Clone o repositório
```bash
git clone https://github.com/bulletdev/ControleDePonto.git
cd ControleDePonto
```

2. Compile o projeto
```bash
mvn clean install
```

3. Rode a aplicação
```bash
mvn spring-boot:run
```

## Documentação da API
Após iniciar a aplicação, acesse:
- Swagger UI: `http://localhost:8080/swagger-ui.html`
- API Docs: `http://localhost:8080/v3/api-docs`

## Banco de Dados
A aplicação utiliza H2 em memória. 
- Console do H2: `http://localhost:8080/h2-console`
- JDBC URL: `jdbc:h2:mem:pontoacessodb`
- Username: `sa`
- Sem senha

## Recursos
- Cadastro de Usuários
- Registro de Ponto
- Auditoria de Alterações
- Controle de Acesso

## Contribuição
1. Faça um fork do projeto
2. Crie sua feature branch (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Licença
[Michael Bullet]
