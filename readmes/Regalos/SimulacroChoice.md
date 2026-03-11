# SIMULACRO DE CHECKPOINT - M4 BACKEND

[Volver a inicio](../../README.md)

## ¡Atención equipo! 🚀

> Este es un simulacro del checkpoint, así que la idea es que se tomen dos horitas y lo hagan como si fuera el real 💪
> 
> Eso sí… tenemos 60 preguntas en lugar de 40, así que pueden tomarse dos horas y cuarto. ¡Un bonus de 15 minutos cortesía de la casa! 😂
> 
> ¡Vamos con todo y éxitos en este entrenamiento! 💥

## 1. ¿Qué comando se utiliza para crear un nuevo proyecto NestJS?

- a) nest start new
- b) npm init nest
- c) nest new
- d) npm run nest new

<details> <summary>Respuesta correcta...</summary> c) `nest new` </details>

## 2. ¿Qué decorador se utiliza para definir un controlador en NestJS?

- a) @Injectable()
- b) @Controller()
- c) @Module()
- d) @Get()

<details> <summary>Respuesta correcta...</summary> b) `@Controller()` </details>

## 3. ¿Qué hace un Pipe en NestJS?

- a) Intercepta las solicitudes HTTP antes del controlador
- b) Transforma y valida los datos de entrada
- c) Gestiona la respuesta del servidor
- d) Registra logs del sistema

<details> <summary>Respuesta correcta...</summary> b) Transforma y valida los datos de entrada </details>

## 4. ¿Cuál de los siguientes módulos permite integrar Swagger en NestJS?

- a) @nestjs/swagger
- b) @nestjs/swagger-ui
- c) swagger-nest
- d) nestjs-docs

<details> <summary>Respuesta correcta...</summary> a) `@nestjs/swagger` </details>

## 5. Dado el siguiente código, ¿qué devolverá la ruta /hello?

```ts
@Controller()
export class AppController {
  @Get("hello")
  getHello() {
    return "Hola Nest!";
  }
}
```

- a) Error 404
- b) JSON vacío
- c) "Hola Nest!"
- d) undefined

<details> <summary>Respuesta correcta...</summary> c) "Hola Nest!" </details>

## 6. En NestJS, ¿qué se utiliza para manejar errores globalmente?

- a) Interceptors
- b) Guards
- c) Exception Filters
- d) Pipes

<details> <summary>Respuesta correcta...</summary> c) Exception Filters </details>

## 7. ¿Qué decorador se usa para definir una ruta tipo POST en un controlador?

- a) @Put()
- b) @Post()
- c) @Route('post')
- d) @HttpPost()

<details> <summary>Respuesta correcta...</summary> b) `@Post()` </details>

## 8. ¿Qué hace un Interceptor en NestJS?

- a) Valida los datos
- b) Modifica las solicitudes o respuestas
- c) Filtra excepciones
- d) Maneja la autenticación

<details> <summary>Respuesta correcta...</summary> b) Modifica las solicitudes o respuestas </details>

## 9. ¿Cuál es el propósito del decorador @UseGuards()?

- a) Inyectar dependencias
- b) Aplicar middlewares
- c) Proteger rutas mediante autorización
- d) Manejar excepciones

<details> <summary>Respuesta correcta...</summary> c) Proteger rutas mediante autorización </details>

## 10. ¿Cómo se define una entidad en TypeORM para NestJS?

- a) Usando @Model()
- b) Usando @Entity()
- c) Usando @Table()
- d) Usando @Database()

<details> <summary>Respuesta correcta...</summary> b) Usando `@Entity()` </details>

## 11. ¿Qué método del módulo SwaggerModule inicializa la documentación?

- a) SwaggerModule.init()
- b) SwaggerModule.start()
- c) SwaggerModule.setup()
- d) SwaggerModule.bootstrap()

<details> <summary>Respuesta correcta...</summary> c) `SwaggerModule.setup()` </details>

## 12. ¿Qué comando permite generar un servicio en NestJS?

- a) nest g module
- b) nest g controller
- c) nest g service
- d) nest new service

<details> <summary>Respuesta correcta...</summary> c) `nest g service` </details>

## 13. Dado el siguiente controlador, ¿qué devuelve la ruta /users/10?

```ts
@Controller("users")
export class UsersController {
  @Get(":id")
  findOne(@Param("id") id: string) {
    return `User ID: ${id}`;
  }
}
```

- a) "User ID: id"
- b) "User ID: 10"
- c) Error 404
- d) undefined

<details> <summary>Respuesta correcta...</summary> b) "User ID: 10" </details>

