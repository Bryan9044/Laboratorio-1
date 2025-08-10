# Laboratorio#1 Bryan Londoño Marchena!

## 1. *Frameworks de desarrollo web*

Framework seleccionado - *Vue*
a. En si un framework lo que hace es darnos una plantilla o una base con la cual empezar a trabajar en el desarrollo de aplicaciones de forma que nos ahorra tiempo en ciertas tareas que antes tal vez fueran más rutinarias, de esta forma los programadores se pueden centrar más en la lógica y en el funcionamiento del mismo.
b. La  arquitectura de *Vue* se basa en el modelo MVVM (modelo - vista - vista modelo) el cual es uno relativamente nuevo además de esto, la separación lógica que contiene lo hace muy flexible y ordenado pues se basa en separar la parte de la capa de presentación y la lógica empresarial, además de esto sus componentes se utilizan en base a su estado
c. 
Estructura de un proyecto en Vue
├── node_modules/
├── public/
├── index.html
├── src/
├── .eslintrc.js
├── .gitignore
├── .prettierrc.json
├── .vscode/
├── e2e/
├── .env
├── package.json
├── package-lock.json
├── playwright.config.js
├── vitest.config.js
└── vite.config.js
En este caso la carpeta denominada como *public* sería la carpeta raíz de nuestro proyecto en esta vamos a guardar los ficheros estáticos o los que no van a ser utilizados por el framework.
Luego está la carpeta *src* que es la carpeta o por lo menos es considerada por mí persona como la más importante pues en este tendremos nuestro código fuente generalmente, aquí están los archivos que vamos a modificar mediante un editor de texto, además de estos dependiendo de la configuración del proyecto ya sea *typescript* o *javascript* tendremos un archivo *main.ts* o *main.js* .

Luego tendremos un archivo como App.vue el cual es casi como un html porque tiene 3 estructuras que son < template >, < script > y < style > 

En la carpeta *assets* guardaremos los archivos estáticos como lo pueden ser las imágenes, audios o videos estos son los que utilizaremos dentro de nuestro código. 
La carpeta *router* sirve para crear rutas dentro del frontend esto lo podemos utilizar para crear aplicaciones con APIS, generalmente su archivo se llama *index.js* o *index.ts* 

Para la carpeta stores generalmente esta solo se utiliza si se combina con pinia o para almacenar algún tipo de estado 

