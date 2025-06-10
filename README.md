<div align="center">
  
<h1 align="center">Laboratorio 1 de Arquitectura de Software (ARSW)</h1>

<p align="center">
Manejo basico de Maven con Java y uso correcto de Git y Github
</p>

</div>

</br>


## Antes de comenzar

En primer lugar, es importante tener en cuenta que las herramientas Maven y Git ya se encuentran instaladas y configuradas en el sistema. Se asume que estos son prerrequisitos preexistentes en el dispositivo, por lo que no se abordará su proceso de instalación.

![versions](/docs/i)


</br>
</br>

## Creacion del proyecto

Para inicializar un nuevo proyecto, simplemente se debe ejecutar un único comando. Este se encargará de generar automáticamente toda la estructura de directorios y archivos necesarios para comenzar. Dando como resultado el siguiente proceso:

```sh
mvn archetype:generate -DgroupId=edu.escuelaing.arsw.ASE.app -DartifactId=mi-primera-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

cd mi-primera-app
```

![initial](/docs/initial.jpeg)

Podemos validar la creacion del proyecto usando el comando `tree` en nuestra consola:

![tree](/docs/tree.jpeg)


</br>
</br>

## Construccion del proyecto

Se finalizó la etapa de construcción y ejecución del proyecto. Se corrió el comando mvn package, el cual completó el ciclo de vida de Maven hasta la fase de empaquetado, generando el archivo .jar en el directorio target. Posteriormente, se ejecutó dicho artefacto, verificando su funcionamiento con el resultado "Hello World!" esperado.

```sh
java -cp target/mi-primera-app-1.0-SNAPSHOT.jar edu.escuelaing.arsw.ASE.app.App
```


![Run](/docs/run.jpeg)


</br>
</br>

## Instalacion de plugins y dependencias

En nuestro proyecto, tenemos un archivo llamado POM.xml, el cual nos permite añadir plugins y dependencias, de modo que es posible añadir funcionalidades específicas a nuestro proyecto. En este caso, se coloca un plugin de documentación automática como ejemplo.

![pom](/docs/pom.jpeg)

Podemos validar el funcionamiento volviendo a construir el proyecto con el comando `mvn clean package`, recordando que se pueden ejecutar de forma secuencial los ciclos de vida en Maven.

![Run](/docs/runmvn.jpeg)

![Doc](/docs/doc.png)

</br>
</br>

## Primeros pasos en Git

Para poder registrar la autoría en cada commit, es fundamental configurar la identidad en Git. Esto se logra estableciendo el nombre de usuario y el correo electrónico de forma global, asegurando que toda contribución quede correctamente atribuida.

```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

resultado es el siguiente, donde apreciamos la configuracion de nuestro git en caso de usar el comando `git config`.

![conf](/docs/conf.jpeg)


</br>
</br>

## Trabajando con git

The exams are designed to assess my individual technical skills, not those of my teammates. Each exam was designed to ensure that the student was not dependent on others and had full knowledge of the subject matter.
- Exam 1: Use Maven, SpringBoot and pattern desings to create a little app without REST.
- Exam 2: Little REST app with deploy and basic interfaz with React.
- Exam 3: Same of second exam, but larger and focuses on architecture desings.

</br>
</br>


## License
Distributed under the GPL-3.0 License. See `LICENSE.txt` for more information.
