# Componente 4: Bitácora de Administración DevOps y Git

Este documento registra las configuraciones de control de versiones y el flujo de despliegue continuo implementados para asegurar el ciclo de vida de la documentación del **Grupo 5**.

## 1. Gestión de Colaboradores y Permisos
Para permitir el desarrollo concurrente del proyecto, se configuró el acceso al repositorio centralizado a los siguientes integrantes en rol de colaboradores con permisos de escritura (Write):
*   Valeria Rodriguez Loiza (Administradora DevOps)
*   Santiago Gil Guzman
*   Daniela Paz
*   Kenneth Gonzalez
*   Johan Erazo

## 2. Flujo de Despliegue Continuo (CD)
La arquitectura de documentación opera bajo un modelo de Automatización Cloud Git:
1.  **Repositorio Central:** Servido en la plataforma GitHub bajo la rama principal `main`.
2.  **Disparador (Trigger):** Cada confirmación de cambio (`git push` o commits directos) activa un flujo automatizado a través de los servidores de GitHub.
3.  **Entorno de Producción:** El compilador procesa el archivo `index.html` y expone de forma inmediata los cambios bajo el protocolo seguro HTTPS en el servicio GitHub Pages.

## 3. Registro de Control de Cambios (Log Base)
*   **Fase 1:** Inicialización del repositorio y adición de la plantilla obligatoria README.md.
*   **Fase 2:** Activación y aprovisionamiento del entorno Cloud con GitHub Pages.
*   **Fase 3:** Estructuración del archivo index.html con semántica formal y distribución para 4 componentes técnicos.
*   **Fase 4:** Creación del árbol de directorios para la segregación de evidencias de cada integrante del equipo.
