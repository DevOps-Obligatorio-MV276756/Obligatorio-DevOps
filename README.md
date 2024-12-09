
<p align = "center">
<img src = "images/ORT.png" width=100%>
</p>

---

# Universidad ORT Uruguay | Facultad de ingeniería | Escuela de tecnología - DevOps | Obligatorio

## Documento Readme Obligatorio

### Mauro Veloso 276756

# Indice

1

2

3

4

5

# Estructura

# Presentacion del problema

Lorem ipsum

# Solucion Planteada

A continuación se detalla la solución presentada.

## Herramientas y Proveedores

Como herramientas a utlizar se seleccionaron las siguientes:

**Herramienta de Git**: GitHub

**Herramienta de CI/CD**: GitHub Actions

**Orquestador**: AWS ECS

**Proveedor de Cloud**: AWS

**Herramienta de Testing de Código Estático**: SonarCloud

**Herramienta de Prueba extra**: Postman

**Aplicación FE a buildear y desplegar**: Vue

**Servicio Serverless**: S3 Bucket

## Tablero Kanban

Se maneja un tablero kanban para documentar el trayecto continuo del proyecto.

### Presentación visual

<p align = "center">
<img src = "images/kanban_example.png" width=100%>
</p>

## Repositorios

Se decide diseñar una estructura de 6 repositorios. Cuatro repositorios para almacenar los microservicios, uno para el FrontEnd y uno para todo lo orientado a DevOps.

### Repositorio DevOps

Para el manejo del repositorio de DevOps se va a utilizar un flujo Trunk based. Se toma la decisión con la consideración de que se apunta a manejar Feature branches de corta vida con pequeñas modificaciónes y no se apunta a mantener otras branches con copias del código, permitiendo evitar problemas al realizar el merge. Manteniendo un ecosistema limpio y pronto para buildear en el momento oportuno.

#### Diagrama de flujo

<p align = "center">
<img src = "https://softwareskill.pl/wp-content/uploads/2022/06/trunk-based-development-release-branch-e1656332842126-1024x478.png" width=100%>
</p>

### Repositorios de MicroServicios y Frontend

Para los repositorios donde se hospedarán los MicroServicios y el repositorio del FrontEnd se decide por el uso del flujo GitFlow. Permitiendo mantener una rama estable para cada ambiente manejado (prod/main, dev, test), con su respectiva lógica de CI/CD.
En este caso se decide utilizar tres ramas estables. Main, que actua como la rama donde se almacena el código desplegable en producción. Dev, donde se almacena el código desplegable en el ambiente de desarrollo. Y por último, Test, donde se almacena el código desplegable en el ambiente de testing.

#### Diagrama de flujo

<p align = "center">
<img src = "images/gitflow.png" width=100%>
</p>

## CI/CD

### Análisis de código estático

Para el análisis de código estático se decide hacer uso de SonarCloud.

### Build

#### MicroSevices

#### FrontEnd

### Análisis de servicios

### Deploy
