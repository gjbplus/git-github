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

- ` git init ` Inicializa un repositorio git en la carpeta activa al ejecutar el comando
  -  En la carpeta activa se crea un carpeta oculta con nombre .git
  -  Esa carpeta **no se puede borrar** ya que se perdería todo el historial y configuraciones.


  


