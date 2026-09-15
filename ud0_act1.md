# 1. Crea un archivo de texto llamado textos.txt:
## Ábrelo con un navegador. Cámbialo de nombre por textos.html. Vuélvelo a abrir con el navegador.
### ¿Qué conclusiones sacas de tu observación?

+ En el .txt muestra la información tal cual la escribimos, mientras que el .html detecta que hemos seguido unas normas del lenguaje de marcas y modifica el texto para seguir con sus reglas.

***
# 2. Observa el siguiente fragmento de un texto:
```
<dam>
<modulo><titulo>Lenguaje de Marcas</titulo>
<contenido>
<unidad>Introducción</unidad>
<unidad>HTML</unidad>
<unidad>CSS</unidad>
…
</contenido>
</modulo>
…
</dam>
```
## Lo que vemos es una manera de estructurar la información sobre los módulos de DAM. Podemos distinguir:
#### Vocabulario: dam, modulo, titulo, contenido, unidad
#### Reglas: dam contiene varios modulos, un modulo tiene un titulo y un contenido, contenido tiene varias unidades, todas las unidades están en un contenido, las unidades son texto simple, detrás de una unidad solo puede ir otra unidad o fin contenido, detrás de uno modulo solo puede ir otro modulo o fin de dam
### Completa con al menos tres de los módulos de DAM en este archivo. Llámale DAM.sgml:
+ Decidí añadir los módulos de "Base de datos", "Programación" y "Sistemas informáticos":
```
<dam>
 <modulo>
  <titulo>Lenguaje de Marcas</titulo>
  <contenido>
   <unidad>Introducción a Lenguaje de marcas</unidad>
   <unidad>HTML</unidad>
   <unidad>CSS</unidad>
  </contenido>
 </modulo>
 <modulo>
  <titulo>Base de Datos</titulo>
  <contenido>
   <unidad>Introducción base de datos</unidad>
   <unidad>Modelo Entidad Relacion</unidad>
   <unidad>Modelo Racional</unidad>
  </contenido>
 </modulo>
 <modulo>
  <titulo>Programacion</titulo>
  <contenido>
   <unidad>Introducción a programacion</unidad>
   <unidad>Introducción a java</unidad>
   <unidad>Condiciones y bucles</unidad>
  </contenido>
 </modulo>
 <modulo>
  <titulo>Sistemas Informáticos</titulo>
  <contenido>
   <unidad>Introducción a Sistemas informáticos</unidad>
   <unidad>Máquinas virtuales</unidad>
   <unidad>Ensamblaje y reparación</unidad>
  </contenido>
 </modulo>
</dam>
```
***
# 3. Crea tu propio documento SGML indicando vocabulario y reglas. Implementa los datos para PAISES DEL MUNDO.
+ Vocabulario: paises_del_mundo, país, nombre, idioma, principal, secundario, capital, area.
+ Reglas: paises_del_mundo contiene varios paises, un pais contiene uno o mas idiomas, un idioma solo tiene uno principal pero puede o no tener varios secundarios y estos serán texto simple, cada país también tendrá un solo nombre, una capital y una area, el terreno son un número en kilometros cuadrados. Detrás de un país solo puede ir otro país o fin de paises_del_mundo.
```
<paises_del_mundo>
 <país>
  <nombre>España</nombre>
  <idioma>
   <principal>Castellano</principal>
   <secundario>Valenciano</secundario>
   <secundario>Catalán</secundario>
   <secundario>Euskera</secundario>
   <secundario>Gallego</secundario>
  </idioma>
  <capital>Madrid</capital>
  <area>505.990</area>
 </país>
 <país>
  <nombre>Alemania</nombre>
  <idioma>
   <principal>Alemán</principal>
  </idioma>
  <capital>Berlin</capital>
  <area>357.375</area>
 </país>
 <país>
  <nombre>Belgica</nombre>
  <idioma>
   <principal>Neerlandés</principal>
   <secundario>Francés</secundario>
   <secundario>Alemán</secundario>
  </idioma>
  <capital>Bruselas</capital>
  <area>30.528</area>
 </país>
 <país>
  <nombre>Canadá</nombre>
  <idioma>
   <principal>Inglés</principal>
   <secundario>Francés</secundario>
  </idioma>
  <capital>Ottawa</capital>
  <area>9.984.670</area>
 </país>
</paises_del_mundo>
```
# 4. Modifica con un lenguaje de marcas la siguiente información para darle estructura y significado semántico al documento. Indica vocabulario y reglas.
###### FALCO (En papel)
###### ISBN 9788420419688
###### ARTURO PEREZ REVERTE
###### 9788420419688
###### 296 págs
###### ALFAGUARA
###### CASTELLÀ
###### TODO ALATRISTE (EBOOK)
###### 9788420425528
###### ARTURO PEREZ REVERTE
###### ALFAGUARA
###### CASTELLÀ
###### HOMBRES BUENOS (En papel)
###### 9788466329804
###### ARTURO PEREZ REVERTE
###### PUNTO DE LECTURA, 2024
###### La heróica aventura de quienes se atrevieron a cambiar el mundo con libros. En tiempos de oscuridad

+ Vocabulario: librería, libro, titulo, isbn, autor, número_de_páginas, editorial, idioma, formato, sinopsis, tipo.
+ Reglas: Una librería tiene varios formatos, los formatos tienen un tipo y varios libros. Libros contienen un titulo, autor, editorial, idioma y también puede tener como opcional una sinopsis o número_de_paginas en texto simple, detrás de libro solo puede ir otro libro o fin de formato, detrás de formato solo puede ir otro formato o fin de librería.

```
<libreria>
 <formato><tipo>En papel</tipo>
  <libro>
   <titulo>Falco</titulo>
   <isbn>9788420419688</isbn>
   <autor>Arturo Perez Reverte</autor>
   <editorial>Alfaguara</editorial>
   <idioma>Castellà</idioma>
   <número_de_paginas>296</número_de_paginas>
  </libro>
  <libro>
   <titulo>Hombres buenos</titulo>
   <isbn>9788466329804</isbn>
   <autor>Arturo Perez Reverte</autor>
   <editorial>Punto de lectura, 2024</editorial>
   <idioma></idioma>  //no se dice cual es el idioma, pero pienso que es un campo principal.
   <sinopsis>La heróica aventura de quienes se atrevieron a cambiar el mundo con libros. En tiempos de oscuridad</sinopsis>
  </libro>
 </formato>
 <formato><tipo>Ebook</tipo>
  <libro>
   <titulo>Todo Alatriste</titulo>
   <isbn>9788420425528</isbn>
   <autor>Arturo Perez Reverte</autor>
   <editorial>Alfaguara</editorial>
   <idioma>Castellà</idioma>
  </libro>
 </formato>
</libreria>
```


###### Alejandro Blasco Mayordomo
