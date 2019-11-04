# jwt-training

Para **firmar** nuestro token utilizaremos un paquete de node llamado jsonwebtoken y al usarlo en nuestro código se verá de esta manera:

**jwt.sign({ sub: user.id }, 'secret', options);**

El primer atributo que recibe es el payload o sea los datos que guardaremos en ese token. De segundo atributo recibe una clave secreta con la cual será firmado y finalmente podremos pasarle opciones si es nuestro caso.
Para **verificar** nuestro token lo haremos de la siguiente manera:

**jwt.verify(token, 'secret', function(err, decoded){});**

Como primer atributo recibiremos el token, de segundo atributo el secreto de la firma y como tercer argumento (opcional) recibiremos el token decodificado.
Vamos a inicializar nuestro proyecto con npm init -y
Crearemos el archivo index.js
Vamos a instalar los paquetes necesarios con npm i jsonwebtoken
En el index.js vamos a hacer toda la lógica de nuestra aplicación
