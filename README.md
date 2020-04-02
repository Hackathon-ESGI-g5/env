Clone repository
```
git clone git@github.com:Hackathon-ESGI-g5/env.git
```

Init submodules
```
git submodule init
```

Deploy submodules
```
git submodule update
```

Add .env file on **api/** project
```
HOST=0.0.0.0
PORT=3333
NODE_ENV=development
APP_NAME=AdonisJs
APP_URL=http://${HOST}:${PORT}
CACHE_VIEWS=false
APP_KEY=glV1t8egyqVdSALLJDcBYlzFp1GD2aio

DB_CONNECTION=pg
DB_HOST=hackathon_postgresql
DB_PORT=5432
DB_USER=adonis
DB_PASSWORD=adonis
DB_DATABASE=hackathon

HASH_DRIVER=bcrypt

SMTP_HOST=hackathon-mailhog
SMTP_PORT=1025
MAIL_SENDER=contact@safeshop.fr

FRONT_URL=http://safeshop.fr
```

Download dependencies for front
```
docker-compose run hackathon-app yarn install
```

Start environement
```
docker-compose up -d --build
```