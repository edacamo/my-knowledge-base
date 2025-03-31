---
layout: default
title: "Comandos para subir un nuevo proyecto a un repositorio en GitHub"
---

# Comandos para subir un nuevo proyecto a GitHub

Si tienes un proyecto local y deseas subirlo a un nuevo repositorio en GitHub, sigue estos pasos:

1. **Navega al directorio de tu proyecto**:
    ```bash
    cd /ruta/a/tu/proyecto
    ```

2. **Inicializa el repositorio Git**:
    ```bash
    git init
    ```

3. **Agrega todos los archivos al área de staging**:
    ```bash
    git add .
    ```

4. **Haz el primer commit**:
    ```bash
    git commit -m "Primer commit"
    ```

5. **Agrega el repositorio remoto en GitHub**:
    ```bash
    git remote add origin https://github.com/tu-usuario/nombre-del-repo.git
    ```

6. **Descarga los últimos cambios del repositorio remoto (si es necesario)**:
    ```bash
    git fetch origin
    ```

7. **Renombra la rama local de 'master' a 'main'**:
    ```bash
    git branch -m master main
    ```

8. **Sube la rama 'main' al repositorio remoto y configura el seguimiento**:
    ```bash
    git push -u origin main
    ```

9. **Eliminar la rama remota 'master' (si es necesario)**:
    ```bash
    git push origin --delete master
    ```

---

> Estos comandos te permitirán inicializar un repositorio Git local, vincularlo a un repositorio remoto en GitHub, y hacer el primer push de tu proyecto. Asegúrate de que la rama principal sea `main`, ya que es la convención más reciente en GitHub.

[Volver a la página principal](index.md)
