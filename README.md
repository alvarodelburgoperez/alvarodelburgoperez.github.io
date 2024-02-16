# Crear un entorno virtual

---

1. Accedemos a la carpeta donde queremos crear el entorno virtual:

```bash
cd C:\Users\alvar\Desktop\DevOps
```

2. Creamos el entorno con este comando:

```bash
python -m venv entorno_mkdocs
```

3. Accedemos al entorno:

```bash
cd entorno_mkdocs
```

4. Activamos el entorno con este comando: 

```bash
.\Scripts\activate
```

# Instalar Mkdocs

---

1. Accedemos al entorno:

```bash
C:\Users\alvar\Desktop\DevOps\entorno_mkdocs
```

2. Ejecutamos el comando de instalación de mkdocks:

```bash
pip install mkdocs
```

3. Creamos el proyecto de mkdocs:

```bash
mkdocs new pagina_mkdocs
```

4. Entramos al directorio del proyecto:

```bash
cd pagina_mkdocs
```

5. Construimos los html del proyecto:

```bash
mkdocs build
```

6. Para ver el archivo index localmente ejecutamos:

```bash
mkdocs serve
```

# Subir archivos al github

---

1. Vamos al directorio donde esta el repositorio local:

```bash
C:/Desktop/DevOps/entorno_mkdocs/pagina_mkdocs
```

2. Añadimos el repositorio al proyecto con el comando:

```bash
git remote add origin https://github.com/alvarodelburgoperez/alvarodelburgoperez.github.io
```

Si no funciona el comando anterior, ejecutamos este comando:

```bash
git config --global --add safe.directory C:/Users/alvar/Desktop/DevOps/entorno_mkdocs/pagina_mkdocs
```

3. Creamos la rama develop y feature:

```bash
git checkout -b feature
```

```bash
git checkout -b develop
```

4. Cambiamos a la rama feature:

```bash
git checkout feature
```

5. Relacionamos la rama feature que hemos creado en Git con la del repositorio de GitHub:

```bash
git pull origin feature --allow-unrelated-histories
```

6. Añadimos los archivos:

```bash
git add .
```

7. Hacemos un commit:

```bash
git commit -m "Initial Commit”
```

8. Subimos los archivos:

```bash
git push origin feature
```

```bash
git push -u origin feature
```

9. Fusionamos la rama feature con la rama main:

```bash
git rebase main
```

```bash
git fetch origin
```
