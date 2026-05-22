# 🛒 Ecommerce API

¡Bienvenido a **Ecommerce API**! Una API REST robusta y escalable diseñada para gestionar un sistema de comercio electrónico, construida con **FastAPI** y **PostgreSQL**, y completamente empaquetada con **Docker** para un despliegue ágil en cualquier entorno.

El proyecto cuenta con arquitectura limpia, validación de datos estricta y un sistema seguro de autenticación por tokens.

---

## 🛠️ Tecnologías Utilizadas

* **Framework principal:** Python 3.11 & FastAPI
* **Base de datos:** PostgreSQL
* **ORM:** SQLAlchemy (para el mapeo de datos)
* **Validación de datos:** Pydantic V2
* **Seguridad:** Autenticación mediante tokens JWT (JSON Web Tokens)
* **Contenedores:** Docker & Docker-slim (optimizado para producción)
* **Servidor ASGI:** Uvicorn
* **Pruebas:** Pytest (en la carpeta `/test`)

---

## 🔒 Variables de Entorno y Seguridad

El proyecto utiliza un archivo `.env` local para gestionar de manera segura las credenciales y configuraciones sensibles. Este archivo está blindado mediante `.gitignore` y **nunca** se sube al repositorio público.

Para que la API funcione, se debe crear un archivo llamado `.env` en la raíz con la siguiente estructura:

```env
DATABASE_URL=postgresql://usuario:password@localhost:5432/ecommerce_db
SECRET_KEY=tu-clave-secreta-super-segura
