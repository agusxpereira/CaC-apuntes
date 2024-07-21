//22:42 
https://www.youtube.com/watch?v=cpyKnUZnrCQ&list=PLMBLJyhQOSWwgSnlZfmLK-yo4_2YeYvty&index=35&ab_channel=CaCJava 


Instalamos el server community manager, el java pack de microsoft y el de redhat 


En el archivo pom es dónde vamos a trabajar con las dependencias. En ella vamos a insatalar el maven sql (el mismo archivo que descargamos en las clases anteriores para hacer las cosnultas) aparte de otros: 

```xml
  <dependencies>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.11</version>
      <scope>test</scope>
    </dependency>

    <!-- https://mvnrepository.com/artifact/mysql/mysql-connector-java -->
  <dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>8.0.31</version>
  </dependency>
  <!-- https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-core -->
<!-- https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-databind -->
<dependency>
    <groupId>com.fasterxml.jackson.core</groupId>
    <artifactId>jackson-databind</artifactId>
    <version>2.13.0</version>
</dependency>
<!-- https://mvnrepository.com/artifact/javax.servlet/javax.servlet-api -->
<dependency>
    <groupId>javax.servlet</groupId>
    <artifactId>javax.servlet-api</artifactId>
    <version>4.0.1</version>
    <scope>provided</scope>
</dependency>
<!-- https://mvnrepository.com/artifact/javax.servlet.jsp/javax.servlet.jsp-api -->
<dependency>
    <groupId>javax.servlet.jsp</groupId>
    <artifactId>javax.servlet.jsp-api</artifactId>
    <version>2.3.3</version>
    <scope>provided</scope>
</dependency>


  </dependencies>
```
Ahora vamos a configurar los plugins: 

```xml
<!--Plugin para compilar codigo fuente-->
        <plugin>
          <groupId>org.apache.maven.plugins</groupId>
          <artifactId>maven-compiler-plugin</artifactId>
          <version>3.8.0</version>
          <configuration>
            <source>22</source>
            <target>22</target>
          </configuration>
        </plugin>

        <!--Plugin para empaquetar la version como war--> 
        <plugin>
          <groupId>org.apache.maven.plugins</groupId>
          <artifactId>maven-war-plugin</artifactId>
          <version>3.3.1</version>
          <configuration>
            <failOnMissingWebXml>false</failOnMissingWebXml>
          </configuration>
        </plugin>

``` 

Esto sirve para levantar el proyecto [44:22]