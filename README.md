<style>
.retorno-menu {
  display: inline-block;
  background-color: #007bff;
  color: white;
  padding: 10px 20px; 
  border-radius: 5px;
  border: 1px solid #007bff; 
  text-decoration: none;
}
 .retorno-menu:hover {
  background-color: #0056b3;
  border-color: #0056b3;
}
</style>

# Java-Zero-To-Hero
Repositorio para notas y ejercicios del Boot Camp 'Zero to Hero' impartido por la comunidad oficial de JAVA. 

## Menu de ejercicios 

* #### Errores del compilador y de ejecución
  * [Ir a Ejercicio 1](#ejercicio-1)
  * [Ir a Ejercicio 2](#ejercicio-2)
  * [Ir a Ejercicio 3](#ejercicio-3)
  * [Ir a Ejercicio 4](#ejercicio-4)
  * [Ir a Ejercicio 5](#ejercicio-5)
  * [Ir a Ejercicio 6](#ejercicio-6)
* #### Ejercicios de codificación
  * [Ir a Ejercicio 7](#ejercicio-7---adivina-la-pelicula)
  * [Ir a Ejercicio 8](#ejercicio-8---llenado-de-caracteres)
  * [Ir a Ejercicio 9](#ejercicio-9)
  * [Ir a Ejercicio 10](#ejercicio-10)
  * [Ir a Ejercicio 11](#ejercicio-11)
* ### Ejercicios de corrección de código
  * [Ir a Ejercicio 12](#ejercicio-12)
  * [Ir a Ejercicio 13](#ejercicio-13)

## Errores del compilador y de ejecución

## Ejercicio 1

```java
err1(){
  return "Donde esta el error?"
}
```
Al crear la función en jshell se obtiene el siguiente error:

<div align='center'>
<img width="427" height="242" alt="image" src="https://github.com/user-attachments/assets/d363109c-16a2-4230-b556-294e3c99d2b6" />
</div>

El error se debe que se no se declaró el tipo de retorno de la función. A continuación, se muestra la corrección:
```java
String err1(){
  return "Donde esta el error?"
}
```

<div align='center'>
<img width="403" height="91" alt="image" src="https://github.com/user-attachments/assets/ecc80878-7609-4d63-8c00-51d613519947" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios" class="retorno-menu">Regresar al menú</a>
</div>

## Ejercicio 2

```java
string err2(){
  return "String o string?"
}
```
Al crear la función se obtiene el siguiente error:

<div align='center'>
<img width="815" height="108" alt="image" src="https://github.com/user-attachments/assets/654d22a7-52ae-4fb6-a580-9b00a74c9284" />
  <img width="309" height="130" alt="image" src="https://github.com/user-attachments/assets/a32303f7-1a9f-48a8-81a9-34d37999e2c9" />
</div>

El error se debe a que en java la declaración de los tipos de salida es sensible al uso de mayusculas o minusculas, al tener el tipo de dato como "string" en lugar de "String" no lo reconoce. A continuación se muestra la corrección:

```java
String err2(){
  return "String o string?"
}
```
<div align='center'>
  <img width="373" height="148" alt="image" src="https://github.com/user-attachments/assets/db18c092-0e78-4895-ae85-fe2cc22452df" />
</div>

## Ejercicio 3

```java
String err3(who){
  return String.format("%s, cual es el error?",who);
}
```

Al crear la funcion se obtiene el siguiente error:

<div align='center'>
  <img width="577" height="149" alt="image" src="https://github.com/user-attachments/assets/b70af088-8161-46d3-9d0c-1de9bb733307" />
</div>

Este error ocurre debido a que no se indico el tipo de dato que recibira la función como parametro. A continuación se muestra la corrección:

```java
String err3(String who){
  return String.format("%s, cual es el error?",who);
}
```
<div align='center'>
<img width="581" height="153" alt="image" src="https://github.com/user-attachments/assets/a78c543e-f3e2-45ca-a157-1de11607cc01" />
</div>

## Ejercicio 4

```java
String err4(){
  return "Este es un error sutil"
}
```

Al crear la función se obtiene el siguiente error:

<div align='center'>
  <img width="430" height="150" alt="image" src="https://github.com/user-attachments/assets/612b8123-aaf1-4174-936f-fcb44f77de8c" />
</div>

En este error se nos indica la ausencia del ";" por lo cual el compilador no puede determinar donde termina la sentencia. A continuación, se muestra la corrección:

```java
String err4(){
  return "Este es un error sutil";
}
```
<div align='center'>
  <img width="452" height="151" alt="image" src="https://github.com/user-attachments/assets/efff99fb-56d6-44e5-aa04-d63eb25a4a98" />
</div>

## Ejercicio 5

```java
String err5(){
  "Es un poco menos sutil";
}
```

Al crear esta función obtenemos el siguiente error:

<div align='center'>
  <img width="459" height="226" alt="image" src="https://github.com/user-attachments/assets/1be78b0e-c2fd-45d4-984f-cf35a92a9a11" />
</div>

El error nos indica que una cadena de texto como tal no es una sentencia, para considerarse como una debe tener sentencias como return, asignaciones, etc. Una literal por si misma no es ejecutable. En la segunda parte el error nos indica que no tiene una sentencia return, en la declaración del tipo de retorno le indicamos a la función que debe devolver un string pero al no tener una sentencia de retorno esto provoca un error. A continuación, se muestra la corrección:

```java
String err5(){
  return "Es un poco menos sutil";
}
```

<div align='center'>
  <img width="459" height="155" alt="image" src="https://github.com/user-attachments/assets/91930898-1e54-4f52-8779-b81457f339e1" />
</div>

## Ejercicio 6

```java
String err6{
  return "Hola error!";
}
```

Al crear la función tenemos el siguiente error:

<div align='center'>
  <img width="349" height="150" alt="image" src="https://github.com/user-attachments/assets/b4bfcd25-7de3-4a3e-ae03-fa36f9256099" />
</div>

Este error se debe a que no se tienen los parentesis de la lista de parametros, aunque una función no reciba ningún parametro, los parentesis deben existir o de lo contrario los compiladores lo interpretaran como un error de sintaxis. A continuación, se muestra la corrección:

```java
String err6(){
  return "Hola error!";
}
```

<div align='center'>
  <img width="349" height="155" alt="image" src="https://github.com/user-attachments/assets/1ea24a01-5050-4839-927c-aea7b6809c25" />
</div>

## Ejercicios de codificación

## Ejercicio 7 - Adivina la pelicula 

Este ejercicio requiere crear una función que reciba 3 emojis y los devuelva a la salida entre parentesis separados por una coma. El código para la función sería el siguiente:

```java
String adivinaLaPelicula(String emoji1, String emoji2, String emoji3){
  return String.format("[%s,%s,%s]",emoji1,emoji2,emoji3);
}
```

Como se puede observar la función se crea correctamente, recibe los emojis en la función y los muestra al final en el formato esperado. Los emojis no se muestran correctamente a la salida por temas de la terminal de Windows, pero la funcion es correcta.

<div align='center'>
  <img width="724" height="153" alt="image" src="https://github.com/user-attachments/assets/970facfd-ccdb-4355-b44c-81c03b10c5f2" />
</div>

## Ejercicio 8 - Llenado de caracteres

Este ejercicio requiere crear una función que sea capaz de insertar un caracter en la posición deseada dentro de una cadena de texto fija. El código para esta función sería el siguiente:

```java
String konnichiwa(String dare){
  return String.format("こんにちは%s",dare);
}
```

Como se puede observar a continuación la función se crea sin problemas y funciona correctamente, dado el parametro "D" lo concateno con la cadena declarada dentro de la función. De igual forma la terminal de Windows no reconoce correctamente los caracteres en japones pero la función es correcta.

<div align='center'>
  <img width="545" height="143" alt="image" src="https://github.com/user-attachments/assets/4a739c48-a206-4e8a-aaa0-cc42123262ab" />
</div>

## Ejercicio 9 

Este ejercicio requiere crear una función que devuelva el separador "<<<>>>". A continuación, se muestra el código para esta función:

```java
String separador(){
  return "<<<>>>";
}
```

Como se muestra a continuación la función se crea correctamente y devuelve el valor deseado.

<div align='center'>
  <img width="300" height="152" alt="image" src="https://github.com/user-attachments/assets/b57fa1b8-ddb4-4d68-9a33-ab95fb67f2ef" />
</div>

## Ejercicio 10

Este ejercicio requiere crear una función que devuelva las vocales "aeiou". A continuación, se muestra el código para esta función:

```java
String vocales(){
  return "aeiou";
}
```

Como se muestra a continuación la función se crea correctamente y devuelve el valor deseado.

<div align='center'>
  <img width="279" height="138" alt="image" src="https://github.com/user-attachments/assets/3e49ac44-6a79-4018-b448-5c4d51c735b2" />
</div>

## Ejercicio 11

Este ejercicio requiere crear una función que adorne un string devolviendolo entre "<<< >>>". A continuación se muestra el código para esta función:

```java
String tituloAdornado(String texto){
  return String.format("<<< %s >>>",texto);
}
```

Como se muestra a continuación la función se crea correctamente y devuelve el valor deseado. Para este ejercico se pidio realizar tres ejemplos. 

<div align='center'>
  <img width="512" height="261" alt="image" src="https://github.com/user-attachments/assets/c49a649a-74d3-445d-b9fe-d07ac31dc31d" />
</div>


## Ejercicios de corrección de código

Para estos ejercicios se brinda un codigo que contiene un error, se debe verificar la función y corregir para que devuelva la salida esperada.

## Ejercicio 12 

Este ejercicio requiere que la función reciba una frase y devuelva el valor entre "<= =>". El código dado es el siguiente:

```java
String adornar(String frase){
  return String.format("<=%s=>, frase");
}
```

Como se observa a continuación, la función se crea correctamente pero al utilizarla esta muestra un error.

<div align='center'>
<img width="691" height="235" alt="image" src="https://github.com/user-attachments/assets/40fc94b6-a218-4f99-9458-5d6ab6b050b7" />
</div>

Este error se debe a que la sintaxis dada para String.format no es correcta, debido a que en el código erreoneo el parametro frase se encuentra dentro de la cadena texto es tomada como tal y no reconoce ningún valor que sustituir en el marcador de posición (%s), debería ser como a continuación se muestra:

```java
String adornar(String frase){
  return String.format("<=%s=>", frase);
}
```

Una vez corregida podemos observar que la función ya no muestra ningún error al ejecutarla y devuelve los valores esperados.

<div align='center'>
<img width="489" height="201" alt="image" src="https://github.com/user-attachments/assets/b26ed52b-9738-4c3b-9eb2-c34d6b0d3e16" />
</div>

## Ejercicio 13 

Este ejercicio requiere que la función reciba dos parametros y los muestre concatenados a la salida. El código dado es el siguiente:

```java
String concatenar(String s1, String s2){
  return String.format("[%s+%s]", s2, s1);
}
```

Las salidas esperadas para esta función son:

<div align='center'>
  <img width="649" height="87" alt="image" src="https://github.com/user-attachments/assets/de2492d5-1798-4a5f-ac43-608ac6fb41bc" />
</div>

Probando la función se crea correctamente pero la salida no es la esperada:

<div align='center'>
  <img width="502" height="100" alt="image" src="https://github.com/user-attachments/assets/12f3d6e1-1bcb-4b74-923e-8af7aeafcc1d" /> <br>
  <img width="342" height="64" alt="image" src="https://github.com/user-attachments/assets/fd3ad4d1-d3e3-410d-80c1-0ec791ae11f2" />
</div>

Esto más que un error se puede considerar como una confución por parte del desarrollador de la función, ya que, invirtió las posiciones de los parametros de entrada y por ello devuelve un valor diferente al esperado. La función debe ser como a continuación se muestra:

```java
String concatenar(String s1, String s2){
  return String.format("[%s+%s]", s1, s2);
}
```

Con esta pequeña corrección se obtienen las salidas esperadas:

<div align='center'>
  <img width="533" height="205" alt="image" src="https://github.com/user-attachments/assets/0b2bdef6-3d27-4e57-a126-fc4234410c53" />
</div>

