# "Aplicación web de microblogging con MERN" (Back-end)

API REST del proyecto "Aplicación web de microblogging con MERN", creada con NodeJS y ExpressJS. Con conexión a base de datos MongoDB a través de MongoDB Atlas

## Comenzando 🚀

_Estas instrucciones te permitirán obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas._

### Pre-requisitos 📋

Se requiere la instalación de node y el gestor de paquetes npm. Es necesario tener una base de datos MongoDB desplegada (por ejemplo, en [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)).

### Instalación 🔧

_Instrucciones para la ejecución de la API REST en local:_

Se necesitarán instalar las dependencias del proyecto y setear las siguientes variables de entorno (o bien crear un fichero ".env" con las mismas):

| Variable | Valor |
| ------------- | ------------- |
| NODE_ENV  | development  |
| PORT  | 5000  |
| DB_URI  | 'Cadena de conexión a la BBDD'  |

Instalación de dependencias:

```
npm install
```

Ejecución de la API REST:

```
npm start
```

_Una vez ejecutada, estará disponible en la URL definida (por ejemplo: "http://localhost:5000") y podremos probar sus servicios con un cliente REST._

* Solicitudes principales de la API REST para el acceso a recursos de los usuarios:

Solicitud | Ruta | Descripción |
| ------------- | ------------- | ------------- |
| GET | /users  | Devuelve todos los usuarios de la colección "users" de la BBDD  |
| GET | /users/:id  | Devuelve el usuario especificado por su Id.  |
| POST | /users  | Añade un nuevo usuario a la colección "users" (en un documento JSON)  |
| PUT | /users/:id  | Actualiza el usuario especificado por su Id, con la información JSON recibida  |
| DELETE | /users/:id  | Elimina el usuario especificado por su Id.  |
| POST | users/signin  | Comprueba la existencia del usuario en la colección "users", con la información JSON recibida  |

* Solicitudes principales de la API REST para el acceso a recursos de los posts:

Solicitud | Ruta | Descripción |
| ------------- | ------------- | ------------- |
| GET | /posts  | Devuelve todos los posts de la colección "posts" de la BBDD  |
| GET | /posts/all/:id  | Devuelve todos los post de un usuario especificado por su Id.  |
| POST | /posts  | Añade un nuevo post a la colección "posts" (en un documento JSON)  |
| PUT | /posts/:id  | Actualiza el post especificado por su Id, con la información JSON recibida  |
| DELETE | /posts/:id  | Elimina el post especificado por su Id.  |

## Despliegue en heroku 📦

_Adicionalmente puedes desplegar la API REST en la plataforma [Heroku](https://heroku.com/)._

Para ello, podrás crear una aplicación en Heroku y conectarla al repositorio Github dónde tengas alojada esta API REST.

## Construido con 🛠️

_Esste proyecto ha sido creado con:_

* [MongoDB](https://www.mongodb.com/) - Sistema gestor de BBDD
* [NodeJS](https://nodejs.org/es/) - Entorno de ejecución Node
* [ExpressJS](https://expressjs.com/es/) - Framework para el enrutado

## Más información 📖

Puedes encontrar más información del proyecto en [Desarrollo web full-stack con MERN](https://jesusfontecha.name/mern/)

📢 _También se ha desarrollado una aplicación web con ReactJS capaz de consumir esta API REST.
Accesible en:_
* [Aplicación web con React](https://github.com/jfontecha/microblogging-example-react-classes)
* [Aplicación web con React hooks](https://github.com/jfontecha/microblogging-example-react-hooks)

## Autores ✒️

_Proyecto desarrollado por:_

* **Jesús Fontecha** - [jfontecha](https://github.com/jfontecha)

## Licencia 📄

Este proyecto es _opensource_ y se ha desarrollado con fines exclusivamente académicos. Si lo descargas, al menos menciona al autor 🤓🍺.

---
_Made with love for a smarter world_ ❤️
