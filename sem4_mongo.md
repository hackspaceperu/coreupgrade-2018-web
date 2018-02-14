<h3> Semana 3 </h3>
<h1> MongoDB </h1>

Luego de crear nuestro web server de manera más eficiente con express, aún nos hace falta almacenar data a través de nuestro servidor, para ello haremos uso de una técnología que con el paso del tiempo ha ido creciendo hasta el punto de convertirse en una de las bases de datos más usadas. Esto no quiere decir que sea la mejor, ya que es muy distinta a las bases de datos más conocidas como MySQL, Oracle o SQL-Server, la gran diferencia entre MongoDB y las mencionadas anteriormente es en el paradigma __"No relacional"__ de esto es que se le conoce como una __"NoSQL"__.

A diferencia de la bases de datos "Relacionales" que usan tablas como estructura básica, MongoDB hace uso de estructuras similares a JSON para almacenar información.

Si deseas saber más acerca de MongoDB puedes visitar el siguiente [enlace](https://www.mongodb.com/es).

## Ventajas de usar MongoDB

En la actualidad la cantidad de data almacenada ha crecido de manera exponencial, se caracterizan por ser grandes, no estructurados y, a veces, difíciles de manejar, esto ha llevado al desarrollo de bases de datos NoSQL.

Las ventajas de usar MongoDB son:

* __Schema less__: MongoDB es una base de datos de documentos en la que una colección contiene diferentes documentos. El número de campos, el contenido y el tamaño del documento pueden diferir de un documento a otro.

* Almacenamiento orientado a documentos: Los datos se almacenan en forma de documento de estilo JSON.

* Sin uniones complejas y alta disponibilidad.

* Capacidad de consulta profunda. MongoDB admite consultas dinámicas en documentos usando un lenguaje de consulta basado en documentos que es casi tan poderoso como SQL, esto permite consultas rápidas.

* Altamente escalable, además utiliza la memoria interna para almacenar el conjunto de trabajo (en ventana), lo que permite un acceso más rápido a los datos.

## ¿Dónde usar MongoDB?

* Big Data
* Gestión de contenido y delivery
* Infraestructura Móvil
* Redes Sociales
* Gestión de datos de usuario
* Hub de datos

## Estructura de una Base de Datos de MongoDB

### Colección

Una colección es un grupo de documentos MongoDB. Es el equivalente de una tabla en un [RDBMS](https://es.wikipedia.org/wiki/Sistema_de_gesti%C3%B3n_de_bases_de_datos_relacionales).

### Documento

Un documento es un conjunto de pares clave-valor. Los documentos tienen un esquema dinámico. El esquema dinámico significa que los documentos en la misma colección no necesitan tener el mismo conjunto de campos o estructura, y los campos comunes en los documentos de una colección pueden contener diferentes tipos de datos.

La siguiente tabla muestra la relación de la terminología RDBMS con MongoDB.

| RDBMS        | MongoDB           |
| ------------- |:-------------:|
| Tabla      | Colección |
| Tupla/Fila      | Documento |
| Columna      | Campo |

Ahora vamos a mostar el ejemplo de un documento:

```javascript
_id: ObjectId(8ef12ew8231c)
titulo: 'Mi primer lenguaje',
autor: 'Kurisu Makise',
contenido: 'El primer lenguaje en el que aprendí a programar fue C++',
fecha: new Date(2018,1,1,2,1),
tags: ['C++','programación'],
likes: 322,
comentarios: [
    {
        usuario: 'Rintarou Okabe',
        mensaje: 'Wow increible!!!',
        fecha: new Date(2018,2,1,3,15),
        likes: 2
    },
    {
        usuario: 'Mayuri Shiina',
        mensaje: 'Tuturuuu',
        fecha: new Date(2018,1,3,4,20),
        likes: 4
    }
]
```
El atributo `_id`, Es creado por MongoDB, tambien puede ser provisto por el usuario.

Ahora vamos a crear una pequeña aplicación usando MongoDB y Node.js para ello vamos a crearnos una cuenta en __mLab__, una plataforma que nos ofrece una BD gratuita en la nube y nos ahorrará el proceso de instalación.

Para crear una cuenta en mLab sigue el siguiente [enlace](https://mlab.com).

Nuestra aplicación será un pequeño TODO list donde guardaremos nuestras tareas para luego leerlas desde nuestra base de datos.

No nos enfocaremos demasiado en los estilos de aplicación así que se va a ver un poco rudimentario.

Iniciaremos nuestra aplicación

```bash
mkdir todo-list
cd todo-list
npm init
```

Luego de esto instalaremos algunos paquetes que vamos a usar como express,body-parser, mongodb y además un template engine para renderizar contenido dinámico llamado [handlebars](http://handlebarsjs.com/installation.html).

```bash
npm install express --save
npm install body-parser --save
npm install mongodb --save
npm install handlebars --save
```

Luego de crear una cuenta en mLab y recibir el correo de confirmación hacemos lo siguiente:

Creamos nuestra BD en Create New en MongoDB Deployment:
<p align="center">
    <img src="img/mongo2.png">
</p>

Luego elegimos a nuestro proveedor en este caso amazon:

<p align="center">
    <img src="img/mongo3.png">
</p>

Nombramos a nuestra BD en mi caso lo terminé llamando todo-list-hackspace ya que no me aceptó todo-list :(
<p align="center">
    <img src="img/mongo4.png">
</p>

Luego al final tendremos nuestra BD ya creada:

<p align="center">
    <img src="img/mongo5.png">
</p>

Si hacemos click en esta instancia veremos que nos dice como conectarnos con nuestra base datos haciendo uso de nuestro usuario y contraseña:

<p align="center">
    <img src="img/mongo6.png">
</p>

Vamos a usar la misma estructura que usamos en la parte de express pero le añadiremos un modulo de conexion a nuestra BD:

```










