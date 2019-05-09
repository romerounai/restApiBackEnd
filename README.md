# RestApiBackEnd
Rest API Backend mock creado con __Node JS__ .

# Instalación
Desde la carpeta del proyecto ejecutar `npm install` (es necesario tener Node.JS).

# Ejecución  
Ejecutar `npm run json-server` para iniciar el **Rest Server**. Después acceder a http://localhost:3001/ . 

El script está configurado para:
* Lanzar en el puerto 3001.
* Permitir el acceso desde la red (abrir puerto en firewall).
* Autogenerar un ID para cada log (para pruebas en local).

# Inicio rápido
Las llamadas se irán listando en el fichero __db.json__ , que funciona a modo de BBDD, ejemplos de uso:

* Para __leer__ los logs existentes, utilizar peticiones HTTP **GET**: 
  * Listar todo: http://localhost:3001/log/
  * Recuperar un registro concreto por su __id__: http://localhost:3001/log/1

* Para __añadir__ nuevos logs utilizar peticioens HTTP **POST**: http://localhost:3001/log/ con el siguiente cuerpo (por ejemplo usar POSTMAN):

  ```json
  {
      "level": "INFO",
      "id": "600600602",
      "clase": "com.paquete.nombre",
      "metodo": "doLogin",
      "mensaje": "El login ha funcionado correctamente 600600602"
  }
  ```

# Dependencias (Modules)
El proyecto utiliza la siguiente dependencia:
* **json-server**: fast full fake REST API, see more in https://github.com/typicode/json-server

# Referencias
Se han utilizado las siguientes referencias:
* **URL**: [rest api backend tutorial](https://www.sitepoint.com/angular-rxjs-create-api-service-rest-backend/).
* **Git**: [angular-todo-app](https://github.com/sitepoint-editors/angular-todo-app)
