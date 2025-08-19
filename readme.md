---

# Práctica: Fundamentos de Git

Hola profe! Acá te dejo los pasos que seguí para la actividad práctica de la unidad. Fui anotando los comandos que usé y te agrego sugerencias de capturas por si hace falta.

---


## 1. Configuración de Git

Primero configuré mi nombre, email

```bash
git config --global user.name "Gustavo Baranda"
git config --global user.email "baranda.gustavo@gmail.com"
```

---


## 2. Creación del repositorio local

Después armé la carpeta del repo, lo inicialicé y revisé que todo esté vacío y listo para arrancar:

```bash
mkdir AprendiendoGit
cd AprendiendoGit
git init
ls -la
git status
```

---


## 3. Creación y preparación de archivos

Arranqué creando el `Readme.md` directamente en VS Code (lo edité a mano) y luego lo agregué al staging. Acá los comandos que ejecuté:

```bash
git status
git add Readme.md
git status
```

---


## 4. Abrir en Visual Studio Code

Abrí el repo en VS Code para trabajar más cómodo:

```bash
code .
```

---


## 5. Agregar la fecha y realizar commit

Le sumé la fecha al Readme y lo guardé con un commit. Así queda registro de cuándo hice el cambio:

Agregué la fecha manualmente en el `Readme.md` desde VS Code y luego hice el commit. Los comandos que ejecuté fueron:

```bash
git status
git add Readme.md
git commit -m "Fecha"
```

---


## 6. Agregar archivo HTML y hacer commit

Después armé el `index.html` con un título y lo subí al repo:

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Introducción a GIT</title>
</head>
<body>
  <h1>Introducción a GIT</h1>
</body>
</html>
```

Y después:

```bash
git add index.html
git commit -m "Agregar index.html"
```

---

## 7 Subida a GitHub (repositorio remoto)

Subí el repositorio a GitHub, los comandos que usé fueron:

```bash
# crear el remoto (reemplazar la URL si es otra)
git remote add origin https://github.com/GustavoBaranda/AprendiendoGit.git
# verificar remotos
git remote -v
# subir la rama master
git push -u origin master
```

Invité al usuario `javierblancoedu` para que pueda revisar el repo en GitHub.

## 7. Mostrar historial y cambios

Revisé el historial y los cambios hechos:

```bash
git status --short
git log --oneline --graph --decorate --all
git show --stat HEAD
```

---

