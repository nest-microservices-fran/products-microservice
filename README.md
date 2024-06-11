# Product Microservice

## Dev

1. Clonar el repositorio
2. Instalar dependencias

```
npm install
```

3. Copiar y renombrar el archivo `.env.template` a `.env`
4. Ejecutar migración de prisma

```
npx prisma migrate dev
```

5. Levantar servidor de nats

```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```

6. Ejecutar

```
npm run start:dev
```
