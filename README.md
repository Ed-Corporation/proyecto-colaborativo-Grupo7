# Proyecto Colaborativo – Gestión de Versionamiento con Git y GitHub
## Descripción
Taller de Git y GitHub, grupo 7.
El objetivo del taller es demostrar la aplicación de un flujo de trabajo colaborativo utilizando Git como sistema de control de versiones y GitHub como plataforma de colaboración y gestión del proyecto.
Durante el desarrollo del taller se implementaron diferentes herramientas y funcionalidades de GitHub, incluyendo:

Repositorios Git.
Archivos .gitignore.
Ramas de trabajo (branches).
Commits.
Issues.
GitHub Projects.
Milestones.
Asignación y seguimiento de tareas.
Pull Requests.
Revisión de código.
Merge de ramas.
Trabajo colaborativo mediante PowerShell y GitHub.

## Integrantes
Integrante	                |Rol
Edwin Santiago Ballesteros	|Colaborador
Byron Diaz                  |Colaborador 

## Repositorio

## Repositorio en GitHub:
proyecto-colaborativo-Grupo7

## Objetivos
### Objetivo general

Aplicar un flujo de trabajo colaborativo utilizando Git y GitHub para gestionar versiones, organizar actividades y controlar el desarrollo de un proyecto mediante ramas, issues, proyectos, milestones y Pull Requests.

### Objetivos específicos
Configurar un repositorio Git y su archivo .gitignore para el trabajo colaborativo.
Crear y administrar ramas independientes para los integrantes.
Utilizar GitHub Projects, Issues y Milestones para organizar y realizar seguimiento a las tareas.
Aplicar Pull Requests para la revisión de los cambios.
Integrar los avances mediante el proceso de merge.to de objetivos
Estructura del flujo de trabajo

El proyecto siguió un flujo colaborativo basado en ramas:

                    ┌─────────────────┐
                    │      main       │
                    └────────┬────────┘
                             │
             ┌───────────────┼───────────────┌──────────────┐
             │               │               │              |
             ▼               ▼               ▼              ▼
       rama-Administrativa  rama-Docentes  ramaEdwin   rama Bairon
             │               │               │              |
             ▼               ▼               ▼              ▼
          commits         commits         commits        commits
             │               │               │              |
             └───────────────┼───────────────┘──────────────┘
                             │
                             ▼
                        Pull Request
                             │
                             ▼
                         Revisión
                             │
                             ▼
                           Merge
                             │
                             ▼
                            main
## Etapas del proyecto
### Etapa 1 – Creación de archivos y .gitignore

En la primera etapa se realizó la creación de los archivos necesarios para el proyecto y la configuración del archivo .gitignore.

El .gitignore permite especificar archivos y carpetas que no deben ser incluidos en el control de versiones.

Ejemplo:

### Archivos temporales
*.tmp

### Archivos del sistema
.DS_Store
Thumbs.db

### Configuraciones locales
.env

Cada integrante trabajó con su respectiva configuración de .gitignore.

### Etapa 2 – Preparación del entorno

Se utilizó PowerShell como terminal para ejecutar los comandos de Git y administrar el repositorio local.

Comandos principales utilizados:

* git --version

Verificación de la instalación de Git.

* git config --global user.name "Nombre del usuario"
* git config --global user.email "correo@email.com"

Configuración de la identidad del usuario.

* git init

Inicialización del repositorio Git.

* git status

Consulta del estado actual del repositorio.

### Etapa 3 – Planificación y organización en GitHub

Para organizar el trabajo colaborativo se utilizaron las herramientas de planificación disponibles en GitHub.

### GitHub Projects

Se creó un Project para organizar las actividades del proyecto mediante diferentes secciones y estados.
El tablero permitió visualizar el progreso de las tareas y facilitar el seguimiento del trabajo realizado por cada integrante (simulación).

Ejemplo de flujo:
To do → In progress → Done

### Milestone

Se creó un Milestone para agrupar los Issues relacionados con el objetivo principal del taller.
Los Milestones permiten establecer un objetivo común y realizar seguimiento al avance de las actividades asociadas.

### Issues

Se crearon Issues para dividir el trabajo en tareas específicas.

Cada Issue podía contener:

- Descripción de la actividad.
- Responsable.
- Milestone asociado.
- Project asociado.
- Estado de la actividad.

El proyecto incluyó la creación y organización de Issues vinculados al Milestone y al Project.

### Asignación de tareas

Las actividades fueron distribuidas entre los integrantes del grupo mediante la asignación de responsables en GitHub. Esto permitió identificar quién debía realizar cada actividad y realizar seguimiento al avance individual.

