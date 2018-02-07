# Reto Semana 2 - Backend

## Introducción

Para este primer reto de backend deberás de construir una aplicación que use modulos y además usarás lo aprendido en la parte de archivos.

Para este reto debes hacer uso de los modulos __fs__ y __lodash__ para poder leer, crear archivos y además manejar arrays. Tambien debes hacer uso del modulo llamado __yargs__ para poder usar los argumentos de la linea de comandos de manera que cuando llamemos a nuestra aplicación quede así:

```bash
node server.js add --name='Lucas' --number=915271232
```


## IMPORTANTE
Debes usar la librería yargs, si deseas saber como usar yargs puedes ver el siguiente [enlace](https://github.com/yargs/yargs/blob/master/docs/examples.md).

Luego debes crear un modulo llamado contact.js que lea un archivo llamado directorio.json y además este modulo debe ser capaz de añadir, leer, listar y borrar un contacto y su respectivo numero de telefono como si fuera un objeto:

```javascript
contact = {
    name: 'Lucas',
    number: 915271232
}
```
Tu aplicación debe ser capaz de recibir estos argumentos:

```bash
# Añadir un contacto
node server.js add --name='Lucas' --number=915271232
# Resultado
Contact created
--
name: Lucas
number: 915271232
```

```bash
# Listar todos los contactos guardados
node server.js list
# Resultado
Printing 4 contacts(s).
--
name: Lucas
number: 915271232
--
name: Megumin
number: 124761238
--
name: Rem
number: 812398123
```

```bash
# Leer un contacto
node server.js read --name='Megumin'
# Resultado
Contact found
--
name: Megumin
number: 124761238
```


```bash
# Remove un contacto
node server.js remove --name='Rem'
Contact was removed
```

Al final tu proyecto debe quedar estructurado de la siguiente manera:

- directory-app
    * node_modules
    * contact.js
    * server.js
    * directorio.json
