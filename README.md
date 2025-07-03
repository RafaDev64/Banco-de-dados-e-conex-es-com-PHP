# Sistema de Gerenciamento de Livros

## Descrição
Este projeto é um sistema web desenvolvido em **PHP** e **MySQL** para gerenciamento de uma biblioteca de livros. Ele inclui uma página de login com autenticação segura, cadastro de usuários e operações **CRUD** (Criar, Ler, Atualizar e Excluir) para gerenciar livros. A interface é estilizada com **Bootstrap 5.3**, garantindo um design responsivo e amigável.

### Funcionalidades
- **Autenticação de Usuários**:
  - Login com verificação de credenciais usando hash de senhas (`password_hash`).
  - Cadastro de novos usuários com armazenamento seguro de senhas.
- **Gerenciamento de Livros**:
  - **Criar**: Adicionar novos livros com título, autor e ano.
  - **Ler**: Exibir a lista de livros em uma tabela.
  - **Atualizar**: Editar informações de livros existentes.
  - **Excluir**: Remover livros com confirmação.
- **Segurança**:
  - Uso de prepared statements para prevenir SQL Injection.
  - Gerenciamento de sessões para controle de acesso.
- **Interface**: Design moderno e responsivo com Bootstrap.

## Tecnologias Utilizadas
- **PHP**: Backend para lógica do sistema e conexão com banco de dados.
- **MySQL**: Banco de dados relacional para armazenar usuários e livros.
- **Bootstrap 5.3**: Framework CSS para estilização.
- **MySQLi**: Extensão PHP para interação com o banco de dados.

## Estrutura do Projeto
- `index.php`: Página de login.
- `register.php`: Página de cadastro de usuários.
- `dashboard.php`: Painel principal com listagem e gerenciamento de livros.
- `edit.php`: Página para edição de livros.
- `logout.php`: Script para encerrar a sessão.
- `config.php`: Configuração da conexão com o banco de dados.
- `database.sql`: Script SQL para criar o banco de dados e tabelas.

## Pré-requisitos
- Servidor web (ex.: Apache) com PHP habilitado.
- MySQL instalado e configurado.
- Extensão MySQLi habilitada no PHP.

## Instruções de Configuração
1. **Banco de Dados**:
   - Execute o script `database.sql` no MySQL para criar o banco `library` e as tabelas `users` e `books`.
   - Atualize as credenciais no arquivo `config.php` conforme seu ambiente.

2. **Instalação**:
   - Copie os arquivos para o diretório raiz do seu servidor web (ex.: `htdocs` no XAMPP).
   - Certifique-se de que o servidor web e o MySQL estão em execução.

3. **Acesso**:
   - Acesse `index.php` no navegador para fazer login ou cadastrar um novo usuário.
   - Após login, o sistema redireciona para o `dashboard.php`, onde é possível gerenciar os livros.

## Como Usar
1. Faça login com um usuário existente ou cadastre-se em `register.php`.
2. No painel principal (`dashboard.php`), adicione, edite ou exclua livros.
3. Use o botão de logout para sair do sistema.

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias, como:
- Adição de novas funcionalidades (ex.: filtros de busca, categorias de livros).
- Melhorias na interface ou experiência do usuário.
- Otimizações de desempenho ou segurança.

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).
