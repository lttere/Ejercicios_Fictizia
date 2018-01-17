# CÓMO FUNCIONA UN NAVEGADOR

El ordenador lee tres idiomas, **HTML,CSS y JAVASCRIPT**.

Se descarga en el caché una copia de la web en tu ordenador(CLIENT SIDE) a través de un dominio. Estos están en servidores (SERVER SIDE), con una dirección IP(números) en lugar del nombre que interpreta primero el DNS(DOMAIN NAMES SERVER), en una carpeta alojada (HOSTING).

**CLIENT SIDE—DNS—SERVER SIDE—CLIENT SIDE**

**HTML:** Alberga contenido estructurado y semántica. **Qué es.**

**CSS:** Se preocupa cómo se ve lo que ponemos en el HTML (presentación, formato, estilos…). **Cómo se ve**.

**JAVASCRIPT**: Comportamiento de los elementos de la interfaz de la descarga de datos dinámincos asíncronos (AJAX). Interactividad, **cómo funciona.** 

La importancia del CSS: http://www.csszengarden.com/ 

# DISTRIBUCIÓN DEL PROYECTO

>## CARPETAS Y ARCHIVOS

El archivo primero será la portada que SIEMPRE ha de llamarse **Index.html**

Tanto las carpetas como archivos, se eligen los nombres sin simbología, espacios, ñ, etc. El nombre del archivo es muy importante por el SEO y Google.
Ej: en lugar de poner Galeria.html poner mejor Trabajos-fotografia.html. El guión del medio siempre lo interpreta como espacio, tanto el guión bajo como el guión simple. ****Recomendación de Google** será poner el guión simple.** 

Los **HTML** no van en subcarpetas, van en raíz.

Sin embargo, el **CSS**, va en una subcarpeta en la que pondremos todo lo relacionado. El nombre de ésta carpeta no es tan importante. Ej: main.css, styles.css, css.css

Dentro de ésta, irán distintas carpetas con sus archivos según el contenido:

 - Las fotografías del CSS: son las de fondo, que va en una subcarpeta dentro del CSS. Ej: ui-img. Sus archivos serán: fondo.jpg, icono.png, icono.svg.
 - Las fuentes (fonts): Las podemos sacar de Googlefonts ó de los archivos estandars. Éstos archivos deben estar en .woof para web, si están en .ttf ó .otf deben ser convertidos. La cantidad de fuentes importa, cuantas menos mejor.

El **JS** tiene una subcarpeta con los archivos y carpetas con las librerías. Ejemplo para la carpeta de la librería: libs.

Reducimos, dentro de lo posible, al mínimo el número de carpetas y archivos por el tema del peso y cantidad de llamadas, cuanto menos mejor. 

**Las fotografías del contenido** irá en otra carpeta. Ej: img. Dentro de ésta carpeta, las fotos serán en jpg la gran mayoría y el nombre será muy importante por el tema del SEO y Google, debe ser muy descriptivo. Ej: titulo-de-la-noticia-referente.jpg .

**Los vídeos**, van en otra carpeta dentro del proyecto la cual llamaremos media si hay vídeo y audio, si sólo tenemos video la llamaremos video. El nombre del video afecta también al SEO y Google. Ej: video.mp4.  Otro archivo que hay que incluir es el poster, que es la imagen principal en jpg relacionada con el video, lo nombramos igual que el video.jpg .

**Los iconos de la web** (touch icon y los logos de la marca), éstos van sueltos sin carpeta. Los generamos de distintos tamaños a través de https://realfavicongenerator.net/ para los distintos dispositivos.

**Carpeta desastre**, ésta es la que no se sube a internet donde ponemos los PSD, los editables, los videos 4k...


# HTML

Empezaremos abriendo una carpeta del proyecto, la guardamos y la vinculamos con el editor de código para comenzar con el HTML.

La primera línea de código será el Doctype que define el tipo de documento con el que vamos a trabajar, quedando así: 

				<!DOCTYPE html>

**Como anotación, toda línea de código estará escrita en minúsculas.*

La segunda línea de código, 		
			
				<html>
		Aquí va todo lo relacionado al documento.		
				</html> (para cerrar)

En tercer lugar,

	<head>
		Se utiliza para poner la información de la web como los títulos.
    </head> (para cerrar)
								 
	<title> texto </title>

 Ésta información afecta mucho al SEO y Google y también corresponde al enlace de la página. Cada página (website) lleva un title distinto obligatoriamente poniendo siempre nombres coherentes para el usuario, con información relevante en primer lugar y 60 caracteres com máximo.
                  
    <meta charset ="mapa de caracteres utf-8">
    
    <meta name = "descripcion" content = "describe el sitio"> con un máximo de 155 			   carácteres.
                  
    <meta property =" " content =" "> se utiliza en redes sociales.

En cuarto lugar,

	<body>
	Aquí se coloca todo el contenido de la web, desde la cabecera, el texto, etc.
	</body> 

Uno de los contenidos de la web son los párrafos que se representan con la etiqueta,

	  <p> </p>
				  
Dentro de los párrafos, al igual que en todo el contenido de la web, es muy importante enriquecer semánticamente todo. Por ello, existen otras etiquetas que se encargan de eso dependiendo de dónde estén colocadas. En párrafo utilizamos,

	<strong> unas palabras de texto elegido </strong>