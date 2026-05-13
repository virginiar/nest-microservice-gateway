<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

# Nest-MicroServices - Client Gateway

Repositorio para el Gateway de la aplicación Products realizada en [Nest](https://github.com/nestjs/nest). 
Basado en el curso de "NestJs + Microservicios: Aplicaciones escalables y modulares" de [DevTalles](https://cursos.devtalles.com/) en Udemy.

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

5. Levantar todos los microservicios consumidos

6. Ejecutar el proyecto

```bash
$ npm run start:dev
```

## Aspectos estudiados

En este repositorio se trabajan los siguientes aspectos de Nest con microservicios:
-	Envío de payload hacia el microservicio
- Enviar mensajes del gateway al microservicio
- Configuración de excepciones:
  - Independientes
  - Globales
- Trabajar con observables y promesas en los mensajes

## Librerías utilizadas

Para las validaciones se utilizan:

```bash
$ npm install class-validator class-transformer
```

Para la gestión de variables de entorno:

```bash
$ npm install dotenv
```

Para los esquemas de validación:

```bash
$ npm install joi
```

Para la gestión de microservicios:

```bash
$ npm i --save @nestjs/microservices
```