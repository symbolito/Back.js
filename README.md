# Back.js
Backend en Node.js + Express conectado a una base de datos PostgreSQL en AWS, que gestiona tareas mediante una API REST.
## 🚀 Tecnologías Utilizadas
- Node.js  
- Express  
- PostgreSQL  
- AWS RDS  
- DBeaver (cliente de conexión)  
- dotenv para variables de entorno  

---

## 📦 Instalación y Configuración

### 1️⃣ Clonar el repositorio
```bash
git clone https://github.com/tu-usuario/task-manager-backend.git
cd task-manager-backend
```
2️⃣ Instalar dependencias
```bash
npm install
```
3️⃣ Crear archivo .env
En la raíz del proyecto crear:

```
Copiar código
DB_HOST=tu-host-de-rds.amazonaws.com
DB_USER=postgres
DB_PASSWORD=tu-password
DB_NAME=tareasdb
PORT=8000
```

🔌 Endpoints de la API
✔️ Obtener todas las tareas

GET /tareas

➕ Crear nueva tarea

POST /tareas

{
  "texto": "Estudiar bases de datos",
  "fecha": "2025-01-10"
}

✏️ Editar tarea

PUT /tareas/:id

🗑️ Eliminar tarea

DELETE /tareas/:id


Despliegue en AWS EC2

El proyecto está configurado para funcionar en una instancia EC2 y conectarse a PostgreSQL en AWS RDS.

Pasos generales:

Instalar Node.js en EC2

Subir este proyecto

Configurar variables de entorno

Permitir tráfico al puerto 8000 en el Security Group

Ejecutar con npm start o PM2
