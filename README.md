# Curso de JavaScript: Interacciones con HTML

## Paso 1: Creación del repositorio y estructura inicial (Usuario 1)

1. Crear un nuevo repositorio en GitHub:
   - Ve a GitHub y crea un nuevo repositorio.
   - Nómbralo como `curs-javascript-interaccions-HTML`.
   - Añade un README.md inicial y selecciona la opción para añadir un .gitignore si quieres (puedes seleccionar uno para proyectos de frontend si es el caso).

2. Clonar el repositorio en tu máquina local:
   
   git clone https://github.com/tu-usuario/curs-javascript-interaccions-HTML.git
   cd curs-javascript-interaccions-HTML
   

3. Configurar Git Flow:
   - Primero, debes tener instalado Git Flow. Si no lo tienes, puedes instalarlo usando:
     
     Para Linux/Mac:
     
     sudo apt-get install git-flow
     
     
     Para Windows: Debes descargarlo desde [aquí](https://gitflow.github.io/).

   - Luego, inicializa el flujo de trabajo:
     
     git flow init
     
   
   - Utiliza las configuraciones por defecto:
     - Nombre para la rama de desarrollo: `develop`
     - Nombre para la rama principal: `main` (o `master`, dependiendo de tus preferencias).

4. Añadir el boilerplate inicial:
   - Descarga el archivo boilerplate del link proporcionado.
   - Incluye los archivos del boilerplate en el repositorio y organiza la estructura:
     - Header
     - Barra de navegación con enlace a Home.
     - Footer.
     - Descripción breve del curso en la parte central.

5. Hacer commit y push inicial:
   
   git add .
   git commit -m "User1: Inicializando estructura del proyecto con boilerplate"
   git push origin develop
   

## Paso 2: Usuario 2 - Creación de las secciones Modificar Contenido HTML y Modificar Atributos HTML

1. Crear dos branches (features):

   Crear feature/contingutHTML:
   
   git flow feature start contingutHTML
   

   Crear feature/atributsHTML:
   
   git flow feature start atributsHTML
   

2. Implementar la sección Modificar Contenido HTML:
   - Crea un ejemplo similar al que mencionas en el link. 
   - Añade una explicación detallada del código JavaScript que modifica el contenido HTML.

3. Hacer commit y cerrar la feature:
   
   git add .
   git commit -m "User2: Añadida sección 'Modificar Contenido HTML'"
   git flow feature finish contingutHTML
   

4. Implementar la sección Modificar Atributos HTML:
   - Añade ejemplos de cómo JavaScript puede modificar atributos de elementos HTML, y escribe una explicación del código.

5. Hacer commit y cerrar la feature:
   
   git add .
   git commit -m "User2: Añadida sección 'Modificar Atributos HTML'"
   git flow feature finish atributsHTML
   

6. Push de las nuevas features a develop:
   
   git push origin develop
   

## Paso 3: Usuario 3 - Implementación de la sección Modificar Estilos CSS

1. Crear la branch feature/estilsCSS:
   
   git flow feature start estilsCSS
   

2. Añadir ejemplos sobre la modificación de estilos CSS:
   - Agrega ejemplos de cómo modificar el estilo de elementos HTML utilizando JavaScript, junto con comentarios y explicaciones del código.

3. Hacer commit y cerrar la feature:
   
   git add .
   git commit -m "User3: Añadida sección 'Modificar Estils CSS'"
   git flow feature finish estilsCSS
   

4. Push de los cambios a develop:
   
   git push origin develop
   

## Paso 4: Creación de la release v1.0 por el Usuario 3

1. Crear una release:
   
   git flow release start v1.0
   

2. Hacer commit de la release:
   
   git commit -m "User3: Release v1.0 con las features completadas"
   

3. Finalizar y etiquetar la release:
   
   git flow release finish v1.0
   git push origin main --tags
   git push origin develop
   

## Paso 5: Usuario 1 realiza un hotfix para mejorar la sección de Contenido HTML

1. Crear una branch de hotfix:
   
   git flow hotfix start milloresV_1_0
   

2. Realizar las mejoras necesarias:
   - Mejora en la sección de Modificar Contenido HTML creada por el Usuario 2.

3. Hacer commit y cerrar el hotfix:
   
   git add .
   git commit -m "User1: Mejora en la sección de Contenido HTML"
   git flow hotfix finish milloresV_1_0
   

4. Push de los cambios a main y develop:
   
   git push origin main
   git push origin develop
   

## Paso 6: Documentación del proceso en gh-pages

1. Crear una nueva branch gh-pages:
   
   git checkout -b gh-pages
   

2. Añadir documentación del proceso:
   - Añade un archivo index.html o README.md con la descripción teórica del proceso de Git y Git Flow.
   - Incluye capturas del proceso (puedes usar herramientas como `git log --graph` para mostrar la estructura de ramas).

3. Push de la branch gh-pages:
   
   git add .
   git commit -m "Documentación del proceso"
   git push origin gh-pages
   

4. Publicar GitHub Pages:
   - Ve al repositorio en GitHub, a la pestaña "Settings", y en la sección de "GitHub Pages", selecciona la branch gh-pages para que se publique la documentación.

## Paso 7: Crear un proyecto en GitHub

1. Crear el proyecto en GitHub:
   - Ve a la pestaña "Projects" del repositorio y crea un nuevo proyecto.
   - Crea columnas para las features (contingutHTML, atributsHTML, estilsCSS) y para el hotfix (milloresV_1_0).

