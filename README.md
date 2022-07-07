# Multiplier-NodeJS-Challenge

## Description

Luis F's NodeJS integration challenge to <a href="http://multiplier.com.br" target="_blank">Multiplier</a>

### Technologies

<a href="https://nestjs.com/"><img src="https://img.shields.io/badge/-NestJS-30363D?style=flat&amp;logo=nestjs" alt="NestJS"/></a> <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/-Typescript-30363D?style=flat&amp;logo=typescript" alt="Typescript"/></a> <a href="https://nodejs.org/en/"><img src="https://img.shields.io/badge/-NodeJS-30363D?style=flat&amp;logo=node.js" alt="NodeJS"/></a> <a href="https://insomnia.rest/"><img src="https://img.shields.io/badge/-Insomnia-30363D?style=flat&amp;logo=insomnia" alt="Insomnia"/></a> <a href="https://dbeaver.io/"><img src="https://img.shields.io/badge/-DBeaver-30363D?style=flat&amp;logo=dbeaver" alt="DBeaver"/></a> <a href="https://sequelize.org/"><img src="https://img.shields.io/badge/-Sequelize-30363D?style=flat&amp;logo=sequelize" alt="Sequelize"/></a>

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Testing

```bash
# testing
$ npm run test
```

## Documentation

### Resource Changes

Some column names was translated to English, you can verify the changes here:

#### Categories

| Column | Type    | Description                | OG Column
|--------|---------|----------------------------|--------|
| id     | int     | Table primary key          | id
| slug   | varchar | Category code              | codigo
| title  | varchar | Category title             | titulo
| status | int     | 0 - Inactive, 1 - Active   | status

#### Products

| Column      | Type    | Description              | OG Column
|-------------|---------|--------------------------|-------|
| id          | int     | Table primary key | id
| categoryId | int     | Category foreign key     | idCategoria
| sku      | varchar | Product SKU           | codigo
| name        | varchar | Product name          | nome
| description   | text    | Product description     | descricao
| price       | decimal | Product price         | valor
| status      | int     | 0 - Inactive, 1 - Active   | status

#### Stock

| Column     | Type    | Description                | OG Column
|------------|---------|--------------------------|-------|
| id         | int     | Table primary key | id
| productId  | int     | Product foreign key       | idProduto
| qty | int     | Stock quantity    | quantidade
| reserve    | int     | Reserve     | reserva
| status     | int     | 0 - Inactive, 1 - Active   | status

### Backup

The backup is done automatically from MySQL to PostgreSQL every 10 seconds.
Don't forget to verify the *dotenv* PostgreSQL variables.

## Author

<a href="https://twitter.com/luisfloat"><img src="https://img.shields.io/badge/-Twitter-30363D?style=flat&amp;logo=twitter" alt="Twitter"/></a> <a href="https://github.com/luisfloat"><img src="https://img.shields.io/badge/-Github-30363D?style=flat&amp;logo=github" alt="Github"/></a> <a href="https://instagram.com/luisfloat"><img src="https://img.shields.io/badge/-Instagram-30363D?style=flat&amp;logo=instagram" alt="Instagram"/></a> <a href="mailto:contact@luisfloat.com"><img src="https://img.shields.io/badge/-Gmail-30363D?style=flat&amp;logo=gmail" alt="Gmail"/></a>

## License

License undefined.
