# RestApiBackEnd
Rest API Backend mock created with __Node JS__ and consumed by __Angular__ App.

## Install
Run `npm install`

## Development server
Just run `npm run json-server` to start the **Rest Server**. Then go to http://localhost:3000/


# Getting started
There is the file __db.json__ with some examples loaded, just some examples to test it:

* To __read__ existing logs, use **GET**: 
  * To list them all: http://localhost:3000/log/
  * To get one, inform the __id__: http://localhost:3000/log/1

* To __add__ a new log use **POST**: http://localhost:3000/log/ with the body:

  ```json
  {
      "level": "INFO",
      "id": "600600602",
      "clase": "com.paquete.nombre",
      "metodo": "doLogin",
      "mensaje": "El login ha funcionado correctamente 600600602"
  }
  ```

## Modules
Used modules:
* **json-server**: fast full fake REST API, see more in https://github.com/typicode/json-server

## Sources
Based on a tutorial:
* **URL**: [rest api backend tutorial](https://www.sitepoint.com/angular-rxjs-create-api-service-rest-backend/).
* **Git**: [angular-todo-app](https://github.com/sitepoint-editors/angular-todo-app)
