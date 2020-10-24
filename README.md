<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/ucrea.jpg" width="200" height="150">    <img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/eg.jpg" width="250" height="100">    <img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/ucr.jpg" width="200" height="150">    <img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/iica.png" width="200" height="150">


<h1 style="font-size:300%;">Introducción al uso de imágenes de Radar de Apertura Sintética aplicado a la agricultura</h1> 
<h2 ">Manual básico de introducción a SNAP</h2> 

<p>Este manual fue elaborado por la Escuela de Geografía de la Universidad de Costa Rica, para el cual colaboraron Jesús Céspedes-Rivera y Cristian Aguilar-Barboza en calidad de asistentes avanzados del proyecto "Transformación digital: Incorporación de tecnología SAR en la gestión de riesgos, agricultura y recursos naturales para Centroamérica", en el marco del proyecto UCREA-IICA.
Este proyecto está coordinado por el Dr Edgar Espinoza Cisneros y co-cordinado por MSc María José Molina Montero. Para mayor información contactar a maria.molinamontero@ucr.ac.cr .</p>

 

<p> Índice </p> 


<li><a href="#Sección1">1. Prerrequisitos</a></li>
<li><a href="#Sección2">2. Objetivos de aprendizaje</a></li>
<li><a href="#Sección3">3. Interfaz de Usuario del software SNAP</a></li>
<li><a href="#Sección4">4. Interpretando una imagen radar.</a></li>

 
<h2 id="Sección1">1. Prerrequisitos</h2>
 
<p>Para ejecutar esta rutina el usuario debe instalar previamente el software Sentinel Toolbox (SNAP), el cual es un software de procesamiento para el análisis y observación de la tierra, con herramientas enfocadas en extensibilidad de datos, portabilidad, procesamiento en marcos gráficos, entre otras herramientas (ESA, 2020).</p>

<p> La descarga del software SNAP se puede realizar en la siguiente dirección electrónica</p> 
<a href="http://step.esa.int/main/download/snap-download/" target="_blank">http://step.esa.int/main/download/snap-download/</a>
 
  
<h2 id="Sección2">2. Objetivos de aprendizaje</h2> 

<li>Explorar la interfaz del software SNAP.</li>
<li>Visualizar imágenes del radar Sentinel 1</li>
<li>Describir las características básicas de una imagen radar.</li>



<h3 ">2.1 Datos a descargar</h3> 

<p>Los datos a utilizar en este ejercicio se pueden descargar en el siguiente link:</p> <a href="https://www.dropbox.com/sh/xb6nb8qwva3e0l8/AACgAV2tx4xtUFa1QtDZKZxUa?dl=0" target="_blank">https://www.dropbox.com/sh/xb6nb8qwva3e0l8/AACgAV2tx4xtUFa1QtDZKZxUa?dl=0</a>



<p>Para este ejercicio se utilizará una imagen radar de apertura sintética tipo GRD de Sentinel-1, estas se pueden obtener de forma gratuita en los repositorios de información Alaska Satellite Facility Vertex y Copernicus Open Access Hub, en ambos casos se debe crear -en caso de no tenerse- una cuenta de acceso que permite descargar información satelital a nivel global.</p>

<h4 ">Alaska Satellite Facility Vertex</h4> 
<p> Buscador de datos:<p>  <a href="https://search.asf.alaska.edu/#/" target="_blank">https://search.asf.alaska.edu/#/</a>
<p> Registro de cuenta:<p>  <a href="https://urs.earthdata.nasa.gov/users/new" target="_blank">https://urs.earthdata.nasa.gov/users/new</a>

<h4 ">Copernicus Open Access Hub</h4>  
<p>Buscador de datos:<p> <a href="https://scihub.copernicus.eu/dhus/#/home" target="_blank">https://scihub.copernicus.eu/dhus/#/home</a>
<p>Registro de cuenta:<p>  <a href="https://scihub.copernicus.eu/dhus/#/self-registration" target="_blank">https://scihub.copernicus.eu/dhus/#/self-registration</a>


<h2 id="Sección3">3. Interfaz de Usuario del software SNAP</h2>

<p>El espacio de trabajo en SNAP está conformado con un menú de archivos (1), un menú de botones (2), el panel de capas (3), espacio de localización (4) y área de trabajo (5) (Fig 1). </p> 

<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig1.jpg">

<h4 id="Sección3">Fig. 1. Interfaz de la vista general de SNAP.</h4>

Abrir archivos en SNAP
<p>Los archivos se pueden abrir mediante: File/Open Product… o seleccionando <img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig18.png"> (Fig 2).</p> 

<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig2.jpg">

<h4 id="Sección3">Fig. 2. Abrir archivos en SNAP.</h4>

<p>Se debe tener claro el tipo de archivo que se desea abrir, en la sección Files of type debe identificar el formato de información que desea manejar(flecha roja) (Fig 3). Finalmente debe seleccionar y abrir el archivo de interés.</p>

<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig3.png">
<h4 id="Sección3">Fig 3.Búsqueda del archivo de interés y la selección de formato.</h4>

<p>Una vez abierto el archivo de interés en <strong>Product Explorer</strong> se visualiza el archivo de la imagen, este incluye los metadatos de la imagen (<strong>Metadata</strong>), así como las bandas (<strong>Bands</strong>) de la imagen, en este caso, las polarizaciones VV y VH. En la parte inferior de la imagen, en la opción <strong>Worldview</strong>, se muestra la localización del área de estudio (Fig 4).</p>

<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig4.jpg">
<h4 id="Sección3">Fig 4. Resultado de cargar una imagen a SNAP. En el recuadro rojo se marca el espacio que cubre la imagen descargada</h4>

<p>Para visualizar la imagen radar, presione doble click sobre cada una de las bandas <strong>Sigma0_VH y Sigma0_VV</strong> (Fig 5).</p>

<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig5.png">
<h4 id="Sección3">Fig 5. Cargar imágenes <strong>Sigma0_VH y Sigma0_VV</strong>.</h4>

<p>Las Imágenes desplegadas en la interfaz de SNAP se visualizan en la Fig 6.</p>

<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig6.png">
<h4 id="Sección3">Fig 6. Visualización de imágenes. La imagen de la izquierda (A) corresponde a <strong>Sigma0_VH</strong>, la imagen derecha (B) corresponde a<strong>Sigma0_VV</strong>.</h4>

<p>En <strong>View/Tool Windows</strong> se puede añadir a la vista de la interfaz diferentes pestañas para analizar u observar los datos de la imagen (Fig 6).</p>

<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig7.png">
<h4 id="Sección3">Fig 7. Añadir ventanas a la interfaz de inicio de SNAP.</strong>.</h4>

<p> El software contiene una caja de herramienta/Toolbox para el preprocesamiento y procesamiento especializado de imágenes radar (Radar) (Fig 8).</p>
<img src="https://github.com/Emmanuel461/Introducci-n-a-SNAP/blob/main/Im%C3%A1genes/Fig8.png">
<h4 id="Sección3">Fig 8. Toolbox Radar en SNAP.</strong>.</h4>

<h2 id="Sección4">4. Interpretando una imagen radar.</h2>


