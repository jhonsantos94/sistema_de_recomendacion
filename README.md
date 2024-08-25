#  Sistema de Recomendación

# Programacion Web Avanzada - 14567

## Grupo #2
- Javier Gonzaga
- Jhon Munarco
- Francisco Terán


# Sistema de recomendacion de peliculas

## Descripción del Proyecto

Este proyecto implementa un sistema de recomendación de películas basado en contenido, desarrollado con Flask y utilizando datos de Peliculas.

## Descripción

La aplicación permite a los usuarios ingresar el nombre de una película y recibir recomendaciones de películas similares, basadas en varias características textuales, como título, director, elenco, géneros y descripción.

## Estructura del Proyecto
- app.py: Archivo principal de la aplicación Flask que gestiona la lógica de recomendación y las rutas.
- templates/: Directorio que contiene las plantillas HTML (index.html y result.html).
- static/stylesheets/: Carpeta que almacena los archivos CSS (style.css y result.css).
- peliculas.csv: Archivo CSV que contiene la información de las películas y programas de TV disponibles.

## Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/jhonsantos94/sistema_de_recomendacion.git

2. Crea un entorno virtual e instala las dependencias necesarias:

python -m venv venv
venv\Scripts\activate  # En Windows

pip install -r requirements.txt

3. Asegúrate de que el archivo peliculas.csv esté en el directorio raíz del proyecto.

4. Ejecuta la aplicación:
python app.py

Luego, abre tu navegador y dirígete a: http://127.0.0.1:5000/

### Uso
- Abre la aplicación en tu navegador.
- Introduce el nombre de una película en el campo de texto.
- Haz clic en "Enviar" para obtener recomendaciones.


### Detalles de los Archivos CSS
- style.css: Contiene los estilos para la página principal (index.html).
- result.css: Incluye los estilos para la página de resultados (result.html).



## Uso de la Aplicación

- Detalles de los Archivos HTML
- index.html: Página principal donde los usuarios pueden ingresar el nombre de una película.
- result.html: Página de resultados que muestra las recomendaciones de películas basadas en la entrada del usuario.

## Tecnologías Utilizadas

- Flask

## Código Principal (app.py)
- Limpieza de Datos: Se procesan los datos eliminando espacios y estandarizando el texto a minúsculas.
- Creación de la "Sopa" de Palabras: Se combinan varias características textuales de cada película para formar un único descriptor.
- Vectorización de Texto: Se utiliza CountVectorizer para transformar la "sopa" de palabras en una matriz de conteo.
- Cálculo de Similitud: Se emplea la similitud del coseno para medir qué tan parecidas son las películas.
- Generación de Recomendaciones: Se obtienen las películas más similares basadas en la similitud del coseno calculada.
