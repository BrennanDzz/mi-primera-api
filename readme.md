# 🎵 Albums API

[🇪🇸 Español](#español) | [🇬🇧 English](#english)

---

<a name="español"></a>

## 🇪🇸 Español

### 📖 Descripción

Pequeña API REST desarrollada con **FastAPI** para gestionar una colección de álbumes musicales.

La API permite consultar, añadir, modificar y eliminar álbumes. Los datos se almacenan en un archivo `albums.json`, por lo que no es necesario utilizar una base de datos.

### 🚀 Tecnologías utilizadas

- Python
- FastAPI
- Pydantic
- JSON
- Uvicorn

### 📁 Estructura del proyecto

```text
.
├── main.py
├── albums.json
├── requirements.txt
└── README.md
```

### ⚙️ Instalación

1. Clona el repositorio:

```bash
git clone <URL_DEL_REPOSITORIO>
```

2. Accede a la carpeta del proyecto:

```bash
cd <NOMBRE_DEL_REPOSITORIO>
```

3. Instala las dependencias:

```bash
pip install -r requirements.txt
```

### ▶️ Ejecutar la API

Puedes iniciar el servidor con:

```bash
fastapi dev main.py
```

Una vez iniciado, la API estará disponible normalmente en:

```text
http://127.0.0.1:8000
```

### 📚 Documentación

FastAPI genera automáticamente una documentación interactiva mediante Swagger UI.

Puedes acceder a ella desde:

```text
http://127.0.0.1:8000/docs
```

También está disponible la documentación alternativa de ReDoc:

```text
http://127.0.0.1:8000/redoc
```

### 🔗 Endpoints

| Método | Endpoint | Descripción |
|---|---|---|
| GET | `/` | Comprueba que la API funciona |
| GET | `/albums` | Obtiene todos los álbumes |
| GET | `/albums/{id}` | Obtiene un álbum por su ID |
| POST | `/albums` | Añade un nuevo álbum |
| PUT | `/albums/{id}` | Modifica un álbum |
| DELETE | `/albums/{id}` | Elimina un álbum |

### 📝 Ejemplo de álbum

Para crear un álbum mediante `POST /albums`:

```json
{
  "titulo": "Born to Die",
  "artista": "Lana Del Rey",
  "anio": 2012
}
```

La API genera automáticamente el `id` del nuevo álbum.

### 🎯 Objetivo

Este proyecto ha sido realizado como práctica para aprender a crear una **API REST con FastAPI**, trabajando con:

- Rutas y endpoints.
- Métodos HTTP.
- Parámetros de ruta.
- Modelos con Pydantic.
- Códigos de estado HTTP.
- Manejo de errores mediante `HTTPException`.
- Lectura y escritura de archivos JSON.
- Operaciones CRUD.

---

<a name="english"></a>

## 🇬🇧 English

### 📖 Description

Small REST API developed with **FastAPI** to manage a collection of music albums.

The API allows users to retrieve, add, update and delete albums. The data is stored in an `albums.json` file, so no database is required.

### 🚀 Technologies Used

- Python
- FastAPI
- Pydantic
- JSON
- Uvicorn

### 📁 Project Structure

```text
.
├── main.py
├── albums.json
├── requirements.txt
└── README.md
```

### ⚙️ Installation

1. Clone the repository:

```bash
git clone <REPOSITORY_URL>
```

2. Navigate to the project folder:

```bash
cd <REPOSITORY_NAME>
```

3. Install the dependencies:

```bash
pip install -r requirements.txt
```

### ▶️ Running the API

Start the development server with:

```bash
fastapi dev main.py
```

Once started, the API will normally be available at:

```text
http://127.0.0.1:8000
```

### 📚 Documentation

FastAPI automatically generates interactive API documentation using Swagger UI.

You can access it at:

```text
http://127.0.0.1:8000/docs
```

An alternative documentation interface is also available through ReDoc:

```text
http://127.0.0.1:8000/redoc
```

### 🔗 Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/` | Checks that the API is running |
| GET | `/albums` | Returns all albums |
| GET | `/albums/{id}` | Returns an album by ID |
| POST | `/albums` | Adds a new album |
| PUT | `/albums/{id}` | Updates an album |
| DELETE | `/albums/{id}` | Deletes an album |

### 📝 Album Example

To create an album using `POST /albums`:

```json
{
  "titulo": "Born to Die",
  "artista": "Lana Del Rey",
  "anio": 2012
}
```

The API automatically generates the `id` for the new album.

### 🎯 Objective

This project was created as a practice exercise to learn how to build a **REST API with FastAPI**, working with:

- Routes and endpoints.
- HTTP methods.
- Path parameters.
- Pydantic models.
- HTTP status codes.
- Error handling with `HTTPException`.
- Reading and writing JSON files.
- CRUD operations.

---