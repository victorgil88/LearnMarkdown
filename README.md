# Aprende Markdown en Markdown

A continuación se muestra una lista de algunas de las posibilidades que ofrece Markdown para trabajar con él.

## Salto a otro párrafo
Botón intro. El HTML producido es \<p></p>

### Ejemplo:

```
Hola

mundo  
```

Hola

mundo  

<br>
</br>

## Salto de línea
Dos espacios después del texto y luego intro. El HTML producido es \<br>

### Ejemplo:
```
Hola ¿qué tal?  
Bien
```  

Hola ¿qué tal?  
Bien  


<br>
</br>


## Encabezados
Cada # equivale a un nivel de \<h> en HTML, es decir, ## es \<h2>  
Otra alternativa es poner === debajo del texto \<h1> o --- debajo del texto \<h2>

### Ejemplo:

Código:  
```
###### Ejemplo de <h5>  
```
Resultado:  
###### Ejemplo de \<h5>  


Código:  
```
Ejemplo de <h1>  
====  
```

Resultado:  
Ejemplo de \<h1>  
====


Código:  
```
Ejemplo de <h2>  
----  
```

Resultado:  
Ejemplo de \<h2>
----

<br>
</br>



## Enfasis
Cursiva: Guión bajo para cursiva o * antes y después. El HTML producido es \<em>\</em> o \<i>\</i>
Negrita: Dos guiones bajos o dos ** antes y después. El HTML producido es \<strong>\</strong> o \<b>\</b>

### Ejemplo
```
__Hola mundo__ o **Hola mundo**  
```
**Hola mundo**  
```
_Hola mundo_  o *Hola mundo*  
```
*Hola mundo*  
```
_**Ho**la mundo_  
```
_**Ho**la mundo_  
```
Hola _**mun**do_  
```
Hola _**mun**do_  

```
~Hola mundo~
```
~Hola mundo~

<br>
</br>


## Saltar simbolos que normalmente tiene significado en Markdown
La barra \ salta símbolos que normalmente tienen significado en Markdown. También aplica para \'_{}[]()#+-.!

### Ejemplo de \ (Backslash)
Para poder mostrar la # en la siguiente línea es necesario poner \ y así no se intrepretará como un \<h6>  
  
\\###### Hola mundo  
  
Sino se pusiera saldría los siguiente:  
###### Hola mundo  
En el código de este documento aparece ampliamente usado para mostrar el resultado que se ve.

<br>
</br>

## Blockquotes
Se usa crear citas en bloque. En Markdown se usa \> y se pueden encadenar varios. El HTML producido es \<blockquote>\</blockquote>

### Ejemplo:

Código: 
```
> ### Ejemplo de una cita  
>> Esta es la **cita**  
```
Resultado:
> ### Ejemplo de una cita  
>> Esta es la **cita**  

<br>
</br>


## Listas
Para generar listas se usa: \*, +, -, números, etc.  
Si la lista es ordenada se usa un número y un punto. La lista empieza en el primer número y avanza con números enteros consecutivos independientemente del número que se ponga.  
El HTML producido para una lista desordenada (*, +, -) es \<ul> \<li>\</li> \<li>\</li> ... \</ul>. El HTML producido para una lista ordenada (1.,2., etc) es \<ol> \<li>\</li> \<li>\</li> ... \</ol>.

### Ejemplo lista desordenada:
Código:  
```
* **Manzana**  
* *Pera*  
* Fresa  
  
- **Manzana**  
- *Pera*  
- Fresa  
  
+ **Manzana**  
+ *Pera*  
+ Fresa  
```

Resultado:  
* **Manzana**  
* *Pera*  
* Fresa  
  
- **Manzana**  
- *Pera*  
- Fresa  
  
+ **Manzana**  
+ *Pera*  
+ Fresa  


### Ejemplo lista ordenada:

Código:  
```
22. **Manzana**  
21. *Pera*  
21. Fresa

9. **Melón**  
10. *Sandía*  
11. Plátano  

4. **Melocotón**  
5. *Uva*  
6. > Piña
```
  
Resultado:  

22. **Manzana**  
21. *Pera*  
21. Fresa

9. **Melón**
10. *Sandía*
11. Plátano

4. **Melocotón**
5. *Uva*
6. > Piña  


<br>
</br>

## Listas encadenadas   
Se puede crear una lista donde cada elemento de la lista es otra lista.  
Para encadenar listas, en la segunda lista tiene que haber al menos dos tabulaciones.  

Código:
```
1. Lista de la compra
     - Manzana
       - Pera  
```

Resultado:

1. Lista de la compra
     - Manzana
       - Pera  
  
<br>
</br>

## Lista de tareas
Se pueden crear listas de tareas.  
  
Código:
```
- [x] Leer
- [X] Escribir
- [ ] Aprender
```

Resultado:
- [x] Leer
- [X] Escribir
- [ ] Aprender


<br>
</br>


