# Notas sobre git y github
Notas y conceptos para aprender git y github

Para comenzar es necesario tener instalado git que lo pueden descargar desde este [enlace](https://git-scm.com/downloads) 
realizan la instalación según su sistema operativo y luego de terminar abren la consola de git llamada git bash
y comprueban que git esté correctamente instalado con el siguiente comando

` git --version `

Podemos acceder a la ayuda de git con el siguiente comando:

` git help `

Para obtener ayuda especifica de un comando escribimos: git help [nombre del comando]
Ejemplo:

` git help config `

Para configurar nuestro nombre escribimos el comando git config --global user.name "Nombre Apellido"
Ejemplo:

` git config --global user.name "Guillermo Jaurena" ` y presionamos enter

- Si el comando es ejecutado correctamente pasa a la sigueinte línea.
- En caso de error, se muestra el mensaje de error y no se realizan cambios.

Ahora debemos configurar nuestro email que debe ser el mismo que tenemos registrado en github
Ejemplo: 

` git config --global user.email "ventasgjb@gmail.com" ` y presionamos enter

Para ver el listado de las configuraciones globales ejecutamos el siguiente comando:

` git config --global -e`

Se muestran las configuraciones globales dentro de un editor de texto
- Si queremos modificar pulsamos la tecla ` a ` para habilitar la edición
- una vez termianda la edición: pulsamos la tecla esc, luego escribimos `:wq!` para salir guardando cambios
- si queremos salir sin guardar los cambios, tecla esc, luego escribimos `:q!` para salir sin guardar cambios

---
### Lista de comandos

- ` git init ` Inicializa un repositorio git en el directorio activo al ejecutar el comando
  -  En la carpeta activa se crea un directorio oculto con nombre .git
  -  Ese directorio **no se puede borrar** ya que se perdería todo el historial y configuraciones.
 
- ` git status ` Proporciona información sobre:
    - los commits
    - la rama en la que se encuentran
    - archivos y directorios en stage (con seguimiento en el repositorio)
    - archivos y directorios sin seguimiento

- ` git add ` permite agregar archivos para realizar el seguimiento del repositorio
    - git add archivo.txt - agrega cada archivo de forma individual
    - ` git add . `
      - agrega todos los archivos del directorio al stage
      - prepara todos los archivos para realizar el proceso de commit

- ` git reset archivo.txt` quita un archivo o directorio que no se quiere realizar seguimiento
-  ` git commit -m "Primer commit" ` este comando realiza el commit
    - Realizar una captura de archivos y configuraciones en ese momento
    - -m " descripcion " es la forma de agregar la descripción de lo que incluye ese commit
    - Es recomendable incluir la descripción adecuada a los cambios realizados
    - No es recomendado hacer commit sin una descripción
    - Luego de hacer commit podemos ver su estado con el comando ` git status `
    - Se recomienda hacer un commit al terminar un cambio o funcionalidad importante
    - Se puede regresar a cada uno de los puntos de commit en cualquier momento

- ` git config core.autocrlf true `
    - Configura el fin de línea automatico en diferentes sistemas operativos
    - Este aviso que se muestra al detectar que se está dando esta combinación de sistemas
    - Al usar este comando se realiza la configuración para evitar errores

- ` git log ` Muestra el detalle para cada commit incluyendo: 
    - Fecha y hora de realizado
    - Autor del commit
    - Rama en la que se encuentra
    - Puede incluir mas detalles


  


