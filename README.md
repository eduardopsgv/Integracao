# Sistema de Gerenciamento de Biblioteca

Este projeto é um sistema simples de gerenciamento de uma biblioteca, utilizando SQLite para armazenar informações sobre autores, livros e empréstimos.

## Funcionalidades

- Cadastro de autores
- Cadastro de livros, com referência aos autores
- Registro de empréstimos de livros

## Estrutura do Banco de Dados

O banco de dados é composto por três tabelas:

1. **Autores**
   - `AutorID`: ID do autor (chave primária)
   - `Nome`: Nome do autor
   - `Nacionalidade`: Nacionalidade do autor

2. **Livros**
   - `LivroID`: ID do livro (chave primária)
   - `Titulo`: Título do livro
   - `AutorID`: ID do autor (chave estrangeira)
   - `AnoPublicacao`: Ano de publicação do livro
   - `Genero`: Gênero do livro

3. **Emprestimos**
   - `EmprestimoID`: ID do empréstimo (chave primária)
   - `LivroID`: ID do livro emprestado (chave estrangeira)
   - `DataEmprestimo`: Data do empréstimo
   - `DataDevolucao`: Data de devolução
   - `NomeUsuario`: Nome do usuário que fez o empréstimo

## Como Executar

1. Clone este repositório.
2. Certifique-se de ter o Python e SQLite instalados em sua máquina.
3. Execute o script `main.py` para criar o banco de dados e inserir dados de exemplo.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
