<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

# Nest-MicroServices - Client Gateway

Repositorio para el Gateway de la aplicación Products realizada en [Nest](https://github.com/nestjs/nest). 
Basado en el curso de "NestJs + Microservicios: Aplicaciones escalables y modulares" de [DevTalles](https://cursos.devtalles.com/) en Udemy.

## Lanzar el proyecto completo

Seguir las indicaciones del launcher para lanzar todos los proyectos

## Configuración del proyecto

1. Instalar NestJS CLI

```bash
$ npm i -g @nestjs/cli
```

2. Clonar el repositorio

3. Instalar las dependencias

```bash
$ npm install
```

4. Crear un archivo ```.env``` basado en ```.env.template```.

5. Levantar el servidor de NATS

```bash
$ docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```

6. Levantar todos los microservicios consumidos

7. Ejecutar el proyecto

```bash
$ npm run start:dev
```

## Producción

Ejecutar

```bash
$ docker build -f Dockerfile.prod -t client-gateway .
```

## Aspectos estudiados

En este repositorio se trabajan los siguientes aspectos de Nest con microservicios:
-	Envío de payload hacia el microservicio
- Enviar mensajes del gateway al microservicio
- Configuración de excepciones:
  - Independientes
  - Globales
- Trabajar con observables y promesas en los mensajes
- Implementando endpoints para Order
- Validación de orden con su detalle de orden
- Agregar NATS como canal de comunicación

## Librerías utilizadas

Para la gestión de microservicios:

```bash
$ npm i --save @nestjs/microservices
```

Para la gestión de variables de entorno:

```bash
$ npm install dotenv
```

Para los esquemas de validación:

```bash
$ npm install joi
```

Para las validaciones se utilizan:

```bash
$ npm install class-validator class-transformer
```

Para utilizar NATS para las comunicaciones del microservicio:

```bash
$ npm i --save nats
```
