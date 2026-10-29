# MiApp
markdown
# 🚀 MiApp - Panel de Control del Repositorio

Este proyecto está configurado para trabajar con el ecosistema de desarrollo de **Google Antigravity IDE**. Cuenta con un flujo de trabajo estructurado en dos ramas principales para mantener el código organizado y seguro.

## 🌿 Estructura de Ramas

*   **`dev` (Rama Activa):** Aquí es donde programas día a día. Todos los archivos nuevos, experimentos y funciones web se suben primero aquí.
*   **`main` (Producción):** Guarda la versión limpia, estable y terminada de tu aplicación web.

---

## 🛠️ Guía Rápida: ¿Cómo subir mis cambios a GitHub?

Cada vez que crees una nueva sección en tu aplicación web (por ejemplo, el diseño del HTML, estilos CSS o funciones JavaScript) y quieras guardarla en la nube, abre tu terminal de PowerShell y ejecuta estos **3 comandos**:

```powershell
# 1. Selecciona y prepara todos los archivos nuevos o modificados
git add .

# 2. Guarda el progreso con un mensaje corto que explique qué hiciste
git commit -m "feat: agregada la estructura inicial de la app web"

# 3. Sube tus cambios de forma segura a la rama de desarrollo en GitHub
git push origin dev
```

---

## 📈 Flujo de Trabajo Recomendado

1.  **Verificar dónde estás parado:** Antes de escribir código, asegúrate de estar en desarrollo ejecutando `git checkout dev`.
2.  **Hacer commits pequeños:** Es mejor subir cambios cada vez que termines una pequeña parte (ej: "creado el botón de ingreso") en lugar de subir todo el proyecto junto al final de la semana.
3.  **Paso a Producción (Opcional):** Cuando tu página web funcione perfecto y quieras actualizar la rama principal `main`, ejecuta:
    ```powershell
    git checkout main
    git merge dev
    git push origin main
    git checkout dev
    ```

    