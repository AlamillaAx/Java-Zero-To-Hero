# Java-Zero-To-Hero
Repositorio para notas y ejercicios del Boot Camp 'Zero to Hero' impartido por la comunidad oficial de JAVA. 

## Menu de ejercicios 

* #### Fundamentos - Errores del compilador y de ejecución
  * [Ir a Ejercicio 1.1](#ejercicio-11)
  * [Ir a Ejercicio 1.2](#ejercicio-12)
  * [Ir a Ejercicio 1.3](#ejercicio-13)
  * [Ir a Ejercicio 1.4](#ejercicio-14)
  * [Ir a Ejercicio 1.5](#ejercicio-15)
  * [Ir a Ejercicio 1.6](#ejercicio-16)
* ### Fundamentos - Ejercicios de codificación
  * [Ir a Ejercicio 1.7](#ejercicio-17---adivina-la-pelicula)
  * [Ir a Ejercicio 1.8](#ejercicio-18---llenado-de-caracteres)
  * [Ir a Ejercicio 1.9](#ejercicio-19)
  * [Ir a Ejercicio 1.10](#ejercicio-110)
  * [Ir a Ejercicio 1.11](#ejercicio-111)
* ### Fundamentos - Ejercicios de corrección de código
  * [Ir a Ejercicio 1.12](#ejercicio-112)
  * [Ir a Ejercicio 1.13](#ejercicio-113)
* ### Operadores - Errores del compilador y de ejecución
  * [Ir a Ejercicio 2.1](#ejercicio-21)
  * [Ir a Ejercicio 2.2](#ejercicio-22)
  * [Ir a Ejercicio 2.3](#ejercicio-23)
* ### Operadores - Ejercicios de codificación
  * [Ir a Ejercicio 2.4](#ejercicio-24)
  * [Ir a Ejercicio 2.5](#ejercicio-25)
  * [Ir a Ejercicio 2.6](#ejercicio-26)
  * [Ir a Ejercicio 2.7](#ejercicio-27)
  * [Ir a Ejercicio 2.8](#ejercicio-28)
  * [Ir a Ejercicio 2.9](#ejercicio-29)
  * [Ir a Ejercicio 2.10](#ejercicio-210)
  * [Ir a Ejercicio 2.11](#ejercicio-211)
  * [Ir a Ejercicio 2.12](#ejercicio-212)
  * [Ir a Ejercicio 2.13](#ejercicio-213)
  * [Ir a Ejercicio 2.14](#ejercicio-214)
* ### Operadores - Ejercicios de corrección de código
  * [Ir a Ejercicio 2.15](#ejercicio-215)
* ### Variables - Errores de compilador y de ejecución
  * [Ir a Ejercicio 3.1](#ejercicio-31)
* ### Variables - Ejercicios de códificación
  * [Ir a Ejercicio 3.2](#ejercicio-32)
  * [Ir a Ejercicio 3.3](#ejercicio-33)
  * [Ir a Ejercicio 3.4](#ejercicio-34)
  * [Ir a Ejercicio 3.5](#ejercicio-35)
  * [Ir a Ejercicio 3.6](#ejercicio-36)
  * [Ir a Ejercicio 3.7](#ejercicio-37)
  * [Ir a Ejercicio 3.8](#ejercicio-38)
  * [Ir a Ejercicio 3.9](#ejercicio-39)
  * [Ir a Ejercicio 3.10](#ejercicio-310)
* ### Variables - Ejercicios de corrección de código
  * [Ir a Ejercicio 3.11](#ejercicio-311)
* ### Strings - Errores del compilador y del tiempo de ejecución.
* ### Strings - Ejercicios de códificación.
* ### Strings - Ejercicios de corrección de código.
  
## Errores del compilador y de ejecución

El objetivo de estos ejercicios es visualizar los errores que arroja cada función al intentar crearlas, entender el error y corregirlo para que funcione correctamente. 

## Ejercicio 1.1

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
<a href="#menu-de-s">Regresar al menú</a>
</div>

## Ejercicio 1.2

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.3

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.4

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.5

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.6

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicios de codificación

El objetivo de estos ejercicios es desarrollar una función desde cero teniendo solamente las salidas deseadas para cada una.

## Ejercicio 1.7 - Adivina la pelicula 

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.8 - Llenado de caracteres

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.9 

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.10

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

## Ejercicio 1.11

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>


## Ejercicios de corrección de código

Para estos ejercicios se brinda un codigo que contiene un error, se debe verificar la función y corregir para que devuelva la salida esperada.

## Ejercicio 1.12 

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 1.13 

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Operadores - Errores del compilador y de ejecución

En estos ejercicios observaremos los errores más comunes durante el uso de operadores así como la solución para cada uno de ellos. 

## Ejercicio 2.1

Este ejercicio requiere crear una función para realizar una multiplicación.

```java
int multiplicacion(String numero1, String numero2) {
  return numero1 * numero2;
}
```

Al crear la función se visualiza el siguiente error, el cual indica que no se puede utilizar un operador de multiplicación con datos de tipo cadena o string. 

<div align='center'>
  <img width="571" height="189" alt="image" src="https://github.com/user-attachments/assets/9b6633c7-b518-48b9-a6ef-55175ccf4c4b" />
</div>

Al corregir el tipo de dato de los parametros de entrada observamos que la función se crea sin inconvenientes y es utilizable.

```java
int multiplicacion(int numero1, int numero2) {
  return numero1 * numero2;
}
```
<div align='center'>
<img width="524" height="149" alt="image" src="https://github.com/user-attachments/assets/4f238560-9ebb-4819-881e-6eb61fabbadc" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.2

Este ejercicio requiere crear una función para realizar una suma

```java
int suma(int numero1, int numero2) {
  return + numero1 numero2;
}
```

Al crear la función se visualiza el siguiente error, el cual nos indica que la posición del operador suma no es la correcta, ya que debe estar entre los numeros a operar para funcionar correctamente.

<div align='center'>
  <img width="431" height="225" alt="image" src="https://github.com/user-attachments/assets/1b8b8666-e50d-45d5-802e-f28d8a7798e0" />
</div>

Al corregir la posición del operador observamos que la función se crea sin inconvenientes y es utilizable.

```java
int suma(int numero1, int numero2) {
  return numero1 + numero2;
}
```
<div align='center'>
<img width="415" height="151" alt="image" src="https://github.com/user-attachments/assets/bc5fc641-8c5f-409c-b3d1-274da4513487" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.3

Este ejercicio requiere crear una función para realizar la comparación de un valor con respecto a otros dados.

```java
boolean positivoMenorDe20(int numero) {
  return numero > 0 && <20;
}
```

Al crear la función se visualiza el siguiente error, el cual nos indica que hace falta el parametro a comprar en esa parte de la función.

<div align='center'>
  <img width="438" height="145" alt="image" src="https://github.com/user-attachments/assets/3ef18d49-09b0-4a5a-b732-fde089198969" />
</div>

Al agregar el parametro en la comparación observamos que la función se crea sin inconvenientes y es utilizable.

```java
boolean positivoMenorDe20(int numero) {
  return numero > 0 && numero < 20;
}
```
<div align='center'>
<img width="450" height="210" alt="image" src="https://github.com/user-attachments/assets/a82be13c-7bc6-4192-9624-7aa397c54c60" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Operadores - Ejercicios de codificación.

## Ejercicio 2.4

Este ejercicio requiere crear una función para que retorne el numero dado sin su último dígito. Los escenarios esperados son los siguientes:

<div align='center'>
<img width="647" height="96" alt="image" src="https://github.com/user-attachments/assets/85f9ff69-7729-4532-ae33-6da07d040536" />
</div>

Con el siguiente código se satisface lo requerido:

```java
int truncado(int n) {
  return n / 10;
}
```

<div align='center'>
  <img width="373" height="207" alt="image" src="https://github.com/user-attachments/assets/7f36aedf-d261-4dfb-9a1d-374b89f40ebb" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.5

Este ejercicio requiere crear una función para que retorne el ultimo digito del numero dado. Los escenarios esperados son los siguientes:

<div align='center'>
<img width="638" height="90" alt="image" src="https://github.com/user-attachments/assets/dbf20d59-842e-487a-9543-18593c292fac" />
</div>

Con el siguiente código se satisface lo requerido:

```java
int ultimoDigito(int n) {
  return n % 10;
}
```

<div align='center'>
  <img width="371" height="322" alt="image" src="https://github.com/user-attachments/assets/c2140f75-c3c7-480a-9400-06c63e5fe58b" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.6

Este ejercicio requiere crear una función que dado un número entero, devuelva verdadero si el número esta dentro del rango de 0 a 9 y falso de lo contrario. Los resultados esperados son los siguientes:

<div align='center'>
<img width="649" height="134" alt="image" src="https://github.com/user-attachments/assets/eefc1ec7-420e-41c6-a3b9-243838030bc7" />
</div>

Con el siguiente código se satisface lo requerido:

```java
boolean unicoDigito(int n) {
 return (n >= 0) && (n < 10);
}
```

<div align='center'>
  <img width="377" height="311" alt="image" src="https://github.com/user-attachments/assets/c088027a-9ce4-4edb-ba1f-ecabbab3ac94" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.7

Este ejercicio requiere crear una función que dado un número entero, devuelva el string "no-negativo" si es positivo o cero, o "negativo" si es negativo.

Con el siguiente código se satisface lo requerido:

```java
String signo(int n) {
 return (n >= 0) ? "no-negativo":"negativo";
}
```

<div align='center'>
  <img width="514" height="215" alt="image" src="https://github.com/user-attachments/assets/32e432ae-cdec-4b4f-92f1-ea6db7097d34" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.8

Este ejercicio requiere crear una función que verifique si un número es par. 

Con el siguiente código se satisface lo requerido:

```java
boolean esPar(int n) {
 return (n % 2) == 0;
}
```

<div align='center'>
  <img width="321" height="221" alt="image" src="https://github.com/user-attachments/assets/d46d3668-072f-4b03-9052-c54cabe16d13" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.9

Este ejercicio requiere crear una función que verifique si un número es impar.

Con el siguiente código se satisface lo requerido:

```java
boolean esImpar(int n) {
 return (n % 2) != 0;
}
```

<div align='center'>
<img width="347" height="320" alt="image" src="https://github.com/user-attachments/assets/8a51305d-c711-42c3-b0e1-4c72bc249573" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.10

Este ejercicio requiere crear una función que tome dos números enteros y devuelva el resultado de a2 - b2. Los resultados esperados son los siguientes:

<div align='center'>
<img width="668" height="60" alt="image" src="https://github.com/user-attachments/assets/545993af-9ebf-4e95-9f27-82f59969ad97" />
<img width="649" height="50" alt="image" src="https://github.com/user-attachments/assets/d8b58067-a185-4f69-add7-b408e746ef8a" />
</div>

Con el siguiente código se satisface lo requerido:

```java
int diferenciaDeCuadrados(int a, int b) {
 return (a * a) - (b * b);
}
```

<div align='center'>
<img width="457" height="205" alt="image" src="https://github.com/user-attachments/assets/5005aa76-9124-467d-9b4a-0873eca0a7eb" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.11

Este ejercicio requiere crear una función que tome dos doubles que representan la medida de dos ángulos de un triangulo y devuelva la medida del tercero. Los resultados esperados son los siguientes:

<div align='center'>
<img width="650" height="82" alt="image" src="https://github.com/user-attachments/assets/a000b129-eb8e-4ffe-9a9b-1622da1c2ddf" />
</div>

Con el siguiente código se satisface lo requerido:

```java
double tercerAngulo(double a, double b) {
 return 180 - (a + b);
}
```

<div align='center'>
<img width="468" height="260" alt="image" src="https://github.com/user-attachments/assets/c623fce2-a43d-43be-b917-e9b27b9aa82c" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.12

Este ejercicio requiere crear una función que tome un entero y devuelva un predicado que sea verdadero si es un múltiplo positivo de siete menor que 1000. Los resultados esperados son los siguientes:

<div align='center'>
<img width="642" height="100" alt="image" src="https://github.com/user-attachments/assets/3bcd8bb5-3d6e-4178-a0ed-1c61c986d884" />

</div>

Con el siguiente código se satisface lo requerido:

```java
boolean validarMultiploDe7(int n) {
 return (n % 7) == 0 && (n > 0) && n < 1000);
}
```

<div align='center'>
<img width="569" height="320" alt="image" src="https://github.com/user-attachments/assets/c07fa1f2-e369-4055-b0b4-cac9ac3627e4" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.13

Este ejercicio requiere crear una función que tome tres números enteros: inicio, mitad y tamaño, debe retornar verdadero si "inicio" es mayor o igual a 0, "inicio" es menor que "mitad" y "mitad" es menor que tamaño. Los resultados esperados son los siguientes:

<div align='center'>
<img width="641" height="121" alt="image" src="https://github.com/user-attachments/assets/e21b97d6-9794-4de5-88a7-7274290e8ee0" />
</div>

Con el siguiente código se satisface lo requerido:

```java
boolean validar(int inicio, int mitad, int tamano) {
 return (inicio >= 0) && (inicio < mitad) && (mitad < tamano);
}
```

<div align='center'>
<img width="678" height="369" alt="image" src="https://github.com/user-attachments/assets/3996d2e7-a5f6-44e9-bac2-5490734e995d" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 2.14

Este ejercicio requiere crear una función para el cobro de un parqueadero que abre de 8:00 am a 6:00 pm, su sistema de cobro es el siguiente: el usuario debe pagar $10.0 por cada minuto de parqueo, pero tiene un cobro minimo de $100.0 y un maximo de $3000.0. Los resultados esperados son los siguientes:

<div align='center'>
<img width="646" height="122" alt="image" src="https://github.com/user-attachments/assets/0b4ba59a-3603-4bd6-b4b2-8c6ed5ef0877" />
</div>

Con el siguiente código se satisface lo requerido:

```java
double cobro(int minutos) {
 double total = minutos * 10;
 return  Math.min(3000.0,Math.max(100.0,total));
}
```

<div align='center'>
<img width="525" height="394" alt="image" src="https://github.com/user-attachments/assets/1d4d5312-894b-4b5e-9525-31d9241ba462" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Operadores - Ejercicios de corrección de código.

## Ejercicio 2.15

Este ejercicio requiere realizar la corrección de una función. Los resultados esperados son los siguientes:

<div align='center'>
<img width="648" height="144" alt="image" src="https://github.com/user-attachments/assets/450ca4e9-c7d3-4861-9d7c-25bdcca273dd" />
</div>

La función dada es la siguiente:

```java
int inicio(int resultados, int pagina) {
 return (resultados * pagina) - 1;
}
```

Y actualmente muestra resultados erroneos:

<div align='center'>
<img width="453" height="318" alt="image" src="https://github.com/user-attachments/assets/aeef08d0-a7a5-4167-9fb2-5614784fb3bf" />
</div>

Con base en los resultados esperados podemos deducir que la operación que se pretende es obtener es la siguiente: resultados * pagina / resultados. 

```java
int inicio(int resultados, int pagina) {
 return (resultados * pagina) - resultados;
}
```

Con esta modificación observamos que ahora se obtienen los resultados esperados:

<div align='center'>
<img width="555" height="313" alt="image" src="https://github.com/user-attachments/assets/fb62718f-957a-4e90-9dd1-f4dc6191870e" />

</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Variables - Errores de compilador y en tiempo de ejecución.

## Ejercicio 3.1

Este ejercicio requiere verificar y solucionar el error de compilación que nos da el código dado.

La función dada es la siguiente:

```java
int duplicar(double a) {
 var foo = a * 2;
 return foo;
}
```

El código genera el siguiente error al ser compilado, esto se debe a que en la operación que genera, var infiere que se trata de un double pero la función fue declarada para devolver un valor del tipo int. 

<div align='center'>
<img width="630" height="167" alt="image" src="https://github.com/user-attachments/assets/a3d66080-5e63-4f55-8a89-de06633b55c9" />
</div>

Realizando la correción del tipo de dato a retornar observamos que el error se corrigue y la función ahora es utilizable.

```java
double duplicar(double a) {
 var foo = a * 2;
 return foo;
}
```

Con esta modificación observamos que ahora se obtienen los resultados esperados:

<div align='center'>
 <img width="367" height="170" alt="image" src="https://github.com/user-attachments/assets/b710ecb1-98b7-4a4e-9dee-5066e9dc87a1" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Variables - Ejercicios de codificación.

## Ejercicio 3.2

Este ejercicio requiere crear una función que calcule el modulo de una división. Los valores esperados de salida con los siguientes:

<div align='center'>
<img width="648" height="81" alt="image" src="https://github.com/user-attachments/assets/de88492c-9d14-4b21-b63a-448a83cb66c2" />
</div>

Con la siguiente función se satisface lo requerido:

```java
int mod(int p, int q) {
 var d = p / q;
 var r = d * q;
 var m = p - r;
 return m;
}
```

<div align='center'>
<img width="382" height="264" alt="image" src="https://github.com/user-attachments/assets/79c25255-d7c2-4f19-aea5-ccfb53384dda" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.3

Este ejercicio requiere crear una función que calcule una diferencia de cuadrados entre dos números enteros dados. Los valores esperados de salida con los siguientes:

<div align='center'>
<img width="654" height="80" alt="image" src="https://github.com/user-attachments/assets/358155ac-09ee-40c2-9831-56ea6f99af8f" />
</div>

Con la siguiente función se satisface lo requerido:

```java
int diferenciaDeCuadrados(int a, int b) {
 var cuadradoDeA = a * a;
 var cuadradoDeB = b * b;
 var diferenciaDeCuadrados = cuadradoDeA - cuadradoDeB;
 return diferenciaDeCuadrados;
}
```

<div align='center'>
<img width="607" height="261" alt="image" src="https://github.com/user-attachments/assets/aefabd96-e87b-4638-a354-9eb8da03735e" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.4

Este ejercicio requiere crear una función que calcule la distancia entre dos puntos. Cada punto está representado por 2 double; la función toma 4 parámetros: x1, y1, x2 e y2; los dos primeros son las coordenadas x e y del primer punto y los dos últimos son las coordenadas x e y del segundo punto. La formula de la distancia y los valores esperados de salida con los siguientes:

<div align='center'>
<img width="652" height="128" alt="image" src="https://github.com/user-attachments/assets/58193b4d-aa32-4df5-94e8-e03e85b3ab48" />
</div>

Con la siguiente función se satisface lo requerido:

```java
double distanciaEntrePuntos(double x1, double y1, double x2, double y2) {
 var diferenciaX = x2 - x1;
 var diferenciaY = y2 - y1;
 var calculoXAlCuadrado = diferenciaX * diferenciaX;
 var calculoYAlCuadrado = diferenciaY * diferenciaY;
 var raizDeDiferencias = Math.sqrt(calculoXAlCuadrado + calculoYAlCuadrado);
 return raizDeDiferencias;
}
```

<div align='center'>
<img width="823" height="297" alt="image" src="https://github.com/user-attachments/assets/54b44c4b-2296-49bb-a028-b9d95a48984d" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.5

Este ejercicio requiere crear una función que realice una conversión entre grados Fahrenheit a grados Celsius, el número recibido deberá ser un double. La fórmula a utilizar es la siguiente C= (F-32) * 5/9 y los valores esperados de salida con los siguientes:

<div align='center'>
<img width="658" height="82" alt="image" src="https://github.com/user-attachments/assets/cf0a425f-4d91-4cb6-9042-6403b4859ddb" />

</div>

Con la siguiente función se satisface lo requerido:

```java
double conversionFtoC(double t1) {
 var diferenciaEntreCeros = (t1 - 32);
 var diferenciaEntreFactor = (diferenciaEntreCeros / 1.8);
 return diferenciaEntreFactor;
}
```

<div align='center'>
<img width="660" height="251" alt="image" src="https://github.com/user-attachments/assets/3c1445d7-29ad-4f2f-a421-e7104621c057" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.6

Este ejercicio requiere crear una función que calcule la gravedad superficial de un planeta dada la masa y el radio de este. La fórmula a utilizar y los valores esperados de salida con los siguientes:

<div align='center'>
<img width="460" height="128" alt="image" src="https://github.com/user-attachments/assets/95df27d6-4784-4fec-87ad-31600f6963cc" />
<img width="646" height="64" alt="image" src="https://github.com/user-attachments/assets/2cf927ac-5080-4319-ba17-c4f1a3ac27c9" />
</div>

Con la siguiente función se satisface lo requerido:

```java
double gravedadSuperficial(double masa, double radio) {
 var gravedadUniPorMasa = 6.67430e-11 * masa;
 var radioAlCuadrado = radio * radio;
 var gravedadSuperficialR = gravedadUniPorMasa / radioAlCuadrado;
 return gravedadSuperficialR;
}
```

<div align='center'>
<img width="704" height="260" alt="image" src="https://github.com/user-attachments/assets/131bf932-fcc9-4bcc-9103-4d3658a26f36" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.7

Este ejercicio requiere crear una función que calcule la gravedad superficial de la tierra teniendo como literales la masa de la tierra y su radio. Los valores esperados de salida con los siguientes:

<div align='center'>
<img width="650" height="48" alt="image" src="https://github.com/user-attachments/assets/d89574d9-035f-4c97-812b-de2a186d8491" />
</div>

Con la siguiente función se satisface lo requerido:

```java
double gravedadSuperficialDeLaTierra() {
 var masaDeLaTierra = 5.972e24;
 var radioDeLaTierra = 6.378e6;
 var constanteDeGravitacionUniversal = 6.67430e-11;
 var gravedadUniPorMasa = constanteDeGravitacionUniversal * masaDeLaTierra;
 var radioAlCuadrado = radioDeLaTierra * radioDeLaTierra;
 var gravedadSuperficial = gravedadUniPorMasa / radioAlCuadrado;
 return gravedadSuperficial;
}
```

<div align='center'>
<img width="809" height="193" alt="image" src="https://github.com/user-attachments/assets/9b6f3318-499e-4bd0-b538-a88b8aec92d9" />
<img width="390" height="52" alt="image" src="https://github.com/user-attachments/assets/06dc1ab2-93ad-457e-afc6-ee815929ea32" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.8

Este ejercicio requiere crear una función que tome el peso de una persona en la tierra, y devuelva el peso de esa persona en Marte. La formula y los valores esperados de salida con los siguientes:

<div align='center'>
<img width="680" height="194" alt="image" src="https://github.com/user-attachments/assets/d2fa2274-4041-4991-84d3-952659d47795" />
</div>

Con la siguiente función se satisface lo requerido:

```java
double pesoEnMarte(double pesoTierra) {
 var masaDeLaTierra = 5.972e24;
 var radioDeLaTierra = 6.378e6;
 var masaDeMarte = 6.421e23;
 var radioDeMarte = 3.3972e6;
 var constanteDeGravitacionUniversal = 6.67430e-11;
 var gravedadSuperficialTierra = (constanteDeGravitacionUniversal * masaDeLaTierra) / (radioDeLaTierra * radioDeLaTierra);
 var gravedadSuperficialMarte = (constanteDeGravitacionUniversal * masaDeMarte) / (radioDeMarte * radioDeMarte);
 var pesoEnMarteR = (gravedadSuperficialMarte / gravedadSuperficialTierra) * pesoTierra;
 return pesoEnMarteR;
}
```

<div align='center'>
<img width="1099" height="403" alt="image" src="https://github.com/user-attachments/assets/a135222b-601f-4fab-870d-848518d38b4c" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.9

Este ejercicio requiere crear una función que dadas las longitudes de los tres lados, verifique si se puede formar un triángulo. Los valores esperados de salida con los siguientes:

<div align='center'>
<img width="643" height="61" alt="image" src="https://github.com/user-attachments/assets/e81c24a4-355b-4057-8eaf-2a823dd46c24" />
</div>

Con la siguiente función se satisface lo requerido:

```java
boolean esTriangulo(double ladoUno, double ladoDos, double ladoTres) {
 var ladoMasLargoUnoDos = Math.max(ladoUno,ladoDos);
 var primerLadoMenor = Math.min(ladoUno,ladoDos);
 var ladoMasLargo = Math.max(ladoMasLargoUnoDos,ladoTres);
 var segundoLadoMenor = Math.min(ladoMasLargoUnoDos,ladoTres);
 var sumaDeLadosMenores = primerLadoMenor + segundoLadoMenor;
 var esPosible = ladoMasLargo < sumaDeLadosMenores;
 return esPosible;
}
```

<div align='center'>
<img width="737" height="313" alt="image" src="https://github.com/user-attachments/assets/9e99e344-14b6-4a1e-a049-55a8d9bafbf9" />
</div>

Otra posible solución simplificando las comparaciones anteriores y con otra logica para determinar la suma de los lados menores:

```java
boolean esTriangulo(double ladoUno, double ladoDos, double ladoTres) {
 var ladoMasLargo = Math.max(ladoUno, Math.max(ladoDos,ladoTres));
 var sumaDeLados = ladoUno + ladoDos + ladoTres;
 var esPosible = ladoMasLargo < (sumaDeLados - ladoMasLargo);
 return esPosible;
}
```

En esta solución se afronta de forma diferente el problema, comparando todos los lados anidando un max dentro de otro para evitar escribir una linea más, adicional se determina la suma de los dos lados menores sumando los tres lados y luego restando la cantidad del lado mayor. Es más corto el código pero quizás llegue a ser un poco menos entendible para principiantes. De igual forma si no se considera necesario se puede omitir el paso de crear la variable esPosible, dejando en el return solamente la evaluación: ladoMasLargo < (sumaDeLados - ladoMasLargo).

<div align='center'>
<img width="763" height="261" alt="image" src="https://github.com/user-attachments/assets/10815a38-84bd-41ef-a5b1-71d4fcbd7132" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 3.10

Este ejercicio requiere crear una función que reciba tres medidas: a, b y gamma, para luego por medio de la ley de cosenos para los triángulos determinar el tamaño del lado c. La formula y los valores esperados de salida con los siguientes:

<div align='center'>
<img width="486" height="87" alt="image" src="https://github.com/user-attachments/assets/f77a5a7d-0d84-4077-bec5-4378d400b2a8" />
<img width="674" height="77" alt="image" src="https://github.com/user-attachments/assets/21a69b85-767b-44fc-a940-bdfcb4c73880" />
</div>

Con la siguiente función se satisface lo requerido:

```java
double leyCosenos(double a, double b, double gamma) {
 var cuadradoDeA = Math.pow(a,2);
 var cuadradoDeB = Math.pow(b,2);
 var cosDeGamma = Math.cos(Math.toRadians(gamma));
 var tamanoDeC = Math.sqrt(cuadradoDeA + cuadradoDeB - 2 * a * b * cosDeGamma);
 return tamanoDeC;
}
```
Un punto muy importante a considerar es que la función Math.cos espera recibir el valor en radianes, por eso se tuvo que utilizar Math.toRadians para convertir el valor en grados a radianes.

<div align='center'>
<img width="854" height="283" alt="image" src="https://github.com/user-attachments/assets/280c38a9-83ac-4778-9e31-355bf35d7fd8" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Variables - Ejercicios de corrección de código.

## Ejercicio 3.11

Este ejercicio requiere corregir la función dada, ya que, esta arrojando resultados incorrectos. Los valores esperados de salida con los siguientes:

<div align='center'>
<img width="669" height="78" alt="image" src="https://github.com/user-attachments/assets/613df2ee-c02c-433a-9563-6a3e97703829" />
</div>

La función dada es la siguiente:

```java
double promedio(int edadMenor, int edadMayor) {
 var sumaEdades = edadMenor + edadMayor;
 var promedio = sumaEdades / 2;
 return promedio;
}
```

<div align='center'>
<img width="544" height="244" alt="image" src="https://github.com/user-attachments/assets/c7ba614f-d596-4b8e-b9d4-68b3c8b23116" />

</div>

Como podemos ver a continuación, el valor que regresa para el primer resultado es 13.0 en lugar de 13.5 y 2.0 para el segundo el lugar de 2.5 como se espera. Esto ocurre debido que como se estan utilizando valores enteros en los parametros de entrada las variables declaradas a continuación para los calculos suponen que también deben ser enteras, aunque para el retorno convierte el valor en double debido a que este tipo de valor que esperamos, para los calculos ya los considero como enteros y omitio considerar la parte decimal. El arreglo para este código es considerar los parametros de entrada también como double y declarar las entradas debidamente. 

```java
double promedio(double edadMenor, double edadMayor) {
 var sumaEdades = edadMenor + edadMayor;
 var promedio = sumaEdades / 2;
 return promedio;
}
```

<div align='center'>
<img width="595" height="247" alt="image" src="https://github.com/user-attachments/assets/279f231f-7d83-4453-979a-9d46bdadadb1" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Strings - Errores de compilador y del tiempo de ejecución.

## Ejercicio 4.1

Este ejercicio requiere corregir visualizar el error que ocurre al compilar y dar una solución al mismo. El código proporcionado es el siguiente:

```java
boolean empiezaConMinuscula(String s) {
 var primerCaracter = String.charAt(s,0);
 return Character.isLowerCase(primerCaracter);
}
```
El error obtenido es el siguiente:

<div align='center'>
<img width="1004" height="365" alt="image" src="https://github.com/user-attachments/assets/68f74499-c0da-4b3b-8a41-31cb7005003d" />
</div>

Como podemos observar la función tiene dos errores pero van enfocados al mismo problema. Se esta tratando de aplicar la función .charAt() con dos parametros dentro cuando solo debería llevar uno, el otro error es porque se intenta aplicar la función a String cuando debería aplicarse a s.

```java
boolean empiezaConMinuscula(String s) {
 var primerCaracter = s.charAt(0);
 return Character.isLowerCase(primerCaracter);
}
```

<div align='center'>
<img width="595" height="124" alt="image" src="https://github.com/user-attachments/assets/bdcf9d64-a0af-4c32-bdf5-e6ff77b66f41" />
 <img width="346" height="67" alt="image" src="https://github.com/user-attachments/assets/c7bb6db7-3ebd-4e32-b2f2-dddbfe79f775" />
</div>

## Ejercicio 4.2

Este ejercicio requiere corregir visualizar el error que ocurre al compilar y dar una solución al mismo. El código proporcionado es el siguiente:

```java
String pluralizar(int conteo, String s) {
 return (conteo < 2) ? s : s.format("%d %ss", conteo);
}
```
El error obtenido es el siguiente:

<div align='center'>
<img width="748" height="299" alt="image" src="https://github.com/user-attachments/assets/27a809e4-b3db-47c1-ab00-f1d4eabbaf3a" />

</div>

Aquí no hay error al compilar pero notamos que al intenter pluralizar por más de uno a la palabra tenemos un error que nos indica que hace falta el argumento del formateador "%s", que sería nuestro parametro s. Al agregar esto al código podremos utilizarlo sin ningún inconveniente.

```java
String pluralizar(int conteo, String s) {
 return (conteo < 2) ? s : s.format("%d %ss", conteo);
}
```

<div align='center'>
<img width="614" height="154" alt="image" src="https://github.com/user-attachments/assets/17026441-de41-414e-9755-febbade2dc91" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicio 4.3

Este ejercicio requiere corregir visualizar el error que ocurre al compilar y dar una solución al mismo. El código proporcionado es el siguiente:

```java
boolean esVocal(char letra) {
 var letraMinuscula = Character.toLowerCase(letra);
 return 'aeiou'.contains(Character.toString(letraMinuscula));
}
```
El error obtenido es el siguiente:

<div align='center'>
<img width="741" height="384" alt="image" src="https://github.com/user-attachments/assets/a73a1979-1ee1-4087-8f21-f6cdfb1f8f0f" />
</div>

Aquí el error al intentar compilar es debido al uso de las comillas simples en la literal "aeiou" que es tipo String, las comillas simples se utilizan para literales tipo char, o sea de un solo caracter. Corrigiendo esto la función funciona sin inconvenientes:

```java
boolean esVocal(char letra) {
 var letraMinuscula = Character.toLowerCase(letra);
 return "aeiou".contains(Character.toString(letraMinuscula));
}

```

<div align='center'>
<img width="717" height="336" alt="image" src="https://github.com/user-attachments/assets/3384cd69-0496-4ea3-90f3-d9611a5198f4" />
</div>

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>
