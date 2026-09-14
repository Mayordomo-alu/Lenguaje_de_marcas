# 1. Crea un archivo de texto llamado textos.txt:
## Ábrelo con un navegador. Cámbialo de nombre por textos.html. Vuélvelo a abrir con el navegador.
### ¿Qué conclusiones sacas de tu observación?

En el .txt muestra la información tal cual la escribimos, mientras que el .html detecta que hemos seguido unas normas del lenguaje de marcas y modifica el texto para seguir con sus reglas.


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
```
<dam>
 <modulo>
  <titulo>Lenguaje de Marcas</titulo>
   <contenido>
    <unidad>Introducción</unidad>
    <unidad>HTML</unidad>
    <unidad>CSS</unidad>
  </contenido>
 </modulo>
 <modulo>
  <titulo>Base de datos</titulo>
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
</dam>
```