## Bloques de código
Se pueden crear bloques de código de dos formas: con 4 espacios en blanco o con  ```  ´´´. El HTML producido es \<pre>\<code>\</code>\</pre>.  
Con Markdown se puede mezclar código HTML.
Después de las 3 ` se puede especificar el lenguaje para que Markdown lo interprete.



### Ejemplo bloques de código:

Código de bloque de código:  
 
\```  
    asdf asdf asdf asdf  
\<a href="http://www.google.com">Google
\</a>  
\```  


Resultado de bloque de código: 
```
    asdf asdf asdf asdf  
<a href="http://www.google.com">Google</a>
```

Código:  
  
\```javascript  
var s = "JavaScript syntax highlighting";  
alert(s);  
\```  
  
\```python  
s = "Python syntax highlighting"  
print s  
\```  

Resultado:  
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```

<br>
</br>


## Línea horizontal
Se pueden crear líneas horizontales poniendo al menos 3 de los siguientes símbolos: * * * , ***, - - - o ---. El HTML producido es \<hr>_\</hr>

### Ejemplo de líneas horizontales:

Código: 
```
* * *  
***  
- - -  
---  
```

Resultado:
* * *
***
- - -
---  


<br>
</br>

## Links
Existen dos formas de poner links. Inline o por referencia.  

Inline:  
```
[Título](link "Etiqueta")  
```

Referencia:  
```  
[Título]:link "Etiqueta"  
Texto [Título]
```  

### Ejemplo de link inline

Código:  
```
Esto es un ejemplo [Google](https:www.google.com "Buscador") de link Inline.  
```

Resultado:  
Esto es un ejemplo [Google](https:www.google.com "Buscador") de link Inline.  

### Ejemplo de link por referencia
Código:  
```
Esto es un ejemplo [Google] de link por referencia.  
[Google]:https:www.google.com "Buscador" 
```

Resultado:  
Esto es un ejemplo [Google] de link por referencia.  

[Google]:https:www.google.com "Buscador" 

  
<br>
</br>


## Links automáticos
Se pueden escribir links automáticos sin necesitad de hacer el paso previo solo escribiendo el link. En el caso de email hay que meterlo dentro de \<>. El HTML producido es el mismo que en el ejemplo anterior.

### Ejemplo link automático
Código:  
```
Visita www.google.com  
Envía a <asdf@asdf.com>
```

Resultado:  
Visita www.google.com  
Envía a \<asdf@asdf.com>

<br>
</br>


## Imágenes
Las imágenes se insertan igual que un link pero con ! delante. Tanto con Inline como con Referencia.

### Ejemplo imagen Inline

Código: 
```
![google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Logo")
```

Resultado:

![google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Logo")

### Ejemplo imagen con referencia

Código:
```
Google ![googlelogo]

[googlelogo]:https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Logo"
```

Resultado:

Google ![googlelogo]

[googlelogo]:https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Logo"

 

<br>
</br>



## Código
Se puede escribir código sin necesidad de usar bloques de código, es decir, inline. El HTML producido es \<code>\</code>.

### Ejemplo de código inline

Código:  
```
Ejemplo de `print()` de `código`
```

Resutado:  
Ejemplo de `print()` de `código`

<br>
</br>

## Tablas
Para crear tablas se usan | para delimitar las columnas de la misma.  
La primera línea es la cabecera de la tabla. La segunda tiene - para delimitar que es una tabla y aquí se indica si está alineado a izquierda, derecha o centrado se usa : en la segunda línea.
El HTML producido es \<table>\<thead>\</thead>\<tbody>\<tr>\<td>\</td>\<td>\</td>\</tr>\<tr>_\</tr>\<tr>\<td>\</td>\</tr>\</tbody>\</table>


### Ejemplo de tabla

Código de tabla: 
```
|Las   |tablas   |son   |fáciles  
|-----:|:-----|:-----:|-----  
|Texto A |**Texto B** |_Texto C_ |Texto D  
|Texto A |*Texto B* |__Texto C__ |Texto D  
| Hola  
|Texto E |Texto F|Texto G  
|Texto H|Texto I|Texto J|Texto K|  
|Texto L|  
```

Resultado:  

|Las   |tablas   |son   |fáciles   
|-----:|:-----|:-----:|-----
|Texto A |**Texto B** |_Texto C_ |Texto D|  
|Texto A |*Texto B* |__Texto C__ |Texto D|  
|# Hola|
|Texto E |Texto F|Texto G||  
|Texto H|Texto I|Texto J|Texto K|  
|Texto L||  

<br>
</br>

## HTML con Markdown
Se puede insertar código HTML en un archivo de Markdown.


### Ejemplo código HTML:  

Código HTML:  
```
<a href="http://www.google.com">*Google*
</a>  
<a href="http://www.google.com">Google
</a>  
```

Resultado HTML:  
<a href="http://www.google.com">*Google*</a>  
<a href="http://www.google.com">Google</a>


Código:  
```HTML
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>
```  

Resultado:  
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

