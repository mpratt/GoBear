GoBear 1.0
==========
Script en Bash (para linux) que permite descargar los mp3s de la página [goear.com](http://www.goear.com)

Este script permite:
- Descargar mp3s usando su url o codigo
- Buscar por artistas o canciones y escoger el audio a descargar

Requerimientos
==============
Para que este script funcione debes tener los siguientes programas instalados:
- Lógicamente una shell bash (Linux)
- dialog
- [xmlstarlet](http://xmlstar.sourceforge.net/)

Instrucciones
=============
- Asegúrate de cumplir con los requerimientos.
- Descarga este script y asegúrate que el archivo gobear tenga permisos de ejecución (chmod +x gobear).
- ./gobear (o si prefieres ./gobear --help para ver todas las opciones)
- ???
- Profit!!

Ejemplos
========
Por defecto puedes usar el comando ./gobear. Ahí veras una ventana que te pedira los terminos de búsqueda.
Despues podrás seleccionar los archivos que quieras descargar.

	[pratt@localhost ~]$ ./gobear

También puedes pasar los terminos por la consola de una sola vez. Por ejemplo para buscar por canciones de
Justin bieber puedes ejecutar:

	[pratt@localhost ~]$ ./gobear -s justin bieber

Por defecto el script busca las primeras 15 páginas de resultados. Ese valor se puede cambiar con el flag "-p [numero de paginas]"

	[pratt@localhost ~]$ ./gobear -s justin bieber -p 50

Si tienes la url de la cancion que deseas descargar puedes usar el flag "-d"

	[pratt@localhost ~]$ ./gobear -d http://goear.com/listen/8b988d8/bound-for-the-floor-local-h

Problemas conocidos
===================
- No es posible descargar las canciones que contengan comillas (" o ').

Licencia
========
MIT
Copyright (C) 2011 by Michael Pratt <pratt@hablarmierda.net>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

Autor
=====
Michael Pratt
http://www.michael-pratt.com