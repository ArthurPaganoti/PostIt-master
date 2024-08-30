## Descrição
Este projeto é uma aplicação de gerenciamento de notas adesivas (Post-Its) desenvolvida como parte do trabalho de Engenharia de Software. A aplicação permite aos usuários criar, salvar e gerenciar notas com título, descrição e prazo. Para o desenvolvimento, utilizamos metodologias ágeis, combinando práticas de Scrum e Kanban para assegurar uma entrega eficiente e organizada.

## Tecnologias Utilizadas
- *Linguagem de Programação:* Java
- *Gerenciador de Dependências:* Maven
- *Banco de Dados:* MySQL
- *IDE:* IntelliJ IDEA 2024.1.4

## Estrutura do Projeto
O projeto segue uma estrutura MVC (Model-View-Controller) para separar as responsabilidades e facilitar a manutenção do código.

### Model
A camada de modelo contém as classes que representam os dados da aplicação. No caso deste projeto, a classe PostIt é responsável por representar uma nota adesiva.

### View
A camada de visualização é responsável pela interface do usuário. No entanto, este projeto não inclui uma implementação de interface gráfica, focando apenas na lógica de backend.

### Controller
A camada de controle gerencia a lógica de negócios e a comunicação entre a camada de modelo e a camada de visualização. A classe PostItController é responsável por gerenciar as operações relacionadas aos Post-Its.

## Configuração do Banco de Dados
As configurações do banco de dados são armazenadas no arquivo .env:

DB_URL=jdbc:mysql://localhost:3306/postit_db
DB_USER=seu_nome_do_banco_de_dados
DB_PASSWORD=sua_senha_do_banco_de_dados
DB_MAX_POOL_SIZE=10


## Padrões de Projeto Utilizados
- *DAO (Data Access Object):* Utilizado para abstrair e encapsular o acesso ao banco de dados.
- *MVC (Model-View-Controller):* Utilizado para separar as responsabilidades da aplicação.

## Como Executar
1. Clone o repositório.
2. Configure o banco de dados MySQL e atualize o arquivo .env com suas credenciais.
3. Execute o comando mvn clean install para instalar as dependências.
4. Execute a aplicação a partir da classe principal.