## 14. ¿Qué hace el decorador @InjectRepository()?

- a) Inyecta un módulo de NestJS
- b) Inyecta una dependencia HTTP
- c) Inyecta un repositorio de TypeORM
- d) Crea una instancia de controlador

<details> <summary>Respuesta correcta...</summary> c) Inyecta un repositorio de TypeORM </details>

## 15. ¿Cuál es el propósito del archivo main.ts en un proyecto NestJS?

- a) Definir las rutas
- b) Configurar la base de datos
- c) Iniciar la aplicación y montar el módulo raíz
- d) Crear controladores

<details> <summary>Respuesta correcta...</summary> c) Iniciar la aplicación y montar el módulo raíz </details>

## 16. ¿Qué devuelve un método marcado con @Post() por defecto si no se especifica un código de estado?

- a) 200 OK
- b) 201 Created
- c) 204 No Content
- d) 500 Internal Server Error

<details> <summary>Respuesta correcta...</summary> b) 201 Created </details>

## 17. ¿Qué comando se usa para correr la aplicación NestJS en modo desarrollo?

- a) npm start
- b) nest serve
- c) npm run start:dev
- d) nest run dev

<details> <summary>Respuesta correcta...</summary> c) `npm run start:dev` </details>

## 18. ¿Qué función de Cloudinary se usa comúnmente para subir un archivo?

- a) cloudinary.upload()
- b) cloudinary.uploader.upload()
- c) cloudinary.fileUpload()
- d) cloudinary.sendFile()

<details> <summary>Respuesta correcta...</summary> b) `cloudinary.uploader.upload()` </details>

## 19. ¿Qué decorador se usa para extraer el cuerpo del request en un método POST?

- a) @Body()
- b) @Param()
- c) @Req()
- d) @Query()

<details> <summary>Respuesta correcta...</summary> a) `@Body()` </details>

## 20. En NestJS, los Guards se ejecutan...

- a) Antes de los pipes
- b) Después de los interceptors
- c) Antes de los controladores
- d) Después del filtro de excepciones

<details> <summary>Respuesta correcta...</summary> c) Antes de los controladores </details>

## 21. ¿Qué propiedad en TypeOrmModule.forRoot() define el nombre de la base de datos?

- a) database
- b) name
- c) dbName
- d) schema

<details> <summary>Respuesta correcta...</summary> a) `database` </details>

## 22. ¿Qué hace el decorador @ApiTags() de Swagger?

- a) Define el nombre del controlador en Swagger
- b) Genera la documentación automática de los métodos
- c) Agrupa endpoints bajo un mismo tag en la UI de Swagger
- d) Genera ejemplos de respuesta

<details> <summary>Respuesta correcta...</summary> c) Agrupa endpoints bajo un mismo tag en la UI de Swagger </details>

## 23. ¿Qué parámetro del método SwaggerModule.createDocument() recibe la configuración básica?

- a) options
- b) config
- c) builder
- d) documentOptions

<details> <summary>Respuesta correcta...</summary> a) `options` </details>

## 24. ¿Cuál de las siguientes opciones define un módulo correctamente?

```ts
@Module({
  imports: [],
  controllers: [AppController],
  providers: [AppService],
})
export class AppModule {}
```

- a) Correcto
- b) Incorrecto, falta el decorador @Controller()
- c) Incorrecto, no debe tener controllers
- d) Incorrecto, providers no es válido

<details> <summary>Respuesta correcta...</summary> a) Correcto </details>

## 25. ¿Qué decorador se usa para inyectar un servicio dentro de otro servicio?

- a) @Injectable()
- b) @Inject()
- c) @Service()
- d) @Provide()

<details> <summary>Respuesta correcta...</summary> b) `@Inject()` </details>

## 26. ¿Cuál es el propósito del decorador @UseInterceptors()?

- a) Definir un guard global
- b) Aplicar pipes a un método
- c) Aplicar interceptores a un controlador o método específico
- d) Configurar middlewares

<details> <summary>Respuesta correcta...</summary> c) Aplicar interceptores a un controlador o método específico </details>

## 27. ¿Qué decorador de NestJS se utiliza para definir una ruta base en un controlador?

- a) @Route()
- b) @Controller('ruta')
- c) @Path()
- d) @Endpoint()

<details> <summary>Respuesta correcta...</summary> b) `@Controller('ruta')` </details>

## 28. En TypeORM, ¿qué método se usa para guardar una entidad?

- a) repository.save()
- b) repository.insert()
- c) repository.create()
- d) repository.persist()

<details> <summary>Respuesta correcta...</summary> a) `repository.save()` </details>

