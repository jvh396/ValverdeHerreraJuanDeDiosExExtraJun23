# Examen HMIS Extraordinario Junio 2023
Examen HMIS  - 23 de junio 2023  - Convocatoria Extraordinaria

## EJERCICIO_0 (0.5 puntos)

1. Forkea este repositorio en tu cuenta personal de GitHub
1. Edita únicamente tu archivo personal con extensión `.md`: escribe tus datos donde se indica. 
1. Para entregar el ejercicio, envía tus cambios a este repositorio.

id | user | Nombre estudiante  | Página personal examen  
--- | --------- | ---------------------------------- | ---------------------
4	|	ccm953	|	C. M. Carlos 	|	[ccm953.md](ccm953.md)
6	|	dd657	|	D. Dawid 	|	[dd657.md](dd657.md)
7	|	ie127	|	E. H. Ilyass 	|	[ie127.md](ie127.md)
8	|	pfs341	|	F. S. Pedro 	|	[pfs341.md](pfs341.md)
11	|	lg330	|	G. Luca Daniel 	|	[lg330.md](lg330.md)
13	|	kg544	|	G. Kacper 	|	[kg544.md](kg544.md)
14	|	fgc367	|	G. C. Francisco De Borja Jose 	|	[fgc367.md](fgc367.md)
15	|	dhc651	|	H. C. David 	|	[dhc651.md](dhc651.md)
18	|	aj171	|	J. Anita 	|	[aj171.md](aj171.md)
23	|	amt871	|	M. T. Alejandro |	[amt871.md](amt871.md)
31	|	dp189	|	P. Deian Orlando 	|	[dp189.md](dp189.md)
32	|	jsh336	|	S. H. Jose Antonio 	|	[jsh336.md](jsh336.md)
33	|	asm978	|	S. M. Alejandro Tomas 	|	[asm978.md](asm978.md)
36	|	mve412	|	V. E. Manuel 	|	[mve412.md](mve412.md)
37	|	jvh396	|	V. H. Juan De Dios 	|	[jvh396.md](jvh396.md)
38	|	bz369	|	Z. E. Omar 	|	[bz369.md](bz369.md)


## EJERCICIO_1 (0.5 puntos)

- Accede a GitHub Classroom e inicia el ejercicio 1: https://classroom.github.com/a/0MgXfXik

- Clona en tu PC el repositorio del ejercicio 1 que se ha creado en el paso anterior y realiza en tu ordenador, usando los comandos de git necesarios, las siguientes operaciones **en el orden mismo en el que se indican**:

    1. Añade un archivo, por ejemplo `ejercicio1.md`
    1. Haz un par de commits en `main`. 
    1. Publica main en tu repo de GitHub.
    1. Crea una rama llamada `parte1`
    1. Realiza un par de commits en la rama `parte1`
    1. Publica la rama en tu repo de GitHub.
    1. Realiza las acciones sobre el repositorio para fusionar la rama `parte1` sobre `main` con un **merge de tipo rebase**
    1. Publica `main` en tu repo de GitHub


- Tras ello, sobre `main`: 
    1. crea otra rama llamada `parte2`
    1. Realiza un par de commits en la rama `parte2`
    1. Publica la rama `parte2`en tu repo de GitHub.
    1. Realiza las acciones sobre el repositorio para fusionar la rama `parte2` sobre `main` de manera que sea necesario un **merge de tipo non-fast forward**
    1. Publica `main` en tu repo de GitHub


# EJERCICIO_2 (2,25 puntos)

- Accede a GitHub Classroom e inicia el ejercicio 2: https://classroom.github.com/a/fhGUFAQA

- Clona en tu PC el repositorio del ejercicio 2 que se ha creado en el paso anterior y realiza en tu ordenador los siguiente pasos.

- Crea un proyecto en Java llamado `Ejercicio2` con una clase con nombre `EdadLegal` que contiene un método 

   `public boolean canDriveACar(int age, String country)`

que toma cómo parámetros un númer entero, `age` (edad) y una cadena, `country` (pais), y devuelve `true` la persona con esa edad es puede condicir legalmente un coche en ese pais, según la siguiente tabla:

| pais | edad | ¿Puede conducir un coche? | 
|----------|----------|----------|
| España y Polonia | desde los 18 años |  si |
| USA y Canada | desde los 16  años  |  si  |
| UK | desde los 17  años  |  si  |

- Además ten en cuenta que el método `canDriveACar` devuelve `false` para edades negativas y para paises que no estén en la tabla anterior. 

- Implementa los casos de prueba necesarios utilizando *JUnit 5* con tests parametrizados, y si es posible, con carga de datos desde un archivo `.csv` para obtener un 100% de cobertura del código del método `isDateCorrect`, usando los valores límite adecuados donde proceda. 

- **Publica tus cambios** en el **repositorio** privado de este ejercicio.

- Crea en Jenkins un proyecto de tipo **pipeline** que construya el proyecto java `Ejercicio2`: compilando los fuentes y ejecutando los tests. Para esto será necesario que el proyecto esté *mavenizado*.

- Publica en Jenkins los resultados de los test y de cobertura de código.

- Genera los Javadoc en una nueva fase del pipeline, y publicalos en Jenkins.

- Añade la siguiente dependencia al `pom.xml` y genera los resultados de Dependency Check en una nueva fase del pipeline, y publicalos en Jenkins.

````xml
  <dependency>
    <groupId>log4j</groupId>
    <artifactId>log4j</artifactId>
    <version>1.2.17</version>
  </dependency>
````

- **Para entregar el ejercicio**: en tu archivo personal con extensión `.md` indica: 
  - el **repositorio** donde has resuelto este Ejercicio 2, 
  - el enlace a Jenkins y el **nombre del proyecto Jenkins** donde has resuelto este Ejercicio 2.
  - añade también varias capturas de pantalla del proyecto Jenkins.  
  - Envía tu archivo `.md` y las imágenes a este repositorio.


## EJERCICIO3 (0,75 puntos)


Realiza con Selenium IDE las pruebas necesarias para verificar la funcion **add to cart** para el usuario `standard_user` con contraseña `secret_sauce` en la web https://www.saucedemo.com/. Para ello: 

* Crea todos los tests que consideres necesarios para verificar qué productos **se añaden** correctamente al carrito al hacer click en **add to cart**.

* Guarda los tests con tu nombre de usuario de la UAL y extensión `.side`. 
En el mismo repositorio privado del Ejercicio2 crea una carpeta llamada `Selenium` y guarda ahí el `.side`.

* En esa misma carpeta `Selenium` guarda  una captura de pantalla de los resultados de la ejecución de los tests en Selenium IDE. 

* Por último, añade a tu pagina `.md` un texto con el nombre del archivo `.side`. No olvides hacer la entrega del ejercicio.
