# Servicios Técnicos - Sistema de Gestión

## Descripción
Aplicación web full-stack diseñada para la administración integral de servicios técnicos, control de clientes y gestión de personal técnico en taller o campo.

## Tecnologías
- **Frontend:** React, JavaScript (ES6+), CSS3, Vite
- **Backend:** Python 3, Flask, Werkzeug, CORS
- **Base de Datos:** MySQL
- **Herramientas de Pruebas:** Thunder Client / Postman

## Requisitos Previos
- Python 3.8+ y pip
- Node.js 16+ y npm
- Servidor MySQL activo
- Git

## Configuración del Entorno Local

1. **Base de Datos:**
   - Crear la base de datos `tecnico` en MySQL.
   - Ejecutar el script SQL del proyecto para estructurar las tablas (`cliente`, `tecnico`, `servicio`, `usuario`).

2. **Variables de Entorno:**
   - Copiar el archivo `.env.example` a `.env` en el backend y completar los parámetros:
     ```env
     DB_HOST=localhost
     DB_USER=root
     DB_PASSWORD=tu_contraseña
     DB_NAME=tecnico
     FLASK_DEBUG=0
     ```

3. **Backend (Flask):**
   ```bash
   cd backend
   python -m venv venv
   # En Windows:
   venv\Scripts\activate
   # En Linux/Mac:
   source venv/bin/activate
   pip install -r requirements.txt