## 29. Si un pipe lanza una excepción, ¿qué sucede?

- a) El controlador la ignora
- b) Se devuelve un error HTTP automáticamente
- c) La excepción es capturada por el interceptor
- d) El proceso se detiene sin respuesta

<details> <summary>Respuesta correcta...</summary> b) Se devuelve un error HTTP automáticamente </details>

## 30. ¿Qué módulo se utiliza para gestionar la configuración de variables de entorno?

- a) @nestjs/env
- b) @nestjs/config
- c) dotenv-nest
- d) nest-environment

<details> <summary>Respuesta correcta...</summary> b) `@nestjs/config` </details>

## 31. ¿Cuál es el decorador que permite definir un parámetro de consulta (query param)?

- a) @Body()
- b) @Param()
- c) @Query()
- d) @Req()

<details> <summary>Respuesta correcta...</summary> c) `@Query()` </details>

## 32. En NestJS, un Guard debe implementar cuál interfaz:

- a) CanExecute
- b) CanActivate
- c) OnRequest
- d) AuthGuard

<details> <summary>Respuesta correcta...</summary> b) `CanActivate` </details>

## 33. En un proyecto NestJS con TypeORM, ¿qué función inicializa la conexión?

- a) TypeOrmModule.forRoot()
- b) DatabaseModule.connect()
- c) Connection.init()
- d) AppModule.registerDB()

<details> <summary>Respuesta correcta...</summary> a) `TypeOrmModule.forRoot()` </details>

## 34. ¿Qué hace un Global Pipe?

- a) Aplica validaciones a todas las rutas
- b) Solo funciona en un controlador
- c) Aplica filtros de errores globales
- d) Configura los interceptores globales

<details> <summary>Respuesta correcta...</summary> a) Aplica validaciones a todas las rutas </details>

## 35. En un archivo app.module.ts, ¿dónde se registran los controladores?

- a) En imports
- b) En controllers
- c) En providers
- d) En exports

<details> <summary>Respuesta correcta...</summary> b) En `controllers` </details>

## 36. ¿Qué decorador de Swagger se usa para describir una respuesta HTTP?

- a) @ApiResponse()
- b) @ApiReturn()
- c) @ApiOutput()
- d) @ApiResult()

<details> <summary>Respuesta correcta...</summary> a) `@ApiResponse()` </details>

## 37. ¿Qué decorador de NestJS permite definir un módulo reutilizable?

- a) @Reusable()
- b) @Module()
- c) @Injectable()
- d) @Shared()

<details> <summary>Respuesta correcta...</summary> b) `@Module()` </details>

## 38. ¿Qué método del repositorio TypeORM elimina una entidad por ID?

- a) removeById()
- b) delete()
- c) destroy()
- d) erase()

<details> <summary>Respuesta correcta...</summary> b) `delete()` </details>

## 39. ¿Qué se usa para definir la estructura del cuerpo de una petición en Swagger?

- a) @ApiBody()
- b) @ApiSchema()
- c) @ApiParam()
- d) @ApiForm()

<details> <summary>Respuesta correcta...</summary> a) `@ApiBody()` </details>

## 40. ¿Qué módulo de NestJS facilita el manejo de archivos en las peticiones?

- a) @nestjs/file
- b) @nestjs/platform-express
- c) @nestjs/upload
- d) @nestjs/storage

<details> <summary>Respuesta correcta...</summary> b) `@nestjs/platform-express` </details>

## 41. ¿Qué interceptor se utiliza comúnmente para transformar respuestas?

- a) MapResponseInterceptor
- b) TransformInterceptor
- c) ResponseMapper
- d) BodyInterceptor

<details> <summary>Respuesta correcta...</summary> b) `TransformInterceptor` </details>

## 42. En una autenticación JWT, ¿dónde se suele incluir el token?

- a) En el cuerpo de la petición
- b) En la URL
- c) En la cabecera Authorization
- d) En una cookie

<details> <summary>Respuesta correcta...</summary> c) En la cabecera `Authorization` </details>

## 43. ¿Qué decorador se usa para declarar una propiedad como clave primaria?

- a) @PrimaryKey()
- b) @Id()
- c) @PrimaryGeneratedColumn()
- d) @Column({ primary: true })

<details> <summary>Respuesta correcta...</summary> c) `@PrimaryGeneratedColumn()` </details>

## 44. ¿Qué librería suele usarse junto a Cloudinary para manejar archivos en NestJS?

- a) multer
- b) busboy
- c) express-fileupload
- d) formidable

