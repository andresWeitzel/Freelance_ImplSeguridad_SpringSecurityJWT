# Desarrollo Freelance Implentando Módulo de Seguridad con Spring Security y Json Web Token.

### Descripción
* A través de mis Proyectos Open Source publicados en esta plataforma me contactó un desarrollador para realizar la securización de un módulo de un proyecto utilizando Spring Security y algún Módulo para la autenticación y demás (Auth0, JWT, etc). Se termino optando el módulo JWT ya que a comparación con Auth0 y otros tiene limitaciones en cuanto a su uso gratuito. No es recomendable para escalabilidad con la versión no paga.
* El Desarrollo se llevo a cabo año actual 2022 (principios de marzo hasta fines abril).
* Se me asignó desarrollar las entidades que funcionarían como autenticación, usuarios del sistema (roles, características, etc), nuevos usuarios, manejo de passwords y campos cifrados, signin, login, refresh token, uso de tokens, entre otros. Todas estas funcionalidades desarrolladas las tuve que documentar en diversos .readme para cada branch implementado respecto a cada funcionalidad enumerada.
* El desarrollo fue a medida ya que se me pidió que la documentación de la Api (no .readme) para este módulo en concreto se realice con SpringFox y Swagger (las nuevas docs se realizan con Open-Api v3.0, por ende supuse que el objetivo fue mantener el proyecto y de a poco ir actualizándolo. No tuve información concreta al respecto ya que este módulo iba a servir de base para la implementación de la securización completa de la aplicación ).
* Al igual que el desarrollo freelance de la Api Rest de Productos, por temas de `DERECHO INTELECTUAL, PAGO TOTAL DEL SERVICIO DESARROLLADO Y ÉTICOS NO SE ANEXA CÓDIGO FUENTE DEL DESARROLLO`.
* Con respecto a la arquitectura implementada a nivel base de datos solamente se persistieron las tablas en una db test/mock desde Spring Data JPA con el Mapeamiento interno de Spring. Las mismas fueron roles (admin, user), usuarios(todos los usuarios del sistema, la lógica de negocios para autenticación y registro se persisten en base a esta tabla) y la tabla relación muchos a muchos respecto a usuarios y roles (Normalización). Luego para la capa de Negocios se implementaron todas las buenas prácticas que una Api Rest requiera, más allá que el objetivo principal fuese la documentación y la implementación de la Securización. Se anexan algunos proyectos al final de este repo implementando dicha lógica.
* El objetivo de trabajar con JWT fue devolver un response con un token con la fírma y credenciales válidas desde el backend para que desde el endpoint requerido se valide y autentique desde el frontend. Mi parte fue solo el Backend, pero anexo algunos proyectos personales donde implemento ambos realizando una app completa.
* Las tecnologías implementadas fueron Spring Boot Spring MVC (validaciones), Spring Security, JWT, Spring Fox, Swagger, Lombok, Log4j, Git, pgAdmin, PostgreSQL, y otras tecnologías.

</br>

#### Endpoint locales entregados
* http://localhost:8093/api/v1/auth/ (Autenticación y Registro de usuarios)
* http://localhost:8093/api/v1/refresh-token/ (Actualización de Token Caducado)
* http://localhost:8093/api/v1/usuarios/ (Administración de Usuarios del Sistema a Nivel Backend)
* En todos los endpoint se desarrollaron los recursos pertinentes a cada funcionalidad requerida.

<hr>

</br>

### Proyectos Personales que implementan Spring Security y JWT
* Aplicación Web acerca de Productos de Electrónica (Frontend, Backend y Database) : https://gitlab.com/andres-weitzel/AppTiendaElectronica_Angular_Bootstrap_SpringBoot_MongoDB
* App Web Productos de Supermercado (Frontend, Backend y Database): https://github.com/andresWeitzel/App_MicroFrontEnd_Productos_SpringBoot_SpringSecurity_PostgreSQL
* Otros (Perfíl Github).



### Ejemplo Gráfico Prueba de Funcionaldiad Api Rest Productos Supermercado (Spring Security y JWT).

</br>


### Login y Signin 
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/loginSignin.png)](https://www.youtube.com/watch?v=vxmJAXwahNk&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=2) 

### Refresh Token
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/refreshToken.png)](https://www.youtube.com/watch?v=P_iGkoIgXFM&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=3) 

### Usuario Controller
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/usuarioController.png)](https://www.youtube.com/watch?v=eG7dirCPflU&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=3) 


### Usuario Bean Validations (Add)
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/beanUsuariosValidat01.png)](https://www.youtube.com/watch?v=U-6sD-k4_lg&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=4) 


### Usuario Bean Validations (Update and Delete)
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/beanUsuariosValidat02.png.png)](https://www.youtube.com/watch?v=o8vOd0dERFI&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=5) 


### Producto Controller
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/productoController.png)](https://www.youtube.com/watch?v=JqrTA97Y4N4&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=4) 

### Producto Bean Validations (CRUD)
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/beanProductosValidation.png)](https://www.youtube.com/watch?v=ytdwagCbJXU&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=7) 


### Documentación SwaggerUI / SpringFox
[![Alt text](https://github.com/andresWeitzel/ApiRest_MicroFrontEnd_ProductosSupermercado/blob/master/doc/miniaturasYt/docSwagger.png)](https://www.youtube.com/watch?v=F2BlURXQaDs&list=PLCl11UFjHurBM42b3iBbQ7iilddzG4t_L&index=5) 