### Etapa 4 – Trabajo mediante ramas

Cada integrante trabajó en una rama personal para evitar realizar directamente los cambios sobre main.

creación de una rama:
* git branch nombre-integrante

Cambio hacia la rama:
* git checkout nombre-integrante

Cambio de rama opcional:
* git switch nombre-integrante

Verificación de las ramas existentes:
* git branch

Commits
Después de realizar cambios en los archivos, estos fueron registrados mediante commits.

* git status
Permite verificar los archivos modificados.

* git add .
Agrega los cambios al área de preparación (staging area).

* git commit -m "Descripción del cambio"
Registra los cambios en el historial de Git.

Para el git commit se recomienda utilizar mensajes de commit claros, cortos y descriptivos.

Ejemplo:
- git commit -m "Agrega documentación inicial del proyecto"

Sincronización con GitHub
Para enviar los cambios al repositorio remoto se utilizó:
* git push origin nombre-integrante

Para actualizar la información del repositorio local:
* git pull

La conexión entre el repositorio local y GitHub permite mantener sincronizados los avances realizados por los integrantes.

### Etapa 5 – Seguimiento y control en GitHub

GitHub fue utilizado como plataforma central para realizar el seguimiento del proyecto.

Las herramientas utilizadas permitieron controlar:
- Integración de cambios.
- Issues.
- Milestones.
- Projects.
- Ramas.
- Pull Requests.
- Revisiones.

De esta manera, se pudo visualizar el estado de las actividades y conocer los avances realizados por cada integrante.

### Pull Request

Una vez finalizado el trabajo en una rama personal, se realizó el envío de los cambios mediante un Pull Request.

El flujo utilizado fue:

Rama personal
      ↓
    Commit
      ↓
     Push
      ↓
 Pull Request
      ↓
Asignación de revisor
      ↓
  Revisión
      ↓
  Aprobación
      ↓
    Merge
      ↓
     main

El Pull Request permitió solicitar formalmente la integración de los cambios realizados en la rama personal hacia la rama principal (Main).

### Revisión de cambios

Durante el proceso de Pull Request se asignó al compañero correspondiente como revisor.
La revisión permitió verificar los cambios realizados antes de integrarlos a la rama principal.
Este procedimiento ayuda a reducir errores y facilita la colaboración entre los integrantes del equipo.

### Merge
Después de completar el proceso de revisión, los cambios fueron integrados mediante un merge.
El proceso permitió incorporar los avances de las ramas personales a la rama principal:

rama personal
      │
 Pull Request
      │ 
      ▼
   Revisión
      │
      ▼
    Merge
      │
      ▼
     main
     
## Comandos principales utilizados
### Comando	Función
git init	Inicializa un repositorio Git
git status	Muestra el estado del repositorio
git add .	Agrega cambios al staging
git commit -m "mensaje"	Registra cambios
git branch	Lista las ramas
git branch nombre	Crea una rama
git checkout nombre	Cambia de rama
git switch nombre	Cambia de rama
git merge nombre	Integra una rama
git pull	Descarga y sincroniza cambios
git push	Envía cambios al repositorio remoto
git remote -v	Muestra los repositorios remotos

## Flujo colaborativo aplicado

El flujo general utilizado durante el taller fue:

Crear y configurar el repositorio.
Configurar el archivo .gitignore.
Preparar el entorno de trabajo mediante PowerShell.
Crear el Project en GitHub.
Crear las secciones del Project.
Crear el Milestone.
Crear los Issues.
Vincular los Issues con el Milestone y el Project.
Asignar las tareas a los integrantes.
Crear ramas personales.
Realizar modificaciones y commits.
Enviar los cambios mediante push.
Crear un Pull Request.
Asignar un compañero como revisor.
Revisar los cambios.
Realizar el merge.
Actualizar el estado de las actividades en GitHub.

## Conclusiones

El desarrollo del taller permitió aplicar un flujo de trabajo colaborativo utilizando Git y GitHub, desde la configuración inicial del repositorio hasta la integración de los cambios mediante Pull Requests y Merge.

El uso de Issues, Projects y Milestones permitió organizar las actividades y realizar seguimiento al trabajo de los integrantes, mientras que el uso de ramas permitió desarrollar cambios de manera independiente antes de integrarlos a la rama principal.

Finalmente, el proceso de revisión mediante Pull Requests permitió establecer un mecanismo de control antes de incorporar los cambios al repositorio principal, simulando un flujo de trabajo utilizado en proyectos de desarrollo de software.

## Autores
Edwin Ballesteros
Bairon Diaz

# Repositorio:
https://github.com/EdwinBalles-T/proyecto-colaborativo-Grupo7.git