<details> <summary>Respuesta correcta...</summary> a) `multer` </details>

## 45. ¿Cuál es el propósito del decorador @ApiProperty()?

- a) Documentar propiedades en DTOs
- b) Crear propiedades dinámicamente
- c) Validar propiedades de entidades
- d) Definir valores predeterminados

<details> <summary>Respuesta correcta...</summary> a) Documentar propiedades en DTOs </details>

## 46. ¿Qué función usa JwtService para verificar un token?

- a) verifyToken()
- b) decode()
- c) verify()
- d) check()

<details> <summary>Respuesta correcta...</summary> c) `verify()` </details>

## 47. ¿Qué hace @UsePipes(new ValidationPipe()) en un controlador?

- a) Lanza errores automáticamente si la validación falla
- b) Aplica interceptores
- c) Resuelve dependencias
- d) Ejecuta middlewares

<details> <summary>Respuesta correcta...</summary> a) Lanza errores automáticamente si la validación falla </details>

## 48. ¿Qué decorador se utiliza para definir la estrategia de autenticación JWT?

- a) @JwtStrategy()
- b) @UseGuards()
- c) @PassportStrategy()
- d) @AuthStrategy()

<details> <summary>Respuesta correcta...</summary> c) `@PassportStrategy()` </details>

## 49. ¿Cuál de los siguientes NO es un tipo de provider en NestJS?

- a) Clase
- b) Fábrica
- c) Valor
- d) Archivo

<details> <summary>Respuesta correcta...</summary> d) Archivo </details>

## 50. ¿Qué se necesita para habilitar CORS en NestJS?

- a) app.use(cors())
- b) app.enableCors()
- c) CorsModule.forRoot()
- d) @EnableCors()

<details> <summary>Respuesta correcta...</summary> b) `app.enableCors()` </details>

## 51. ¿Qué propiedad define la relación entre entidades en TypeORM?

- a) @Join()
- b) @Relation()
- c) @ManyToOne()
- d) @LinkedEntity()

<details> <summary>Respuesta correcta...</summary> c) `@ManyToOne()` </details>

## 52. ¿Qué método del repositorio obtiene todos los registros?

- a) getAll()
- b) findAll()
- c) find()
- d) list()

<details> <summary>Respuesta correcta...</summary> c) `find()` </details>

## 53. ¿Qué decorador de NestJS se usa para acceder al objeto Request?

- a) @Req()
- b) @HttpRequest()
- c) @Body()
- d) @Param()

<details> <summary>Respuesta correcta...</summary> a) `@Req()` </details>

## 54. ¿Qué decorador de Swagger define un parámetro de ruta?

- a) @ApiParam()
- b) @ApiBody()
- c) @ApiRoute()
- d) @ApiPath()

<details> <summary>Respuesta correcta...</summary> a) `@ApiParam()` </details>

## 55. En NestJS, ¿cómo se definen middlewares?

- a) Implementando NestMiddleware
- b) Con @Middleware()
- c) Dentro del módulo principal
- d) En el archivo main.ts

<details> <summary>Respuesta correcta...</summary> a) Implementando `NestMiddleware` </details>

## 56. ¿Qué devuelve repository.findOneBy({ id: 3 }) si no encuentra el registro?

- a) undefined
- b) null
- c) Lanza una excepción
- d) false

<details> <summary>Respuesta correcta...</summary> a) `undefined` </details>

## 57. ¿Qué decorador se usa para exportar un módulo y compartirlo con otros?

- a) @Share()
- b) @Export()
- c) exports dentro del @Module()
- d) @Provide()

<details> <summary>Respuesta correcta...</summary> c) `exports` dentro del `@Module()` </details>

## 58. ¿Qué hace el método app.useGlobalInterceptors()?

- a) Define interceptores globales para todas las rutas
- b) Aplica pipes globalmente
- c) Configura guards globales
- d) Inicializa Swagger

<details> <summary>Respuesta correcta...</summary> a) Define interceptores globales para todas las rutas </details>

## 59. ¿Qué archivo suele almacenar las credenciales de Cloudinary?

- a) .env
- b) cloudinary.json
- c) config.ts
- d) main.ts

<details> <summary>Respuesta correcta...</summary> a) `.env` </details>

## 60. ¿Qué método del servicio de Cloudinary elimina una imagen?

- a) cloudinary.deleteFile()
- b) cloudinary.uploader.destroy()
- c) cloudinary.remove()
- d) cloudinary.uploader.delete()

<details> <summary>Respuesta correcta...</summary> b) `cloudinary.uploader.destroy()` </details>

---

[Volver a inicio](../../README.md)