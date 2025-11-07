# 🐮 Animal Farm - Node.js Project

Este proyecto es una pequeña aplicación **Node.js** basada en **Express**, que genera respuestas tanto en formato HTML como JSON relacionadas con animales y sus sonidos.  
Está inspirada en la canción “Old MacDonald had a farm”, adaptada en tono humorístico con “George Orwell had a farm”.

---

## 🚀 Estructura del proyecto

```
.
├── app.js               # Servidor principal Express
├── package.json         # Dependencias y scripts
├── test.js              # Pruebas automatizadas con Mocha y Supertest
├── Dockerfile           # Configuración para ejecutar la app en un contenedor
```

---

## ⚙️ Instalación

Instale yarn

```bash
npm install --global yarn
```

Clona el repositorio y ejecuta los siguientes comandos:

```bash
yarn install
```

---

## ▶️ Ejecución

Para iniciar el servidor en modo local:

```bash
yarn start
```

El servidor se lanzará en [http://localhost:8080](http://localhost:8080)

---

## 🧪 Tests

Ejecuta las pruebas automatizadas con:

```bash
npm test
```

---

## 🐳 Ejecución con Docker

Para construir la imagen Docker:

```bash
docker build -t animal-farm .
```

Para ejecutar el contenedor:

```bash
docker run -p 8080:8080 animal-farm
```

---

## 📡 Endpoints principales

| Ruta | Descripción | Formato |
|------|--------------|---------|
| `/` | Devuelve una página HTML con un animal aleatorio y su sonido | text/html |
| `/api` | Devuelve un objeto JSON con todos los animales y sus sonidos | application/json |

---

## 🧩 Dependencias principales

- [Express](https://expressjs.com/) - Framework de servidor web
- [Underscore.js](https://underscorejs.org/) - Utilidades funcionales
- [Mocha](https://mochajs.org/) y [Supertest](https://github.com/visionmedia/supertest) - Pruebas automatizadas
- [NYC](https://github.com/istanbuljs/nyc) - Cobertura de código

---

## 📄 Licencia

Este proyecto está licenciado bajo la **MIT License**.
<!-- Comentario para activar el workflow-->