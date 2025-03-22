# Pratica-02---Construcao-de-Servico-Web
# Projetos: Demo e FIPE

Este repositório contém dois projetos independentes:

1. **Demo**
2. **FIPE**

Cada projeto tem sua própria estrutura e propósito. Abaixo, apresento detalhes técnicos sobre os códigos e as pastas incluídas em cada um.

---

## Projeto Demo

Este é um projeto Java Spring Boot configurado para gerenciar uma aplicação simples com controle de produtos.

### Estrutura do Projeto

- **`.git`**: Contém arquivos de controle de versão do Git.
- **`.mvn`**: Configurações do Maven Wrapper.
- **`.vscode`**: Arquivos de configuração do Visual Studio Code.
- **`src/main/java/com/example/demo`**:
  - `DemoApplication.java`: Classe principal responsável por inicializar a aplicação Spring Boot.
  - `controller/HelloController.java`: Controlador com endpoints de teste ou exemplo.
  - `controller/ProdutoController.java`: Controlador para gerenciar operações de produtos (CRUD).
  - `model/Produto.java`: Classe que representa o modelo de dados de produtos.
- **`src/main/resources/application.properties`**: Arquivo de configuração principal da aplicação.
- **`src/test`**: Contém os testes da aplicação, incluindo a classe `DemoApplicationTests.java`.
- **`target`**:
  - Contém arquivos gerados após a compilação do projeto.

### Configurações Importantes

- **Dependências**: Especificadas no arquivo `pom.xml`, incluindo frameworks e bibliotecas do Spring Boot.
- **Porta Default**: Configurada no `application.properties`.

### Como Executar o Projeto

1. Certifique-se de ter o Maven e o JDK 17 ou superior instalados.
2. No terminal, navegue até a raiz do projeto.
3. Execute:
   ```bash
   ./mvnw spring-boot:run
   ```
4. A aplicação estará acessível na porta configurada (padrão: 8080).

---

## Projeto FIPE

Este projeto Java Spring Boot é destinado à integração com a Tabela FIPE, fornecendo endpoints para consultar informações sobre veículos.

### Estrutura do Projeto

- **`fipe`**: Pasta principal contendo o projeto completo.
- **`.mvn`**: Configurações do Maven Wrapper.
- **`fipe/src/main/java/com/api/fipe`**:
  - `FipeApplication.java`: Classe principal responsável por inicializar o projeto FIPE.
  - `controller/FipeController.java`: Controlador para gerenciamento de endpoints relacionados à FIPE.
  - `service/FipeService.java`: Classe de serviço contendo a lógica de negócio para as operações FIPE.
- **`fipe/src/main/resources/application.properties`**: Configuração principal do projeto.
- **`fipe/src/test`**: Contém testes para a aplicação, incluindo `FipeApplicationTests.java`.
- **`fipe/target`**:
  - Arquivos gerados após a compilação do projeto.

### Configurações Importantes

- **Dependências**: Especificadas no arquivo `fipe/pom.xml`, com integração do Spring Boot e outras bibliotecas necessárias.
- **Porta Default**: Configurada no `application.properties`.

### Como Executar o Projeto

1. Certifique-se de ter o Maven e o JDK 17 ou superior instalados.
2. No terminal, navegue até a pasta `fipe`.
3. Execute:
   ```bash
   ./mvnw spring-boot:run
   ```
4. A aplicação estará acessível na porta configurada (padrão: 8080).

---

## Observações Gerais

- Certifique-se de que as dependências Maven sejam baixadas antes de executar os projetos.
- Ajuste as configurações no arquivo `application.properties` conforme necessário (ex.: conexões com bancos de dados ou integrações).

