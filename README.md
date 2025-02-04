
# **Guía para el Uso de GitHub**

## **Introducción**
Este documento tiene como objetivo principal guiar a un equipo de programadores en la adopción y uso de GitHub, basándose en la demo presentada en el video [1]. Se incluirán ejemplos, referencias a puntos clave del video y explicaciones detalladas en español, para garantizar la comprensión de aquellos miembros del equipo que no dominan el inglés.

> [1] Video de referencia:  
> [https://www.youtube.com/watch?v=Hpx4Zlu8ujk](https://www.youtube.com/watch?v=Hpx4Zlu8ujk)

A lo largo de este documento, encontrarás secciones dedicadas a cada parte importante de la demo, con fragmentos breves del video (por ejemplo, el minuto **5:43**) para ilustrar o aclarar conceptos cuando sea necesario.

---

## **1. Descripción General de GitHub**
GitHub es una plataforma de desarrollo colaborativo que permite:
- Alojar y gestionar repositorios de código.
- Revisar código mediante pull requests y comentarios.
- Controlar versiones a través de la integración con Git.
- Organizar proyectos y tareas con herramientas de seguimiento (issues, proyectos, etc.).

En la demo se muestra cómo GitHub facilita la colaboración entre varios desarrolladores, permitiendo llevar un control detallado de los cambios y versiones del proyecto.

---

## **2. Creación de una Cuenta y Configuración Inicial**
1. **Crear una cuenta**: El primer paso es registrarse en [github.com](https://github.com/). Se solicita un correo electrónico, nombre de usuario y contraseña.
2. **Configuración de perfil**: Añadir foto de perfil, bio y otras opciones para personalizar tu cuenta.
3. **Instalar Git (en local)**: Para trabajar con GitHub desde tu equipo, debes tener Git instalado. Se recomiendan versiones actualizadas de Git para evitar problemas de compatibilidad.  
   - Windows: [https://git-scm.com/download/win](https://git-scm.com/download/win)  
   - macOS: [https://git-scm.com/download/mac](https://git-scm.com/download/mac)  
   - Linux: Se instala normalmente desde el gestor de paquetes (ej. `sudo apt-get install git`).

**Referencia rápida** (minuto **5:43** del video):  
> *“Aquí podemos ver cómo configurar rápidamente el nombre de usuario y el correo en nuestra terminal para que Git sepa quién hace los commits…”*

Configurar usuario y correo en Git local:
```bash
git config --global user.name "TuNombreDeUsuario"
git config --global user.email "tu@correo.com"
```
Estas credenciales ayudarán a identificarte en cada commit que realices.

---

## **3. Creación de Repositorio en GitHub**
1. **Iniciar un nuevo repositorio**: Desde tu cuenta de GitHub, haz clic en el botón “New” o “Nuevo repositorio”.
2. **Rellenar detalles**: Asigna un nombre, una descripción (opcional) y decide si el repositorio será público o privado.
3. **Inicializar con un README**: Marca la casilla “Add a README file” para que tengas un archivo básico de documentación.
4. **Elegir licencia** (opcional): GitHub ofrece opciones de licencias de software libre o propietario.

---

## **4. Clonar un Repositorio y Sincronizar Cambios**
Una vez creado el repositorio en GitHub, puedes **clonarlo** (copiarlo) a tu máquina local.

1. **Obtener URL** del repositorio desde la página principal de tu repo en GitHub (botón verde “Code”).
2. **Clonar usando Git**:
   ```bash
   git clone https://github.com/TuUsuario/TuRepositorio.git
   ```
3. **Crear y editar archivos** en local.
4. **Realizar cambios**:
   ```bash
   git add .
   git commit -m "Mensaje descriptivo de los cambios"
   ```
5. **Enviar (push)** los cambios a GitHub:
   ```bash
   git push origin main
   ```

---

## **5. Branches (Ramas) y Trabajo Colaborativo**
Una de las funciones más potentes de GitHub es el manejo de ramas que permite desarrollar nuevas características sin afectar la rama principal (**main**).

1. **Crear una rama**:
   ```bash
   git checkout -b nombre-rama
   ```
2. **Realizar cambios y subir la rama**:
   ```bash
   git push origin nombre-rama
   ```
3. **Pull Request (PR)**: Al terminar tu cambio, puedes crear una Pull Request en GitHub para que el equipo revise y apruebe antes de fusionar con la rama principal.

---

## **6. Uso de Issues y Seguimiento de Tareas**
GitHub incluye un sistema de **Issues** para:
- Reportar bugs.
- Proponer mejoras.
- Asignar tareas específicas a los miembros del equipo.

**Cómo crear un Issue**:
1. Entrar a la pestaña “Issues” de tu repositorio.
2. Hacer clic en “New Issue”.
3. Añadir un título y descripción detallada.
4. Asignar etiquetas (labels) para clasificar (ej. *bug*, *enhancement*, *question*).

---

## **7. Integraciones y Herramientas Adicionales**
- **GitHub Actions**: Para automatizar pruebas, despliegues u otras tareas.  
- **Projects**: Tableros tipo *Kanban* para organizar flujos de trabajo y tareas.  
- **GitHub Pages**: Permite alojar sitios estáticos directamente desde un repositorio de GitHub.

---

## **8. Consejos de Colaboración y Flujo de Trabajo**
- Mantener la rama **main** siempre **estable** y con código funcional.  
- Crear ramas de trabajo para cada tarea o funcionalidad nueva.  
- Realizar **commits** con frecuencia y con mensajes claros.  
- Realizar revisiones de código (pull requests) y retroalimentar de manera constructiva.  
- Sincronizar constantemente el repositorio local con **main** para evitar conflictos de fusión.

---

## **9. Referencia Rápida**
- **Configurar Git**:
  ```bash
  git config --global user.name "TuNombre"
  git config --global user.email "tu@correo.com"
  ```
- **Clonar repositorio**:
  ```bash
  git clone URL-del-repositorio
  ```
- **Crear rama**:
  ```bash
  git checkout -b nombre-rama
  ```
- **Agregar y hacer commit**:
  ```bash
  git add .
  git commit -m "Mensaje del commit"
  ```
- **Subir cambios**:
  ```bash
  git push origin nombre-rama
  ```

---

## **Conclusiones**
El video explica de manera práctica cómo arrancar con GitHub y aprovecharlo para el control de versiones y la colaboración en equipo. A continuación, se resumen los puntos más importantes:

1. **Registrar una cuenta en GitHub** y **configurar Git** a nivel local.  
2. **Crear repositorios** públicos o privados según la necesidad.  
3. **Clonar repositorios y trabajar con ramas** para mantener un código organizado.  
4. Emplear **pull requests** para revisión de código antes de fusionar cambios.  
5. Usar **Issues y Projects** para la gestión y organización de tareas.

---

*Documento creado por [TuNombre / Equipo X]*  
*Fecha: [dd/mm/aaaa]*
