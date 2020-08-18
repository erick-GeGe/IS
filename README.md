# OnlineDoc Web

Pagina que ayuda a estar al danto de tu salud para que puedas vivir de manera feliz xd

## Comenzando 🚀

Para iniciar puedes descargar el proyecto y ubicarlo en una carpeta de tu preferencia, solo necesitas descomprimirlo, nada mas.     

### Pre-requisitos 📋

Tecnologia usadas en el proyecto

```
Python3
Pip
Django
Postgres
```

## Construido con 🛠️

* [django](https://www.djangoproject.com/) - El framework web usado
* [postgres](https://www.postgresql.org/) - Base de datos

## Estilos de programacion ⌨️

Los estilos de programacion usados son los siguientes:

### Things

### Trinity

#### Modelo 
Almacenamiento de datos
```
# Fragmento de archivo models

from django.db import models

class Persona(models.Model):
    dni = models.CharField(max_length=8, primary_key=True, null=False)
    nombre = models.CharField(max_length=20, null=False)
    apellido_paterno = models.CharField(max_length=20, null=False)
    apellido_materno = models.CharField(max_length=20, null=False)
    celular = models.CharField(max_length=9, null=False)
```

#### Controlador
Control de los datos

```
from farmaciaApp.models import Personsa

personas = Persona.objects.all()
```

#### Vista Template
La vista decide que informacion vamos a mostrar y en que template

```
#Archivo views

from django.shortcuts import render, HttpResponse

def home(reques):
    return render(reques,"home.html")

def emergencia_medica(reques):
    return render(reques,"emergencia_medica.html")

def reservar_cita(reques):
    return render(reques,"reservar_cita.html")

def recibir_atencion_medica(reques):
    return render(reques,"recibir_atencion_medica.html")

def recibir_receta(reques):
    return render(reques,"recibir_receta.html")

def solicitar_atencion_fisica(reques):
    return render(reques,"solicitar_atencion_fisica.html")


```



### Nose

## Principios SOLID usados

## Principios DDD