Y por último la carpeta *components/*  en esta carpeta se van a guardar los archivos .vue que se creen durante la ejecución del proyecto es importante recordar que estos son los que contienen html, css y js 

d.  Para la comparación será entre *Vue* y *Angular*  las dos son relativamente similares pues ambas utilizan javascript un lenguaje relativamente derivado del otro pues Angular utiliza *typescript*  los cuales son muy parecidos sin embargo Vue se enfoca más para una curva de aprendizaje más fácil y con despliegue de proyectos más rápido sin embargo typescript es un poco más compleja y se usa para proyectos con mayor escala. 

## *2. Control de versiones y trabajo colaborativo*

a. Un control de versiones se puede observar como una lista en las cuales se tendrán diferentes progresos o partes del proyecto según se requiera esto generalmente para llevar un mejor orden y así evitar problemas ante futuras actualizaciones.
b. 
*Repositorio:* Se puede observar como un sistema de almacenado el cuál contiene grandes cantidades de información
*Commit:* Se puede decir que es como un pre-guardado antes del guardado final.
*Branch:* Con esto se refiere especificamente a una rama la cual puede consistir en partes del proyecto que se separan para formar un todo. 
*Merge:* Esto es cuando se quiere realizar cambios en una rama la cual ya tiene cierto tipo de contenido
*Pull request:* Esto lo podemos observar como la acción de pedir subir nuestros cambios a la rama que deseemos y estos si son aprobados van a ser subidos a la rama en que se haya realizado 
c. Uno de estos flujos de trabajo es el flujo de trabajo centralizado lo que hace es que utiliza un repositorio central generalmente esta rama se llama Main y los cambios se realizan en esta rama si o si, en este caso uno de los supervisores debe confirmar todos los cambios o devolverlos en caso de que no cumplan los estándares, un ejemplo de estos es en la página de github . 
d.  Lo primero es tener una cuenta creada y estar en nuestra computadora, en este caso crearemos una carpeta donde vamos a guardar el repositorio, en este caso lo que se puede hacer es clonar un repositorio o crearlo desde cero en nuestra carpeta, entonces lo primero que haremos son los siguientes pasos:
1. Entrar en nuestra carpeta y abrir una terminal de comandos
2. Escribir lo siguiente *git innit* 
3. Sino tenemos la cuenta registrada se nos pedirá que la iniciemos 
4. Luego verificamos que exista una carpeta que se llame .git 
5. Después podemos agregar archivos como echo "# Mi proyecto" > README.md
6. Hacemos un git add . en caso de haber agregado archivos
7. Luego un commit para ir subiendo estos cambios y darle un nombre, escribimos lo siguiente *git commit -m "Prueba commit"*
8. Luego aca cambiamos el nombre de la rama *git branch -M main* 
9. *git push -u origin main* y guardamos los cambios que habíamos realizado. 
10. Esto es opcional, pero si queremos crear más ramas hacemos esto *git branch pruebaRama2*
11. Si queremos hacer cambios en la nueva rama es importante hacer lo siguiente que es pasarse de rama *git checkout pruebaRama2*

e. De forma personal y por experiencia recomendaría Github pues es una forma de utilizar repositorios de forma sencilla y sin muchas complicaciones pues te da muchas herramientas al momento de subir archivos además que por decirlo de alguna manera te protege ante posibles errores avisando si hay algún commit mal hecho o si un merge está muy por encima del otro entre otras cosas, sin embargo, en el mercado tecnologico se encuentras otras opciones igual de buenas como lo son: Taravault, Bitbucket y SourceForge.  

## *3. Autenticación y seguridad moderna*
a. 
*Autentificación:* Según Microsoft es el proceso que usan las empresas para confirmar que solo las personas, servicios y aplicaciones adecuados con los permisos correctos pueden acceder a recursos de la organización.
*Autorización:* La autorización es un método que comprueba que las credenciales solicitadas por una plataforma o persona sean correctas y de esta forma permite un acceso. 
*Tokens:* En general un token es reconocido por ser un tipo de activo digital, en estos casos puede representar monedas digitales, derechos de autor o el acceso a ciertos tipos de servicios. 
*JWT (Json Web Token):* Es un tipo de token el cual se encarga de recibir ciertos tipos de datos en formato Json para verificar la propiedad de una persona, la diferencia es que la cadena ya viene codificada y con URL seguro para ser utilizada. 
*OAuth:* Según Microsoft es un estándar tecnológico que permite autorizar a una aplicación o servicio a iniciar sesión en otra sin divulgar información privada, como contraseñas.
b.![Diagrama de JWT](https://drive.google.com/file/d/1prk6zxAKNjlCXZKiY3tb-UjD1EUETZEH/view?usp=sharing)
c. 
1. No dejar ninguna contraseña de forma que sea visible o algún dato sensible a la vista.
2. Utilizar protocolos https con certificado SSL para mayor seguridad.
3. Realizar copias de seguridad.
4. Limitar las acciones por medio de roles. 
5. Pedir autentificación de dos pasos para todos los usuarios.

d. Actualmente hay muchas de estas empresas que utilizan los consejos anteriores y más, algunas de estas podrían ser: Epic games la cual no importa en qué momento uno intente entrar siempre te va a pedir que, aunque coloques la contraseña de forma correcta lo verifiques por medio de un factor de dos pasos, además de esta tenemos a Google que utilizan los protocolos HTTPS y que permiten el uso de OAuth para iniciar sesión con otras aplicaciones y por último podríamos mencionar que el Auth0 utiliza JWT para la emisión de tokens. 

## *4. Gestores de contenidos desacoplados (Headless CMS)*
a.
**Headless CMS:** Este sistema se enfoca totalmente en lo que compete al backend o sea con la información que no está a la vista pues en esta se da la creación, modificación o el envio de estos mismos, pero no muestra nada con respecto al frontend. 

**CMS tradicional:** En este tipo de sistema el backend y el frontend estan fuertemente conectados, de forma que se puede ver como una asociación fuerte pues el uno sin el otro no funciona de la forma esperada, sino que fueron creados para mostrar y reproducir el contenido entre ellos mismos 
b. Generalmente su arquitectura se basa en el aprovechamiento por medio de APIS, pero no solo esto además utilizan un sistema de archivos o un almacenamiento de datos en la nube. Para solicitar el contenido estas utilizan las APIS de forma que con algún tipo de estas como lo pueden ser GraphQL O RESTful eligen de manera específica los datos o el contenido que desean traer para así poder mostrarlo de una forma constante o algunas lo combinan con un CRUD para su creación, lectura, actualización y eliminación de los datos que se tienen en el backend de forma que se mantiene más ordenado y limpio al momento de trabajar. 
c. 
Ventajas: 
1. Mayor flexibilidad al momento de modificar la capa de presentación.
2. Puede distribuir el contenido a distintas plataformas por medio de su API.
3. Tiene mayor escalabilidad en caso de ser necesario la agregación de más contenido.
4. Tiene mayor rendimiento pues solo consume los datos necesarios. 
Limitaciones:
1. Es más complejo pues este como tal no cuenta con un frontend.
2. Es muy dependiente de las APIS para su funcionamiento.
3. Necesita de conocimiento previo en APIS por lo cual la curva de aprendizaje es más lenta.
4. Prácticamente que no tiene plantillas ya predefinidas pues como cada una varía mucho por el tipo de dato que consuma no es tan eficiente el que existan. 
d. ![Ejemplo de cómo conectar un frontend con un headless cms ](https://drive.google.com/file/d/1p8d-b9efdw2jZ45k3aSQQnqRfJhesuR-/view?usp=sharing)

## *5. Pasarelas de pago en aplicaciones web*
a. Una pasarela de pago se puede ver como un método el cual contiene distintos servicios monetarios los cuales están a disposición de los usuarios y por el cual al utilizar uno de estos servicios se va a poder efectuar una transacción monetaria con el fin de pagar por un producto o servicio final. El rol que estos cumplen es el de automatizar procesos y el poder realizar compras en línea. 
b. **Cuenta de comercio:** Es una cuenta de banco especializada y dada por un banco oficial con el fin en que una empresa pueda recibir pagos y aceptar pagos de manera electrónica. 
**Seguridad:** Para los casos en los que la información es tan sensible es necesario utilizar encriptación y si es posible la tokenización para así sustituirlo por los datos de la tarjeta de forma que si se roban algo es solo un token y no la información real, además de esto se deben seguir las leyes informáticas de cada país con respecto a las transacciones bancarias. Además, existen ciertas normas a utilizar que son casi como un estándar las cuales se denominan PCI DSS en estas hay ciertos pasos o reglas a seguir para mantener las transacciones de una forma más segura. 
**Integración tecnica:** En este apartado lo más importante a definir es el tipo de API a utilizar y el tipo de información que se va a estar enviando a la pasarela, además de esto los tipos de verificaciones que se van a solicitar, para llevar a cabo el tener una pasarela robusta es necesario generar distintas pruebas a modo de observar si algo falla o si hay alguna posibilidad de filtrar la información.
c.
**Ventajas:**
	1. Hace más llamativo al sitio web.
	2. Mejora la experiencia del cliente.
	3. Permite una mayor expansión territorial.
	4. Ofrecen muchas alternativas al cliente.
**Limitaciones:**
	1. Generalmente se cobran comisiones al utilizarse.
	2. Es necesario utilizar sistemas de terceros (APIS)
	3. Puede existir el fraude (pagos con tarjetas robadas)
	4. Se tiene que invertir mucho dinero en la seguridad y en las pruebas.

d. Mi comparación la realizo a modo personal, en este caso yo elegi a **Paypal** y **Skrill** en general me parecen muy buenas aplicaciones sin embargo alguna mejor que otra, por ejemplo a mi parecer Paypal no cobra tantas comisiones al mover dinero a ciertas cuentas o al pasarlo de vuelta a tu tarjeta cosa que con **Skrill** es un porcentaje de casi un 7% del valor total del dinero que estes moviendo lo cual es bastante si se considera que es la cuenta de banco personal de uno, sin embargo al momento de recibir dinero me parece que **Skrill** si le gana y por bastante a **Paypal** ya que si ocupas que te paguen en **Skill** no es necesario que la otra persona tenga **Skrill** con que uno le pase un link único ya te puede realizar un pago a tu cuenta cosa que en **Paypal** no sucede pues si o si necesitas cuenta para enviar dinero a una persona de **Paypal**  y por último me parece que las dos reciben muy por debajo el dinero pues generalmente el dólar o la moneda en la que uno quiere cambiar siempre tienen un margen bastante alto, por lo cual te quitan al depositar y al cambiar. 

## *6. Automatización del despliegue y hosting moderno*

a. 
**CI (Integración continua):** Consiste en integrar los cambios del código en un repositorio de código fuente compartido de forma automática y frecuente. 
**CD (Distribución continua):** Es un proceso de dos partes que implica la integración, la prueba y la distribución de los cambios en el código. Mientras que en la distribución continua los cambios no llegan a implementarse en la etapa de producción de forma automática, en la implementación continua sí se logra. En general se usan en el desarrollo web pues permiten captar los errores con mayor facilidad y aunado a esto permite un mejor desarrollo durante todo el proceso pues al tener distintas fases se hacen mejores trabajos y con mayor retroalimentación. 
b.  

 1. 
Diferencias entre hostings 

|----------------------------------------------------| a
|	|Estático|--|Dinamico|									| 
|	|Fácil de constuir |--| Muy interactivo |		|
|	|Económico |--| Personalizable |					|
|	|Poco interactivo |--| Más costoso |				|
|		|Sin base de datos |--| Muy escalable |	|
|----------------------------------------------------|
c. Pasos para crear un flujo de despliegue automatizado
d.



Fuentes: 
[Framework: qué es y para qué sirve, significado, ejemplos, características y tipos](https://ebac.mx/blog/frameworks)
[Introducción — Vue.js](https://es.vuejs.org/v2/guide/#Empezando)
[Frameworks para desarrollo web: 15 ejemplos con características](https://blog.hubspot.es/website/framework-desarrollo-web)
[Flujo de trabajo de Git | Atlassian Git Tutorial](https://www.atlassian.com/es/git/tutorials/comparing-workflows)
[Iniciar repositorio Git y primer commit](https://desarrolloweb.com/articulos/iniciar-repositorio-git-primer-commit.html)
[Las 14 mejores alternativas GRATUITAS de GitHub (2025)](https://www.guru99.com/es/github-alternative.html)
[¿Qué es la autenticación? Definición y métodos | Seguridad de Microsoft](https://www.microsoft.com/es-mx/security/business/security-101/what-is-authentication?msockid=06b89eb8d93e62e727b68b8bd82263ee)
[¿Qué es un token, cómo funciona y para qué sirve? Tipos y ejemplos - Finect](https://www.finect.com/usuario/avillanuevae/articulos/que-es-un-token-como-funciona-y-para-que-sirve-tipos-y-ejemplos)
[Autenticación JWT, qué es y cuándo usarla | Ciberseguridad](https://ciberseguridad.com/guias/prevencion-proteccion/autenticacion-jwt/#%C2%BFQue_es_JWT)
[¿Qué es OAuth? | Seguridad de Microsoft](https://www.microsoft.com/es-es/security/business/security-101/what-is-oauth?msockid=06b89eb8d93e62e727b68b8bd82263ee)
[Las 10 MEJORES PRÁCTICAS de SEGURIDAD para tu SITIO WEB](https://km32.com/mantenimientos-webs/mejores-practicas-seguridad-sitio-web/)
[Headless CMS vs CMS tradicional: Diferencias clave](https://www.alumio.com/es/blog/headless-cms-vs-traditional-cms-key-differences)
[Headless CMS vs. CMS tradicional: ventajas y desventajas en comparación - alojamiento web](https://webhosting.de/es/headless-cms-vs-tradicional-cms-comparacion-ventajas-y-desventajas/)
[Cuenta de Comerciante vs. Pasarela de Pago: Principales diferencias](https://blog.payproglobal.com/es/merchant-account-vs-payment-gateway)
[Puntos esenciales de la seguridad de las pasarelas de pago para el comercio electrónico - 10Web](https://10web.io/blog/es/puntos-esenciales-de-la-seguridad-de-las-pasarelas-de-pago-para-el-comercio-electronico/)
[La integración y la distribución continuas (CI/CD)](https://www.redhat.com/es/topics/devops/what-is-ci-cd)
[Sitio web estático vs. dinámico: en qué se diferencian y cuál es la mejor elección - BC de SiteGround](https://www.siteground.es/kb/sitio-web-estatico-vs-dinamico/)
