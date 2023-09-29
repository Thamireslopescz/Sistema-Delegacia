# Sistema de Delegacia de Polícia
![download](https://github.com/Thamireslopescz/Sistema-Delegacia/assets/100656019/cdadaa8b-c9c8-44df-8b99-31d503c0a1a9)


Este é um projeto de exemplo para um sistema de delegacia de polícia que utiliza Prisma e Express.js para realizar operações CRUD (Create, Read, Update, Delete) em criminosos, crimes e armas. 
O sistema permite o registro e gerenciamento de informações sobre criminosos, crimes e as armas envolvidas.

## Pré-requisitos

Antes de executar este projeto, certifique-se de ter instalado o seguinte:

- Node.js: https://nodejs.org/
- PostgreSQL: https://www.postgresql.org/
- Prisma CLI: Você pode instalá-lo globalmente com `npm install -g prisma` ou usá-lo como uma dependência de desenvolvimento no projeto.

## Configuração

1. Clone este repositório:

   ```bash
   git clone https://github.com/seu-usuario/delegacia-policial.git
   cd delegacia-policial
   ```

2. Instale as dependências:

   ```bash
   npm install
   ```

3. Configure as variáveis de ambiente:

   Crie um arquivo `.env` na raiz do projeto e configure as variáveis de ambiente conforme necessário. Você pode usar um banco de dados PostgreSQL local ou hospedado. Aqui está um exemplo de `.env`:

   ```env
   DATABASE_URL=postgresql://seu_usuario:senha@localhost:5432/nome_do_banco
   ```

4. Execute as migrações do Prisma para criar as tabelas no banco de dados:

   ```bash
   npx prisma migrate dev
   ```

## Uso

Para iniciar o servidor, execute o seguinte comando:

```bash
npm start
```

O servidor estará disponível em `http://localhost:3001`.

### Rotas API

- `GET /criminosos`: Lista todos os criminosos registrados.
- `POST /criminosos`: Cria um novo criminoso.
- `PUT /criminosos/:id`: Atualiza informações de um criminoso existente.
- `DELETE /criminosos/:id`: Deleta um criminoso.

- `GET /crimes`: Lista todos os crimes registrados.
- `POST /crimes`: Cria um novo crime.
- `PUT /crimes/:id`: Atualiza informações de um crime existente.
- `DELETE /crimes/:id`: Deleta um crime.

- `GET /armas`: Lista todas as armas registradas.
- `POST /armas`: Cria uma nova arma.
- `PUT /armas/:id`: Atualiza informações de uma arma existente.
- `DELETE /armas/:id`: Deleta uma arma.

## Contribuição

Contribuições são bem-vindas! Se você deseja contribuir para este projeto, siga estas etapas:

1. Faça um fork do repositório.
2. Crie uma branch com sua feature: `git checkout -b minha-feature`.
3. Faça commit das suas alterações: `git commit -m 'Adicione uma nova feature'`.
4. Envie suas alterações: `git push origin minha-feature`.
5. Abra um pull request.


Feito com ❤️ por [Thamires Lopes e Lucas Siki].
