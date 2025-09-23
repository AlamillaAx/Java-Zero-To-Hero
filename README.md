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
* ### Ejercicios de codificación
  * [Ir a Ejercicio 7](#ejercicio-7---adivina-la-pelicula)
  * [Ir a Ejercicio 8](#ejercicio-8---llenado-de-caracteres)
  * [Ir a Ejercicio 9](#ejercicio-9)
  * [Ir a Ejercicio 10](#ejercicio-10)
  * [Ir a Ejercicio 11](#ejercicio-11)
* ### Ejercicios de corrección de código
  * [Ir a Ejercicio 12](#ejercicio-12)
  * [Ir a Ejercicio 13](#ejercicio-13)
* ### Operadores - Errores del compilador y de ejecución
  * [Ir a Ejercicio 14](#ejercicio-14)
  * [Ir a Ejercicio 15](#ejercicio-15)
  * [Ir a Ejercicio 16](#ejercicio-16)
* ### Operadores - Ejercicios de codificación
  * [Ir a Ejercicio 17](#ejercicio-17)
  * [Ir a Ejercicio 18](#ejercicio-18)
  * [Ir a Ejercicio 19](#ejercicio-19)
  * [Ir a Ejercicio 20](#ejercicio-20)
  * [Ir a Ejercicio 21](#ejercicio-21)
  * [Ir a Ejercicio 22](#ejercicio-22)
  * [Ir a Ejercicio 23](#ejercicio-23)
  * [Ir a Ejercicio 24](#ejercicio-24)
  * [Ir a Ejercicio 25](#ejercicio-25)
  * [Ir a Ejercicio 26](#ejercicio-26)
  * [Ir a Ejercicio 27](#ejercicio-27)
* ### Operadores - Ejercicios de corrección de código
  * [Ir a Ejercicio 28](#ejercicio-28)
* ### Variables - Errores de compilador y de ejecución
  * [Ir a Ejercicio 29](#ejercicio-29)
* ### Variables - Ejercicios de códificación
* ### Variables - Ejercicios de corrección de código
  
## Errores del compilador y de ejecución

El objetivo de estos ejercicios es visualizar los errores que arroja cada función al intentar crearlas, entender el error y corregirlo para que funcione correctamente. 

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
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Ejercicios de codificación

El objetivo de estos ejercicios es desarrollar una función desde cero teniendo solamente las salidas deseadas para cada una.

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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
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

<div align='right'>
<a href="#menu-de-ejercicios">Regresar al menú</a>
</div>

## Operadores - Errores del compilador y de ejecución

En estos ejercicios observaremos los errores más comunes durante el uso de operadores así como la solución para cada uno de ellos. 

## Ejercicio 14

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

## Ejercicio 15

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

## Ejercicio 16

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

## Ejercicio 17

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

## Ejercicio 18

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

## Ejercicio 19

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

## Ejercicio 20

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

## Ejercicio 21

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

## Ejercicio 22

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

## Ejercicio 23

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

## Ejercicio 24

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

## Ejercicio 25

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

## Ejercicio 26

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

## Ejercicio 27

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

## Ejercicio 28

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

## Ejercicio 29

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

## Ejercicio 30

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
