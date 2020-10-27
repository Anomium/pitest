# Pitest 🚀
## ¿Que es Pitest?
_Pitest es un modificador de codigo, que verifica el buen funcionamiento de los test unitarios._
_Modifica operadores logicos, aritmeticos, valores retornados.. con la finalidad de detectar el buen funcionamiento de los test, pero ¿como verifica esto? Pitest modifica y luego ejecuta el test unitario, en caso de que el test unitario salga mal es porque nuestro test esta bien hecho y en caso contrario el test unitario sigue saliendo bien pues tendremos que verificar el test debido a que le falta validar algo que no hemos tenido en cuenta._

### Instalación Basica 🔧
_Añadir el plugin al pom.xml dentro de la etiqueta ```<plugins>``` _
```
<plugin>
  <groupId>org.pitest</groupId>
  <artifactId>pitest-maven</artifactId>
  <version>1.4.9</version>
</plugin>
```
Comando para ejecutar pitest en el cmd ```mvn org.pitest:pitest-maven:mutationCoverage```

