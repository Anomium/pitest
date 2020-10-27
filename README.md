# Pitest 🚀
## ¿Que es Pitest?
Pitest es un modificador de codigo, que verifica el buen funcionamiento de los test unitarios.
Modifica operadores logicos, aritmeticos, valores retornados.. con la finalidad de detectar el buen funcionamiento de los test, pero ¿como verifica esto? Pitest modifica y luego ejecuta el test unitario, en caso de que el test unitario salga mal es porque nuestro test esta bien hecho y en caso contrario el test unitario sigue saliendo bien pues tendremos que verificar el test debido a que le falta validar algo que no hemos tenido en cuenta.

### Instalación Basica 🔧
Añadir el plugin al pom.xml dentro de la etiqueta ```<plugins>``` 
```
<plugin>
  <groupId>org.pitest</groupId>
  <artifactId>pitest-maven</artifactId>
  <version>1.4.9</version>
</plugin>
```
Comando para ejecutar pitest en el cmd ```mvn org.pitest:pitest-maven:mutationCoverage```
A los cambios que genera pitest se le llaman  Mutantes/Mutaciones.
* Si las pruebas pasan al ejecutarse sobre el mutante, el mutante sobrevive.
* Si las pruebas no pasan al ejecutarse sobre el mutante, el mutante muere

El objetivo es que todos los mutantes mueran, así podremos decir que el test responde a la definición concreta del código y que lo prueba correctamente.

![Imagen de ejecucion del comando](https://github.com/Anomium/pitest/blob/main/img/mutators.PNG)



