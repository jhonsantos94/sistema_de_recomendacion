#  Proyecto 3er Parcial

# Programacion Web Avanzada - 14567

## Grupo #2
- Javier Gonzaga
- Jhon Munarco
- Francisco Terán


# Sistema de gestion de clinica dental GAP-Dental

## Descripción del Proyecto

Este proyecto implementa un sistema de gestión de un centro odontologico el cual permite gestionar usuarios ya sean paciente o medicos, agendar citas por horario y fecha, mostrar mensajes de futuras citas.

## Descripción

La aplicación permite ser administrada por un solo usuario administrador el cual gestiona la creacion de usuarios con sus respectivos roles y estados, tambien de agregar o elimininar citas en el calendario.

## Estructura del Proyecto

Este proyecto combina una aplicación Django con un frontend desarrollado en Next.js. A continuación, se proporcionan instrucciones para configurar y ejecutar ambas partes del proyecto.

## Requisitos Previos

- Python 3.x
- Node.js
- pip (gestor de paquetes de Python)
- Virtualenv (opcional pero recomendado)

## Configuración del Backend (Django)

1. Clona este repositorio en tu máquina local:

## Instalación

1. Clona el repositorio:
   
   git clone https://github.com/JaviGonzaga27/Next_Django.git

2. Crea y activa un entorno virtual:

python -m venv venv
source venv/bin/activate  # En Windows usa `venv\Scripts\activate`

3. Instala las dependencias de Python:

pip install -r requirements.txt


4. Realiza las migraciones de la base de datos:
python manage.py migrate

5. Ejecuta el servidor de desarrollo de Django:
python manage.py runserver

El servidor estará disponible en http://localhost:8000



## Configuración del Frontend (Next.js)

1. Navega al directorio del frontend:
cd frontend

2. Instala las dependencias de Node.js:
npm install

3. Ejecuta el servidor de desarrollo de Next.js:
npm run dev

El servidor estará disponible en http://localhost:3000.


### Despliegue
Despliegue en Vercel
La manera más fácil de desplegar la aplicación de Next.js es utilizando la plataforma Vercel, creada por los desarrolladores de Next.js. Consulta la documentación de despliegue para más detalles.

### Despliegue de Django
Para desplegar la aplicación Django, puedes utilizar servicios como Heroku, AWS, o cualquier servidor con soporte para WSGI. Asegúrate de configurar correctamente el archivo settings.py para producción.


## Tecnologías Utilizadas

1. Backend - Django:

- Python: El backend está construido sobre Django, un framework web en Python.
- Django: Framework web de alto nivel para crear aplicaciones web rápidas y seguras.
- Virtualenv: Utilizado para aislar el entorno de desarrollo de Python, manejando las dependencias de forma independiente.


2. Frontend - Next.js:

- Next.js: Un framework de React para la creación de aplicaciones web estáticas y dinámicas.
- React: Biblioteca de JavaScript para construir interfaces de usuario.
- Node.js: Entorno de ejecución de JavaScript utilizado para ejecutar scripts de desarrollo y gestión de paquetes.
- npm/yarn/pnpm: Gestores de paquetes utilizados para instalar dependencias del frontend.


3. Dependencias adicionales:

- Django: Probablemente se incluyen bibliotecas y middleware adicionales en requirements.txt.
- Paquetes de Node.js: Dependencias definidas en el archivo package.json que incluyen bibliotecas necesarias para el desarrollo con Next.js y React.



## Descripción técnica del Proyecto:

Este proyecto es una aplicación web que combina un backend desarrollado con Django y un frontend moderno construido con Next.js. Está diseñado para ofrecer una solución completa donde Django maneja la lógica del servidor, la gestión de la base de datos y la API, mientras que Next.js proporciona una interfaz de usuario interactiva y eficiente.

### Funcionalidades Principales:
1. Gestión de Usuarios y Autenticación:

- Django gestiona la autenticación y autorización de usuarios, permitiendo que los usuarios se registren, inicien sesión, y gestionen sus perfiles.


2. API RESTful:

- El backend de Django expone una API que permite la interacción con la base de datos y otros servicios del lado del servidor. Esto incluye operaciones CRUD (Crear, Leer, Actualizar y Eliminar) para diferentes recursos manejados por la aplicación.

3. Interfaz de Usuario Dinámica:

- El frontend, construido con Next.js, ofrece una experiencia de usuario rápida y reactiva. Las páginas se cargan rápidamente gracias al renderizado del lado del servidor (SSR) y la generación de páginas estáticas (SSG) que Next.js permite.

- La interfaz está diseñada para ser intuitiva y responsiva, adaptándose a diferentes tamaños de pantalla y dispositivos.


4. Optimización y Despliegue:

- Next.js incluye características avanzadas como la optimización automática de fuentes y la carga diferida de componentes, mejorando el rendimiento de la aplicación.
- La aplicación está preparada para ser desplegada fácilmente en plataformas como Vercel para el frontend y en cualquier servidor compatible con WSGI para el backend de Django.


### Uso Típico:
Este proyecto es ideal para crear aplicaciones web que requieren una arquitectura completa y bien estructurada, como sistemas de gestión, plataformas de contenido, o cualquier aplicación donde se necesite combinar un backend robusto con un frontend moderno y eficiente.

### Licencia
Este proyecto está bajo la Licencia MIT.
