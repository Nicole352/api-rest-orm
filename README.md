#api-rest-orm##

Esta es una API REST desarrollada en **Node.js** con **Express** y **MongoDB** que permite realizar operaciones CRUD sobre usuarios. Incluye autenticación segura mediante **JWT** y almacenamiento de contraseñas encriptadas con **bcrypt**.

> ✅ Esta rama contiene **solo el backend**, ideal para integraciones con frontend o apps móviles.

---

## 🚀 Características principales

- CRUD completo de usuarios
- Autenticación mediante email y contraseña
- Encriptación de contraseñas usando `bcrypt`
- Generación de tokens JWT válidos por 1 hora
- Conexión segura con MongoDB vía Docker
- Panel visual de base de datos con mongo-express 


## 📁 Estructura del proyecto

├── src/
│ ├── controllers/ # Lógica de negocio (endpoints)
│ ├── models/ # Modelo Mongoose (User)
│ ├── routes/ # Definición de rutas REST
├── index.js # Archivo principal del servidor
├── .env # Variables de entorno
├── docker-compose.yml # Define MongoDB + mongo-express
└── package.json


## 🧪 Requisitos

- Node.js >= 18
- Docker y Docker Compose
- Postman (Para pruebas)


## ⚙️ Instalación y ejecución

### Clonar el repositorio y entrar al proyecto

https://github.com/Nicole352/api-rest-orm.git

**Iniciar base de datos con Docker**

docker-compose up -d
Esto levantará: MongoDB en localhost:27017
mongo-express en http://localhost:8081

**Instalar dependencias y ejecutar el backend**

npm install
npm start
El servidor estará activo en http://localhost:8080

##Endpoints 
##
Método	            Endpoint	             Descripción
POST	              /api/users	           Crear usuario
GET	                /api/users	           Listar usuarios
GET	                /api/users/:id	       Obtener un usuario
PUT	                /api/users/:id	       Actualizar usuario
DELETE	            /api/users/:id	       Eliminar usuario
POST	              /api/login	           Iniciar sesión (login)

Autora
Nicole Jamilex Díaz Valdez
GitHub: @Nicole352
