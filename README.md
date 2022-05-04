[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/hebertcisco/nestjs-rest-boilerplate)

# Basic documentation

## Postgres with Docker
> Up an image and run postgres image with docker

```sh
docker run --name db_pg -p 5432:5432 -e POSTGRES_PASSWORD=postgres -e POSTGRES_USER=postgres -d postgres:11
```

## Environment variables

> Create a `.env` file in the root directory of your project

```dotenv
POSTGRES_DATABASE="postgres"
POSTGRES_HOST="127.0.0.1"
POSTGRES_USER="postgres"
POSTGRES_PASSWORD="postgres"
POSTGRES_PORT=5432

PORT=3333
APP_SECRET='senhona_grossa'
MODE="DEV"
```

## Runing the application with docker

### Run as dev 

```sh
docker-compose up dev
```

### Run as prod

```sh
docker-compose up -d prod
```

## Runing the application with npm scrips

```sh
npm install && npm run build
```
```sh
npm run prepare:enviroment
```

### Run as dev

```sh
npm run dev
```
or
```sh
npm run dev:test
```

### Run as prod

```sh
npm run start
```
or 
```sh
npm run start:prod
```

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](issues).

## Show your support

Give a ⭐️ if this project helped you!

Or buy me a coffee 🙌🏾

<a href="https://www.buymeacoffee.com/hebertcisco">
    <img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=hebertcisco&button_colour=FFDD00&font_colour=000000&font_family=Inter&outline_colour=000000&coffee_colour=ffffff" />
</a>

## 📝 License

Copyright © 2022 [Hebert F Barros](https://github.com/hebertcisco).<br />
This project is [MIT](LICENSE) licensed.
