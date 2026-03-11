# EJERCICIOS TIPO

## 1. Filtros

Crear un FILTRO en "GET /users" de modo que:  
GET /users?page=1&limit=5&country=uruguay

- Reciba por Query el nombre del país, y devuelva solamente los usuarios residentes en el país solicitado
- La ruta GET /users debe conservar también el paginado que ya tiene, pero sobre los usuarios filtrados

## 2. Ordenamientos

GET /users?page=1&limit=5&order=asc
Crear un ORDENAMIENTO en "GET /users" de modo que:

- Reciba por Query "asc" o "desc", y cuyo valor por defecto sea "asc" (si no se envía este valor por query)
- Si se recibe "asc": devuelva los usuarios ordenados en forma ascendente (de la "A" a la "Z") por la propiedad "name"
- Si se recibe "des": devuelva los usuarios ordenados en forma descendente (de la "Z" a la "A") por la propiedad "name"
- La ruta GET /users debe conservar también el paginado que ya tiene

## 3. GET /categories/:id

Crear una Ruta "GET /categories/:id":

- Recibir el "id" del producto a obtener por params
- Buscar y retornar el producto correspondiente
- Si no se encuentra el producto, retornar una excepción con un mensaje representativo

## 4. Borrado Lógico

Implementar el borrado lógico en la ruta "DELETE /users":

- Crear una nueva propiedad "isActive" en la entidad "User" que tenga un valor true por defecto
- Al borrar un usuario, no eliminarlo de la base de datos, sino pasar la propiedad "isActive" a false
- En la ruta "GET /users" filtrar los usuarios cuya propiedad "isActive: false" de modo de no retornarlos (estos usuarios son virtualmente invisibles para nosotros)

## 5. Agregar nuvo atributo a la Entida Users

Agregar a la Entidad Users el Atributo "birthdate":

- Debe ser una fecha con el formato "dd/mm/yyyy"
- Debe marcarse como obligatorio
- dropSchema = true // false

## 6. Auth

Crear un nuevo rol de "SuperAdmin", y proteger la ruta "GET /products"

- Crear lo necesario en la entidad y el dto
- Setear la propiedad correspondiente en la Metadata de la ruta
- Crear el Guardián que validará el paso

## 7. Estandarizar Respuestas

Unificar la respuesta de todos los Endpoints de tal modo que:

- Nuestro Backend siempre retorne un objeto
- Definiendo un formato estándar de respuesta según una interfaz
- Tipar los retornos de los métodos

```ts
export interface ApiResponse {
  success: boolean;
}

GET /users
{
  "success": true,
  "message": "Listado de usuarios",
  "data": Date,
  "response": [ {...}, {...} ],
  "error": null,
}
```

## 8. Estandarizar Errores

Unificar el manejo de errores de tal modo que:

- Nuestro Backend siempre retorne un objeto similar
- Crear un Exception Filter Global

## 9. Middlewares, Interceptors, Pipes, Guards

- Filtrar el password de usuarios de forma global => Interceptor

| Tipo                | Cuándo se ejecuta                | Para qué sirve                         |
| ------------------- | -------------------------------- | -------------------------------------- |
| 🧩 **Pipe**         | Antes del controlador            | Validar y transformar datos            |
| 🛡️ **Guard**        | Antes de los Pipes               | Autenticación y autorización           |
| 🎯 **Interceptor**  | Antes y después del controlador  | Transformar respuesta, logging, cache  |

## 10. Simulacro de Ejercicio

Baneo de Usuarios por parte del Administrador

1. Crear nuevo atributo en el Modelo Users de la Base de Datos
   - Llamarlo "isBlocked" y cuyo tipo sea "boolean"
   - Darle valor "false" por defecto
   - Impedir que el valor pueda ser enviado en el Body
2. Crear una ruta "PUT /users/blocked/:id"
   - Esta ruta cambia el valor de "isBlocked" al usuario cuyo ID se recibe por params
   - Proteger la ruta para que solo sea accesible por Administradores
3. Agregar este atributo al Payload del Token
   - Restringir el acceso a todo usuario bloqueado
