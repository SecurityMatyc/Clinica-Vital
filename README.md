# Clínica Vital Service 📚

Proyecto académico desarrollado en 2026 para la **Evaluación 2 de Backend**.  
Este sistema representa una aplicación web de gestión clínica enfocada en el registro y administración de información médica básica.

## 👥 Autor

**Matías Gajardo**

Este proyecto fue realizado **individualmente** como parte del proceso de aprendizaje en desarrollo backend con Django.

## 🧩 Descripción del proyecto

Clínica Vital es un proyecto académico **funcional, pero muy básico**, creado en una etapa inicial de aprendizaje para practicar:

- Modelado de datos relacionales en Django.
- Operaciones CRUD con formularios y vistas.
- Exposición de endpoints con Django REST Framework.
- Navegación por plantillas HTML.

El sistema permite gestionar las entidades principales de un flujo médico simple:

- Especialidades médicas.
- Médicos.
- Pacientes.
- Consultas médicas.
- Tratamientos.
- Medicamentos.
- Recetas médicas.

También incluye documentación automática de API con Swagger y ReDoc.

## ✨ Características principales

- CRUD completo en interfaz web para las entidades del sistema.
- Formularios basados en `ModelForm` para crear y editar registros.
- Vistas basadas en funciones (FBV) para listado, creación, edición y eliminación.
- API REST por entidad con `ModelViewSet` y `DefaultRouter`.
- Documentación de API disponible en Swagger (`/swagger/`) y ReDoc (`/redoc/`).
- Estructura simple y clara, adecuada para aprendizaje.

## 🛠️ Stack tecnológico

- Python 3.13
- Django 6.0.3
- Django REST Framework
- drf-yasg (Swagger/ReDoc)
- HTML, CSS y plantillas Django
- SQLite (base de datos por defecto de este repositorio)
- PostgreSQL (motor utilizado en una fase previa del proyecto)

## 🗂️ Estructura del proyecto

- `clinica_vital`: configuración principal del proyecto (settings, urls, wsgi, asgi).
- `gestion`: app principal con modelos, formularios, vistas, serializers y rutas.
- `gestion/templates/gestion`: plantillas para menú y vistas CRUD.

## 🚀 Puesta en marcha local

### 1. Clonar el repositorio

```powershell
git clone <url-del-repositorio>
cd Clinica-Vital
```

### 2. Crear y activar entorno virtual (Windows PowerShell)

```powershell
python -m venv env
.\env\Scripts\Activate.ps1
```

### 3. Instalar dependencias

```powershell
pip install -r requirements.txt
```

### 4. Aplicar migraciones

```powershell
python manage.py migrate
```

### 5. Iniciar servidor

```powershell
python manage.py runserver
```

## 🌐 Rutas útiles

- `http://127.0.0.1:8000/` Menú principal de la aplicación.
- `http://127.0.0.1:8000/admin/` Panel de administración Django.
- `http://127.0.0.1:8000/gestion/api/` Endpoints REST.
- `http://127.0.0.1:8000/swagger/` Documentación Swagger.
- `http://127.0.0.1:8000/redoc/` Documentación ReDoc.

## ☁️ Despliegue y base de datos

Durante el desarrollo se trabajó con PostgreSQL en una etapa previa.  
Para facilitar la ejecución local y la revisión académica, esta versión del repositorio utiliza **SQLite por defecto**, de modo que puedas probarla rápido y sin configuraciones externas.

## 🎯 Contexto académico

Este repositorio conserva una entrega de formación enfocada en backend con Django.  
El objetivo principal fue aprender fundamentos de desarrollo web, organización de una app MVC de Django y consumo básico de API REST.

## 📌 Resumen

Clínica Vital es una base académica funcional para gestionar datos clínicos esenciales.  
Es un proyecto **simple y básico**, construido por **Matías Gajardo** en etapa de aprendizaje, y pensado como referencia de progreso en backend.
