# Projeto FIAP - Sistema de Gestão de Produtos

Este é um projeto de sistema de gestão de produtos desenvolvido na FIAP. O sistema permite cadastrar, editar, listar e excluir produtos, além de possibilitar o login de usuários.

## Arquitetura e Tecnologias

- **Java**: Linguagem principal do projeto.
- **Servlets**: Para controle das requisições HTTP.
- **JDBC**: Conexão com banco de dados Oracle.
- **JSP**: Para renderização das páginas web.
- **Oracle Database**: Banco de dados utilizado.
- **DAO Pattern**: Padrão de persistência para acesso aos dados.

## Estrutura de Pacotes

### `br.com.fiap.connection`

- **ConnectionManager**: Gerencia a conexão com o banco de dados.

### `br.com.fiap.controller`

- **LoginServlet**: Controle das requisições de login.
- **ProdutoServlet**: Controle das operações de CRUD de produtos.

### `br.com.fiap.dao`

- **CategoriaDAO**: Interface para operações com categorias.
- **ProdutoDAO**: Interface para operações com produtos.
- **UsuarioDAO**: Interface para operações com usuários.

### `br.com.fiap.exception`

- **DBException**: Exceção customizada para erros de banco de dados.

### `br.com.fiap.factory`

- **DAOFactory**: Fabrica os DAOs necessários para acesso ao banco.

### `br.com.fiap.filter`

- **LoginFilter**: Filtra requisições para autenticação de usuários.

## Modelos

- **Categoria**: Representa as categorias dos produtos.
- **Produto**: Contém informações dos produtos.
- **Usuario**: Contém informações dos usuários.

## Funcionalidades

1. **Autenticação de Usuário**:
   - Login de usuários.
   - Filtro de segurança em URLs restritas.

2. **Gestão de Produtos**:
   - Cadastro, edição, listagem e exclusão de produtos.
   - Associação de produtos com categorias.

## Como Executar

1. **Configurar Banco de Dados**:
   - Certifique-se de ter um banco de dados Oracle configurado conforme as especificações do projeto.

2. **Configurar Conexão com o Banco**:
   - Atualize as credenciais de banco no `ConnectionManager`.

3. **Implantar aplicação em um servidor de aplicação**:
   - Exemplo: Apache Tomcat.

4. **Acessar a Aplicação**:
   - Utilize um navegador para interagir com as funcionalidades disponíveis.

## Considerações Finais

- Certifique-se de ter as bibliotecas JDBC necessárias para conectar ao Oracle Database.
- Este projeto foi desenvolvido para fins educacionais na FIAP e pode ser expandido para incluir mais funcionalidades conforme a necessidade.
