# Proyecto Django: Home & About

Este es un proyecto básico en Django que muestra una página de inicio ("home") y una página "about".

## Estructura del Proyecto

- **django_base/**: Configuración principal del proyecto Django.
- **pages/**: Aplicación Django que contiene las vistas y rutas para las páginas.
- **templates/**: Plantillas HTML para las páginas.
- **db.sqlite3**: Base de datos SQLite por defecto.

## Instalación

1. Clona este repositorio.
2. Instala las dependencias:
   ```sh
   pip install -r requierenst.txt
   ```
3. Ejecuta las migraciones:
   ```sh
   python manage.py migrate
   ```
4. Inicia el servidor de desarrollo:
   ```sh
   python manage.py runserver
   ```

## Uso

- Accede a la página principal en `http://localhost:8000/`
- Accede a la página "about" en `http://localhost:8000/about/`

## Archivos principales

- [`pages/views.py`](pages/views.py): Define las vistas [`pages.views.HomePageView`](pages/views.py) y [`pages.views.AboutPageView`](pages/views.py).
- [`pages/urls.py`](pages/urls.py): Define las rutas de la app.
- [`django_base/urls.py`](django_base/urls.py): Incluye las rutas de la app principal.
- [`templates/home.html`](templates/home.html) y [`templates/about.html`](templates/about.html): Plantillas de las páginas.
- [`templates/_base.html`](templates/_base.html): Plantilla base para heredar estructura común.

## Notas

- No hay modelos personalizados ni lógica avanzada.
- El proyecto está listo para expandirse con nuevas páginas