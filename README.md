# Java-Zero-To-Hero
Repositorio para notas y ejercicios del Boot Camp 'Zero to Hero' impartido por la comunidad de JAVA Latinoamérica. 

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

