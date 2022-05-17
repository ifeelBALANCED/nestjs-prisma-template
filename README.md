# NestJS Prisma Docker

> DON'T commit .env files into version control, add `.env` to `.gitignore`. `.env` files are added here as an example.

Develop the Nest application

```bash
yarn install

cp .env.example .env

npx prisma generate

yarn run start:dev
```

## Docker File

Get started by running

```bash
docker build -t project_name .

docker run -p 5000:5000 --env-file .env -d project_name
```

## Docker Compose

```bash
docker-compose up
# or detached
docker-compose up -d
```
