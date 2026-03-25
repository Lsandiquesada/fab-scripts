# Guía de Funcionamiento de Repositorios Git

Este repositorio tiene como objetivo principal explicar el flujo de trabajo básico de Git, desde la configuración inicial del entorno hasta la conexión segura con un servidor remoto como GitHub mediante llaves SSH.

## Descripción

Un **repositorio** es un espacio donde Git realiza un seguimiento de todos los cambios realizados en los archivos de un proyecto. Esto permite:
* Mantener un historial de versiones.
* Revertir cambios si algo sale mal.
* Colaborar con otras personas sin sobrescribir el trabajo ajeno.

---

## Instalación y Configuración Inicial

Sigue estos pasos detallados para configurar tu entorno de desarrollo y conectar tu computadora con GitHub de forma segura.

### 1. Instalar Git Bash
Descarga e instala la última versión de Git para tu sistema operativo desde [git-scm.com](https://git-scm.com/). En Windows, se recomienda usar **Git Bash** para tener una terminal compatible con comandos Unix.

### 2. Configuración de Identidad
Antes de crear commits, debes identificarte. Abre Git Bash y ejecuta los siguientes comandos con tu información:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```
### 3. Generar llave SSH

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```
### 4. Registrar la llave en GitHub

GitHub > Settings > SSH and GPG keys > New SSH key
Se debe copiar el contenido de la llave y guardar.

### 5. Clonar el repositorio

```bash
git clone git@github.com:usuario/nombre-del-repo.git
```
