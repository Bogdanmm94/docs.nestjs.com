### Introducción

Nest (NestJS) es un marco de trabajo para construir aplicaciones eficientes y escalables del lado del servidor [Node.js](https://nodejs.org/). Utiliza JavaScript progresivo, está construido y totalmente compatible con [TypeScript](http://www.typescriptlang.org/) (aunque todavía permite a los desarrolladores programar en JavaScript puro) y combina elementos de OOP (Programación Orientada a Objetos), FP (Programación Funcional) y FRP (Programación Reactiva Funcional).

Bajo el capó, Nest hace uso de robustos marcos de trabajo de servidor HTTP como [Express](https://expressjs.com/) (el predeterminado) y opcionalmente puede configurarse para usar [Fastify](https://github.com/fastify/fastify) ¡también!

Nest proporciona un nivel de abstracción por encima de estos marcos de trabajo comunes de Node.js (Express/Fastify), pero también expone sus APIs directamente al desarrollador. Esto les da a los desarrolladores la libertad de usar la gran cantidad de módulos de terceros disponibles para la plataforma subyacente.

#### Filosofía

En los últimos años, gracias a Node.js, JavaScript se ha convertido en la "lengua franca" de la web tanto para aplicaciones de frontend como de backend. Esto ha dado lugar a proyectos increíbles como [Angular](https://angular.io/), [React](https://github.com/facebook/react) y [Vue](https://github.com/vuejs/vue), que mejoran la productividad de los desarrolladores y permiten la creación de aplicaciones frontend rápidas, testables y escalables. Sin embargo, aunque existen muchas bibliotecas, ayudantes y herramientas excelentes para Node (y JavaScript del lado del servidor), ninguna de ellas resuelve eficazmente el problema principal de la **arquitectura**.

Nest proporciona una arquitectura de aplicación lista para usar que permite a los desarrolladores y equipos crear aplicaciones altamente testables, escalables, débilmente acopladas y fácilmente mantenibles. La arquitectura está fuertemente inspirada en Angular.

#### Instalación

Para empezar, puedes crear el esqueleto del proyecto con el [Nest CLI](/cli/overview) o clonar un proyecto de inicio (ambos producirán el mismo resultado).

Para crear el esqueleto del proyecto con el Nest CLI, ejecuta los siguientes comandos. Esto creará un nuevo directorio de proyecto y poblará el directorio con los archivos principales iniciales de Nest y los módulos de soporte, creando una estructura base convencional para tu proyecto. La creación de un nuevo proyecto con el Nest CLI se recomienda para los usuarios que lo usan por primera vez. Continuaremos con este enfoque en [Primeros Pasos](first-steps).

```bash
$ npm i -g @nestjs/cli
$ nest new project-name
```

> info **Pista** Para crear un nuevo proyecto con Typescript con el modo [estricto](https://www.typescriptlang.org/tsconfig#strict) pase el indicador `--strict` al comando `nest new`. 

#### Alternativas

Como alternativa, puede instalar el proyecto de inicio de TypeScript con **Git**:
```bash
$ git clone https://github.com/nestjs/typescript-starter.git project
$ cd project
$ npm install
$ npm run start
```

> info **Pista** Si desea clonar el repositorio sin el historial de git, puede usar [degit](https://github.com/Rich-Harris/degit).

Abra su navegador y navegue a [`http://localhost:3000/`](http://localhost:3000/).

Para instalar la versión en JavaScript del proyecto de inicio, use `javascript-starter.git`  en la secuencia de comandos anterior.

También puede crear manualmente un nuevo proyecto desde cero instalando los archivos principales y de soporte con **npm** (o **yarn**). En este caso, por supuesto, será responsable de crear los archivos de la plantilla del proyecto usted mismo.

```bash
$ npm i --save @nestjs/core @nestjs/common rxjs reflect-metadata
```
