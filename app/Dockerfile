FROM python:3.12
LABEL org.opencontainers.image.authors="daniel.gonzalezp@edu.uah.es"

# Declaramos la carpeta de trabajo
WORKDIR /app

# Copiamos el archivo requirements.txt dentro de la imagen del contenedor. 
# El contenido de este archivo se explica más adelante
COPY requirements.txt /app

# Instalamos las dependencias dentro de la imagen
RUN pip install -r requirements.txt

# Copiamos la aplicación web dentro de la imagen
COPY . /app

# Puerto en el que escuchará el contenedor
EXPOSE 8080

ENTRYPOINT ["python", "main.py"]
