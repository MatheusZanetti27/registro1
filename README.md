# registro1
Meu primeiro sistema de registro utilizando mysql.

```markdown
# Sistema de Registro de Usuários

Projeto de aplicação web para cadastro e gerenciamento de usuários, desenvolvido com o objetivo de implementar a integração entre interface de usuário (front-end), lógica de negócios (back-end) e persistência de dados em um banco de dados relacional.

## Tecnologias e Ferramentas

O desenvolvimento deste sistema baseou-se na seguinte pilha tecnológica:

* **HTML5:** Estruturação semântica das interfaces de usuário.
* **CSS3:** Estilização e responsividade da aplicação.
* **PHP:** Processamento de requisições, validação de dados e regras de negócio.
* **MySQL:** Sistema de gerenciamento de banco de dados relacional para armazenamento de informações.
* **XAMPP:** Ambiente de desenvolvimento local provendo os serviços Apache e MySQL.

## Funcionalidades Implementadas

* Processamento e validação de formulários de cadastro no lado do servidor.
* Estabelecimento de conexão segura com o banco de dados MySQL via interface PDO (PHP Data Objects).
* Tratamento de exceções e prevenção de redundância de dados (ex: restrição de e-mails duplicados).
* Arquitetura de interface voltada para a usabilidade e clareza das informações.

## Estrutura do Diretório

```text
├── css/
│   └── style.css          # Arquivos de folha de estilo
├── db/
│   └── database.sql       # Script DDL para inicialização do banco de dados e tabelas
├── config.php             # Parâmetros de configuração e rotinas de conexão com o banco
├── cadastrar.php          # Lógica de processamento das requisições do formulário
├── index.html             # Interface principal da aplicação
└── README.md              # Documentação técnica do projeto

```

## Instruções para Execução Local

Para provisionar este projeto em um ambiente de desenvolvimento local, é necessário possuir o XAMPP ou pacote equivalente (servidor web e MySQL) previamente configurado.

### 1. Preparação do Repositório

Realize o clone ou download do repositório e aloque o diretório na raiz de documentos do seu servidor local:

* Ambientes Windows: `C:\xampp\htdocs\nome-do-repositorio`
* Ambientes Linux: `/opt/lampp/htdocs/nome-do-repositorio`

### 2. Configuração do Banco de Dados

1. Inicie os serviços Apache e MySQL através do painel de controle do XAMPP.
2. Acesse a interface de administração do banco de dados (geralmente em `http://localhost/phpmyadmin/`).
3. Instancie um novo banco de dados (recomendado: `sistema_registro`).
4. Execute a importação do arquivo `database.sql`, localizado no subdiretório `db/` deste projeto, para gerar as tabelas necessárias.

### 3. Configuração de Credenciais

Caso o seu ambiente local possua credenciais distintas do padrão de instalação, atualize as variáveis de conexão no arquivo `config.php`:

```php
$host = "localhost";
$dbname = "sistema_registro";
$username = "root"; // Usuário de acesso ao MySQL
$password = "";     // Senha de acesso ao MySQL

```

### 4. Inicialização

Para acessar a aplicação, utilize o navegador web apontando para o endereço de *localhost* seguido do diretório do projeto:

```text
http://localhost/nome-do-repositorio/

```

## Competências Desenvolvidas

A arquitetura e o desenvolvimento deste sistema permitiram a aplicação prática dos seguintes conceitos de engenharia de software:

* Gerenciamento de requisições baseadas no protocolo HTTP (métodos POST e GET).
* Implementação de boas práticas de segurança, visando a mitigação de vulnerabilidades comuns, como ataques de *SQL Injection*, por meio do uso de *Prepared Statements*.
* Estruturação de instruções SQL em ambiente de produção para operações de inserção e consulta de dados.

---

Desenvolvido por Matheus Zanetti

```

```
