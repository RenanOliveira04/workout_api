# Workout API

Este repositório contém a implementação de uma API para gerenciamento de rotinas de exercícios físicos. A API permite criar, atualizar, visualizar e excluir informações sobre exercícios e treinos. A seguir, você encontrará instruções sobre como configurar e utilizar o projeto.

## Índice

- [Pré-requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Configuração](#configuração)
- [Uso](#uso)
- [Endpoints](#endpoints)
- [Contribuindo](#contribuindo)
- [Licença](#licença)

## Pré-requisitos

Antes de começar, você precisará ter as seguintes ferramentas instaladas em sua máquina:

- [Python 3.x](https://www.python.org/downloads/)
- [pip](https://pip.pypa.io/en/stable/installation/)

## Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/RenanOliveira04/workout_api.git
   ```

2. Navegue até o diretório do projeto:

   ```bash
   cd workout_api
   ```

3. Crie e ative um ambiente virtual:

   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
   ```

4. Instale as dependências:

   ```bash
   pip install -r requirements.txt
   ```

## Configuração

1. Crie um arquivo `.env` na raiz do projeto e configure as variáveis de ambiente necessárias:

   ```
   SECRET_KEY=<sua_secret_key>
   DATABASE_URL=<sua_url_do_banco_de_dados>
   ```

## Uso

1. Execute as migrações do banco de dados:

   ```bash
   python manage.py migrate
   ```

2. Inicie o servidor:

   ```bash
   python manage.py runserver
   ```

3. Acesse a API no seu navegador ou via ferramenta de requisição (por exemplo, [Postman](https://www.postman.com/)):

   ```
   http://127.0.0.1:8000/
   ```

## Endpoints

### Exercícios

- **GET /exercises/**: Lista todos os exercícios.
- **POST /exercises/**: Cria um novo exercício.
- **GET /exercises/{id}/**: Retorna os detalhes de um exercício específico.
- **PUT /exercises/{id}/**: Atualiza um exercício específico.
- **DELETE /exercises/{id}/**: Exclui um exercício específico.

### Treinos

- **GET /workouts/**: Lista todos os treinos.
- **POST /workouts/**: Cria um novo treino.
- **GET /workouts/{id}/**: Retorna os detalhes de um treino específico.
- **PUT /workouts/{id}/**: Atualiza um treino específico.
- **DELETE /workouts/{id}/**: Exclui um treino específico.

## Contribuindo

Contribuições são bem-vindas! Se você tiver alguma ideia ou encontrar algum problema, por favor, abra uma issue ou envie um pull request.

1. Fork o projeto
2. Crie uma nova branch (`git checkout -b feature/nova-feature`)
3. Commit suas alterações (`git commit -am 'Adiciona nova feature'`)
4. Envie para o branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

Esperamos que este guia seja útil. Se você tiver alguma dúvida ou precisar de ajuda, sinta-se à vontade para entrar em contato.

Boas práticas e bons treinos! 💪

---

Renan Oliveira  
[GitHub](https://github.com/RenanOliveira04)  
[LinkedIn](https://www.linkedin.com/in/renanoliveira04)  
