# Prueba Técnica – API REST de Productos

Este proyecto es una API RESTful desarrollada para gestionar productos. Permite realizar operaciones de **creación, modificación, consulta, eliminación**, así como la **activación e inactivación** de productos. La información se almacena en una base de datos PostgreSQL.

---

## ⚙️ Configuración del Proyecto

### `.env.template`

Este archivo contiene las variables de entorno necesarias para el funcionamiento de la API. Para configurarlo:

1. Renombra el archivo `.env.template` a `.env`.
2. Asigna valores válidos a las variables, por ejemplo:

```
env
PORT=3000                    # Puerto donde se expondrá la API
DATABASE_URL=postgres://... # Cadena de conexión a PostgreSQL
```

## 📁 Archivos Adicionales
A continuación se describen los archivos adicionales incluidos en el proyecto:

### api-products.postman_collection.json
Colección de Postman con ejemplos de los endpoints expuestos por la API api-products. Puedes importarla directamente en la aplicación Postman para probar fácilmente cada ruta.

### example-CI.yml
Workflow de GitHub Actions para Integración Continua (CI). Ejecuta:

Instalación de dependencias.

Linting y pruebas unitarias.

Sirve para validar que el proyecto funcione correctamente antes de aceptar cambios en el código.

### example-CD.yml
Workflow de GitHub Actions para Despliegue Continuo (CD). Este archivo simula el proceso de despliegue de la API de forma local. Puede extenderse fácilmente para apuntar a un entorno real (por ejemplo, AWS o Vercel).

## 🧪 Requisitos y dependencias
* Node.js v22.17.0

* Yarn

* PostgreSQL

* Postman (opcional, para probar endpoints)

### ¿Cómo ejecutar la API?

Crea el archivo .env a partir de .env.template.

#### Instala dependencias:
``` 
bash
yarn install
```

#### Ejecuta la API:
```
bash
yarn start:dev
```

### Pruebas Unitarias
Puedes ejecutar las pruebas unitarias con:
```
bash
yarn test
```
