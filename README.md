### Identificarse
Estos pasos se realizan por primera vez una vez que se instala git.

```bash
git config --global user.name "FIRST_NAME LAST_NAME"
git config --global user.email "MY_NAME@example.com"
```
### Crear un repositorio en git de forma local
Paso 1.- Eligir una ubicaion en donde vivira el proyecto

Paso 2.- Iniciar el repositorio: Ejecutar este comando dentro de la carpeta en donde vive el proyecto

```bash
git init 
```

### Crear puntos de restauracion 
(Opcional) Revisar como va el asunto
```bash
git status
```

Paso 1: Subir archivos al staged
```bash
git add .
```

Paso 2: Crear el punto de restauracion
```bash
git commit -m "Este es mi primer commit"
```

Repetir los pasos cuantas veces se necesite un **punto de restauracion** (Llamemoslo commit (^ - ^)/ )


## Enlazar repositorio en la nube con repositorio local
**Nota: Crear un repositorio en github**

**Paso 1.-** Enlazar el repositorio local con el repositorio en la nube

En la terminal en la ubicacion del archivo (**El enlace es de ejemplo**, se debe usar el enlaze del repositorio que esta en github)
```bash
git remote add origin https://github.com/Roque98/linuxjourney.git
```

**Opcional**: Verificar que la fuente remota este agregada
```bash
git remote -v
```

### Traer y enviar cambios al repositorio

**IMPORTANTE:** Antes de enviar cambios a la nube, siempre se debe hacer un pull primero.

**Traer cambios (pull)**
Para traer los cambios de la nube al respositorio local
// origin: El nombre de la fuente remota
// master: El nombre de la rama (Despues discutimos el asunto de las ramas)
```bash
git pull origin master
```

**Enviar cambios (push)**
```bash
git push origin master
```

### Detalles y notas adicionales

Otras formas de subir archivos al staged
```bash
git add nombre_carpeta/ASDFHFJKD/.
```

Identificarse de forma local en el repositorio local
```bash
git config --global --list
git config user.name "FIRST_NAME LAST_NAME"
git config user.email "MY_NAME@example.com"
```
