# Mi Proyecto de Evaluación CI/CD

Este repositorio es la evaluación práctica 1 de la asignatura DevOps sobre los fundamentos de Git, modelo de ramas y automatización con GitHub Actions.

## Tabla de Contenidos

- [Instalación](instalación)
- [Uso](uso)
- [Tecnologías](tecnologías)

## Instalación

Para clonar y probar este proyecto localmente, sigue estos pasos:

1. Clona el repositorio:

    ```bash
    git clone https://github.com/Xang-Shoku-Liao/Ev1-DevOps.git
    ```

2. Accede al directorio:

    ```bash
    cd Ev1-DevOps
    ```

## Uso

Este proyecto no requiere ejecución de código, su propósito es la validación de flujos CI mediante GitHub Actions. Al realizar un Push o Pull Request, el linter revisará automáticamente la sintaxis de los archivos.

## Tecnologías

- Git
- GitHub Actions
- Markdownlint

## Automatización (CI/CD)

En este proyecto utilizamos **GitHub Actions** como nuestra herramienta de automatización para implementar la Integración Continua (CI).

**¿Cuál es su rol en nuestro flujo de trabajo?**
GitHub Actions nos permite ejecutar procesos automáticos cada vez que alguien del equipo sube código nuevo. Esto es fundamental en la cultura DevOps porque nos ayuda a detectar errores rápidamente antes de que el código llegue a los usuarios finales.

**Nuestra configuración (ci-cd.yml):**
Hemos configurado un flujo de trabajo que se dispara automáticamente bajo dos condiciones:

1. Cuando se hace un *push* directo a la rama `develop`.
2. Cuando se abre un *Pull Request* hacia la rama `main`.

Actualmente, este archivo simula la descarga del código y la ejecución de pruebas unitarias. Al automatizar este paso, garantizamos que todo código nuevo que intente fusionarse con nuestras ramas principales sea validado, manteniendo la estabilidad y calidad de nuestro microservicio.
