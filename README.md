<div align="center">
  <img src="https://github.com/8ByteSword/padelHubTournament2Electricboogaloo/assets/72978286/677ca6e7-f874-4da4-80b8-8de480bf64a1" width="200px">
</div>

# Club de Pádel - Gestión de Reservas y Torneos

Este proyecto es una aplicación web para la gestión de reservas, torneos, ligas y partidas en un club de pádel. Está construido con un frontend en Svelte, utilizando Tailwind CSS para los estilos, y un backend en Python con FastAPI. La comunicación en tiempo real se realiza a través de WebSockets (integrados en FastAPI) o Socket.IO. La base de datos utilizada es PostgreSQL.

## Funcionalidades base

- Gestión de reservas de pistas
- Gestión de torneos (inscripción, generación de cuadros, asignación de enfrentamientos)
- Gestión de ligas (creación, calendario, clasificación)
- Gestión de partidas (registro de resultados, cálculo de enfrentamientos pendientes)
- Asignación automática de enfrentamientos
- Notificaciones automáticas vía WhatsApp (opcional)

## Arquitectura

La aplicación sigue una arquitectura cliente-servidor, donde el frontend en Svelte se encarga de la interfaz de usuario y la interacción con el usuario, mientras que el backend en FastAPI proporciona una API RESTful para la gestión de datos y la lógica de negocio. La comunicación en tiempo real se realiza a través de WebSockets o Socket.IO para actualizar la información en tiempo real. La base de datos PostgreSQL almacena los datos de reservas, torneos, ligas y partidas.

## Configuración del entorno de desarrollo

### Requisitos previos

- Node.js y npm
- Python y pip
- PostgreSQL

### Pasos de configuración

1. Clona el repositorio: `git clone https://github.com/tu-usuario/club-padel.git`
2. Instala las dependencias del frontend: `cd frontend && npm install`
3. Instala las dependencias del backend: `cd ../backend && pip install -r requirements.txt`
4. Configura la base de datos PostgreSQL (crea una base de datos y actualiza la configuración en `backend/settings.py`)

## Instalación y ejecución

1. Clona el repositorio: `git clone https://github.com/tu-usuario/club-padel.git`
2. Instala las dependencias del frontend: `cd frontend && npm install`
3. Instala las dependencias del backend: `cd ../backend && pip install -r requirements.txt`
4. Configura la base de datos PostgreSQL (crea una base de datos y actualiza la configuración en `backend/settings.py`)
5. Inicia el servidor de desarrollo del frontend: `cd ../frontend && npm run dev`
6. Inicia el servidor de desarrollo del backend: `cd ../backend && uvicorn main:app --reload`

La aplicación estará disponible en `http://localhost:5173` (frontend) y `http://localhost:8000` (backend).

## Estructura del proyecto
club-padel/
├── frontend/
│ ├── src/
│ │ ├── components/
│ │ ├── routes/
│ │ ├── stores/
│ │ ├── utils/
│ │ ├── App.svelte
│ │ ├── main.js
│ │ └── ...
│ ├── static/
│ ├── package.json
│ └── ...
├── backend/
│ ├── app/
│ │ ├── api/
│ │ ├── models/
│ │ ├── schemas/
│ │ ├── utils/
│ │ └── ...
│ ├── tests/
│ ├── main.py
│ ├── requirements.txt
│ └── ...
└── ...


- `frontend/`: Contiene el código fuente del frontend en Svelte, incluyendo componentes, rutas, stores y utilidades.
- `backend/`: Contiene el código fuente del backend en FastAPI, incluyendo modelos, esquemas, APIs y utilidades.

## Contribución

Si deseas contribuir a este proyecto, por favor sigue estos pasos:

1. Haz un fork del repositorio
2. Crea una rama para tu nueva funcionalidad: `git checkout -b nueva-funcionalidad`
3. Realiza tus cambios y haz commit: `git commit -am 'Agrega nueva funcionalidad'`
4. Envía tus cambios al repositorio remoto: `git push origin nueva-funcionalidad`
5. Crea una nueva solicitud de extracción en GitHub

## Licencia

Este proyecto está licenciado bajo la [Licencia MIT](LICENSE).

## Contacto

Si tienes alguna pregunta o sugerencia, no dudes en ponerte en contacto con nosotros:

- Desarrollador principal: [tu-nombre@ejemplo.com](mailto:tu-nombre@ejemplo.com)
- Equipo de desarrollo: [equipo@ejemplo.com](mailto:equipo@ejemplo.com)

## Enlaces útiles

- [Documentación oficial de Svelte](https://svelte.dev/docs)
- [Documentación oficial de Tailwind CSS](https://tailwindcss.com/docs)
- [Documentación oficial de Python](https://docs.python.org/3/)
- [Documentación oficial de FastAPI](https://fastapi.tiangolo.com/docs/)
- [Documentación oficial de PostgreSQL](https://www.postgresql.org/docs/)
- [Documentación oficial de WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) o [Documentación oficial de Socket.IO](https://socket.io/docs/v4/)
- [Documentación oficial de WhatsApp Business API](https://developers.facebook.com/docs/whatsapp/api/) (para las notificaciones automáticas)

## TODOs iniciales

1. Configurar el entorno de desarrollo
   - Instalar Node.js, npm, Python, pip y PostgreSQL
   - Clonar el repositorio

2. Crear la estructura básica del proyecto
   - Configurar la estructura de directorios para el frontend y backend
   - Inicializar los proyectos de Svelte y FastAPI

3. Implementar el enrutamiento básico en el frontend
   - Configurar el enrutador de Svelte
   - Crear rutas iniciales (inicio, reservas, torneos, ligas)

4. Crear un diseño de interfaz de usuario inicial utilizando Tailwind CSS
   - Definir la paleta de colores y estilos base
   - Crear componentes reutilizables (navbar, footer, botones, etc.)

5. Configurar la conexión a la base de datos en el backend
   - Instalar y configurar SQLAlchemy
   - Definir la cadena de conexión a PostgreSQL

6. Crear modelos y esquemas de base de datos iniciales
   - Definir modelos para reservas, torneos, ligas y partidas
   - Crear esquemas de Pydantic correspondientes

7. Implementar endpoints de API básicos para las funcionalidades principales
   - Crear rutas de API para CRUD de reservas, torneos, ligas y partidas
   - Implementar la lógica de negocio en los controladores

8. Integrar WebSockets o Socket.IO para la comunicación en tiempo real
   - Configurar WebSockets en FastAPI o instalar Socket.IO
   - Implementar la comunicación en tiempo real para actualizar información

9. Crear un mockup de interfaz de usuario con un ejemplo de demo
   - Diseñar mockups de las principales vistas de la aplicación
   - Implementar una vista de demo con datos de prueba
 
