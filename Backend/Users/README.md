# ProyectoFinalHenry / Users

---
# Modelo users.
### Developer: Sergio Valdivia

**Tecnoligias:**
1. Express
2. NodeJS
3. PostgreSQL
4. Cors
5. Dontenv
6. Sequelize
7. Sequeli-cli
7. Axios
8. Multer
9. Moment

### Este microservicio será el encargado de crear, almacenar, listar, los datos tanto de los clientes como de los colaboradores del restaurante.

*Se guardarán basados en un ID que proporciona la base de datos, adicionalmente se hará relación de ellos con el token y el rol:*

- El nombre del usuario.
- El apellido del usuario
- El numero telefónico.
- El email (con el cual se hará la validacion).
- La dirección.
- El rol que cumple dentro del restaurante (cliente = regular, admin, cajer@, meser@, cociner@, etc).
- Un conteo de los pedidos que haya hecho siempre y cuando sea cliente.
- El avatar (se hará enlace con avatar.com por medio del correo brindado por el usuario).
- Una contraseña.

> Todos estos datos los entregara en formato Json para poder ser consumidos por el ApiGateway el cual se encarga de entregar toda la información necesaria al Front para poder ser mostrada al consumidor final.Todos estos datos los entregara en formato Json para poder ser consumidos por el ApiGateway el cual se encarga de entregar toda la información necesaria al Front para poder ser mostrada al consumidor final.

```json
"id",
"name";
"lats_name";
"phone",
"email",
"addres",
"role",
"history_menu",
"avatar",
```

##### Para iniciar el microservicio:Para iniciar el microservicio:

- Clonar el repositorio con git clone [Ir al Repositorio](http://https://github.com/CarlosGiovannyG/ProyectoFinalHenry/tree/main "Enlace del Repositorio")
- Dirigirse a la carpeta Backend/Users
- Instalar todas las dependencias con npm i.
- Iniciar el servidor con npm run dev ya que está en producción
- Ir al localhost en el puerto 7000 [Ir a localhost](http://localhost:7000 "Ir a localhost")

**Las rutas con que cuenta el microservicio son:**
1. Una ruta para registro de usuario.
2. Una ruta para Login de usuario.
3. Una ruta para modificar datos.
4. una ruta para consultar las estadísticas de pedidos del usuario.