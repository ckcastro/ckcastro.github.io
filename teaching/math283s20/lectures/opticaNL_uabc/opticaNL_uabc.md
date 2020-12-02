<style>

.section .reveal .state-background {
   background: #ffffff;
   word-wrap: normal;
  -moz-hyphens: none;
}

.reveal h1, .reveal h2, .reveal h3 {
  word-wrap: normal;
  -moz-hyphens: none;
}

.section .reveal h1, 
.section .reveal h2,
.section .reveal h3,  
.section .reveal ul,
.section .reveal p {
   color: black;
   margin-top: 50px;
   text-align: center;
}

.midcenter {
    position: fixed;
    top: 50%;
    left: 50%;
}

.footer {
    color: black; 
    background: #ffffff;
    position: fixed; 
    top: 95%;
    text-align:left; 
    width:100%;
    font-size: 30px;
}

table {
  border: 1px solid black;
  text-align: center;
  border-bottom: 1px solid #ddd;
}

th {
  text-align: center;
}

tr {
  text-align: center;
}

td {
  text-align: center;
}


table.minimalistBlack {
    border: 3px solid #000000;
    width: 100%;
    text-align: center;
    border-collapse: collapse;
}

body{
  font-size: 40px;
}

</style>


<!-- foo 
Highlighting
bold
strong
orange <b style="color:#d95f02"> text </b>
green  <b style="color:#1b9e77"> text </b>
purple <b style="color:#d24693"> text </b>
red    <b style="color:#FF0000"> text </b>
blue   <b style="color:#0000FF"> text </b>

<p style = "font-size: 50px;">Definición de onda </p>

font-weight:bold;
-->

Estabilidad y dinámica de modos ópticos en estructuras no lineales, helicoidales y PT-simétricas 
=================================================
title: Fibras opticas retorcidas
author: Dr. Claudia Castro Castro
date: 2 de Diciembre del 2020
autosize: true
incremental: true
width: 1920
height: 1080
font-family: 'Lato'


<p style="text-align:center; font-weight:bold">Seminario “Dr. Alberto Rubio” Facultad de Ciencias UABC </p>

<div class='footer'>
<center>
   Copyright Disclaimer: material is for educational purposes only under fair use.
</center>
</div>

Índice
==========================================================

<div style="float:left; width:100%">
<ul>
<li>
Introducción
    <ul>
      <li>Definición de onda</li>
      <li>Antecedentes</li>
      <li>Fibras ópticas</li>
      <li>Fenómenos ópticos lineales vs no lineales</li>   
      <li>Ecuaciones de Maxwell</li>
      <li>¿Qué significa PT-simétrico?</li>
      <li>¿Qué significa torcido?</li>
    </ul>
</li>
<li>Ecuación de Schrödinger </li>
<li>Dinámica y estabilidad</li>
<li>Conclusiones</li>
</ul>
</div>


Definición intuitiva de onda 
========================================================

<div style="border: 1px solid blue;border-color:#287EC7; color:black;position: fixed; top:30%; text-align:center;left:5%;padding:1em; font-size: 45px" class="fragment">
<ul style="list-style-type:none;">
Cualquier señal reconocible que se transfiere de una parte del medio a otra con una velocidad de propagación reconocible
</ul>
</div> 


<div class='footer'>
<small>Whitham, G. B., "Linear and nonlinear waves", Ed. John Wiley & Sons, 1974</small>
</div>


Antecedentes
========================================================

<div style="float:left; width:30%" class="fragment">
1790s: "Telégrafo óptico" inventado por Claude Chappe 
<img src="figs/telegrafooptico.jpeg" alt="Telegrafo optico y sus simbolos"><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Courtesía de Wikipedia Commons </small>
</p>
</div>

<div style="float:left; width:30%" class="fragment">
<img src="figs/fountain.png" alt="Luz guida en chorros de agua"><div style="float:center; width:100%">
</div>
</div>


<div style="float:left; width:40%">
<ul style="list-style-type:none;">
<li> 1840s: Daniel Collodon y Jacques Babinet demostraron que la luz podía guiarse a través de chorros de agua para exhibiciones de fuentes.
</li>
<li></br>
Cuando los rayos de luz en el agua golpean el borde del chorro con un ángulo, la <strong>reflexión interna total</strong> los atrapa en el líquido.
</li>

<li></br>
Refracción en la superficie depende de la diferencia en el <strong>índice de refracción</strong>; cuanto mayor es la diferencia, más refracción
</li>
</ul>
</div>

<div class='footer'>
<small>Hecht, J. City of Light: The Story of Fiber Optics
Oxford University Press, 1999</small>
</div>


Reflexión interna total (TIR)
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li> 
Es un efecto secundario de la <i>refracción</i>, la curvatura de la luz que pasa de un material transparente a otro.
</li>
</ul>
</div>

<div style="float:left; width:50%" class="fragment">
<img src="figs/refraction_city_of_light.png" alt="Refraction de vidrio a aire"><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Courtesía de Hecht, J. City of Light: The Story of Fiber Optics, 1999</small>
</p>
</div>

<div style="float:left; width:50%">
<ul style="list-style-type:none;">
<li></br><strong>Índice de refracción</strong>
$$n=\frac{\text{velocidad de la luz en el vacio}}{\text{velocidad en el material}}$$
</li>
<li></br><strong>Ley de Snell</strong>
$$n_1 \sin{\theta_1} = n_2 \sin{\theta_2} $$
</li>
<li></br>Resposable por 
</li>
</ul>
</div>

<div style="float:left; width:10%;padding-left:5%" class="fragment">
<img src="figs/fresnel.JPG" alt="Lente de faro Fresnel"><div style="float:center; width:100%">
</div>
</div>

<div style="float:left; width:15%" class="fragment">
<img src="figs/lotus.jpeg" alt="Flor de loto de cristal"><div style="float:center; width:100%">
</div>
</div>

<div style="float:left; width:20%" class="fragment">
<img src="figs/diamond.jpg" alt="Total Internal Reflections in Diamond "><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Courtesía de Wikimedia Commons</small>
</p>
</div>


Reflexión interna total (TIR)
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li> 
</li>
</ul>
</div>

<div style="float:left; width:40%;font-size: 40px" class="fragment">
<img src="figs/totalinternalreflexion.png" alt="Luz guida en chorros de agua"><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Courtesía de Hecht, J. City of Light: The Story of Fiber Optics, 1999</small>
</p>
</div>


<div style="float:left; width:60%">
<ul>
<li> La luz que golpea la superficie casi directamente se refracta en el aire
</li>

<li>Hay un <b>ángulo crítico</b> donde no puede emerger al aire, se mide a partir de una línea llamada <b>normal</b> que es perpendicular a la superficie.
</li>
<li>Si $\theta_1 > \sin^{-1}\left(\frac{n_2}{n_1}\right)$ $\Rightarrow \sin \theta_2 > 1 \;\;(!)$
</li>
<li>
La luz fuera del ángulo crítico se refleja de nuevo en el cristal.
</li>
<li>ángulo crítico
$\theta_c = \sin^{-1}\left(\frac{n_2}{n_1}\right)$ existe solo cuando $n_2 < n_1$, entonces
TIR ocurre solo dentro del <b>medio con índice más alto</b>
</li>
</ul>
</div>

<div style="float:left; width:20%; padding-left:20%" class="fragment">
<img src="figs/tir_in_a_wine_glass.jpg" alt="Demonstration of Total-Internal-Reflection(TIR) in a wine glass"><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Courtesía de Keerthi, CC BY 4.0 via Wikimedia Commons</small>
</p>
</div>


Inicios de las fibras ópticas
========================================================

<div style="float:left; width:100%">
<ul>
<li>Generaciones de artesanos, inventores, ingenieros y científicos
desarrollaron la tecnología para hacer vidrio
</li>
  <ul>
  <li> Es <b>maleable</b> cuando está caliente, así como la <b>transparencia</b> del sólido, lo que lo ha convertido en un material atractivo.
  </li>
  <li> El ingrediente más importante del vidrio común es el dióxido de silicio, un mineral duradero conocido como <strong>Sílice/Silica</strong>.
  </li>
  </ul>
<li> 1930s: Heinrich Lamm (médico) primera persona conocida que ha demostrado la transmisión de imágenes a través de un arreglo de fibras ópticas
</li> 
  <ul>
  <li> Sin embargo, las fibras descubiertas transmitían imágenes de manera deficiente.
  </li>
  </ul>
<li>1950s: Van Heel y O'Brien recubren una fibra descubierta con un <b>material de índice menor</b> mantendría la TIR mientras protege la superficie óptica
</li>
<ul>
<li>Fibras revestidas de vidrio tenían una atenuación de aproximadamente un <b>decibel por metro (dB/m)</b>, lo que está bien para imágenes médicas, pero demasiado alto para comunicaciones.
</li>
</ul>
</ul>
</div>

<div class='footer'>
<small>Hecht, J. City of Light: The Story of Fiber Optics
Oxford University Press, 1999</small>
</div>


Características de las fibras ópticas
========================================================

<div style="float:left; width:33%" class="fragment">
<img src="figs/dielectric_fiber.png" alt="Esquema de fibra optica dielectric y el perfil de indices de refraccion"><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Agrawal G., Nonlinear fiber optics, Academic Press, 2013</small>
</p>
</div>


<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li> 
</li>
</ul>
</div>


Características de las fibras ópticas
========================================================

<div style="float:left; width:35%" class="fragment">
<img src="figs/opticalFiber.jpeg" alt="Esquema de fibra optica multi-nucleo"><div style="float:center; width:100%">
</div>
<p style="text-align:left">
<small>Courtesía de ..</small>
</p>
</div>

<div style="float:left; width:30%" class="fragment">
<img src="figs/hexagonalarray.png" alt="Esquema de un arreglo 2D"><div style="float:center; width:100%"></div>
<p style="text-align:center">
<small>Pertsch et al. Nonlinearity and
disorder in fiber arrays. Physical
Review letters, 2004</small>
</p>
</div>

<div style="float:left; width:33%" class="fragment">
<img src="figs/array.png" alt="Esquema de un arreglo 2D"><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Joannopoulos et al. Photonic crystals: molding the flow of light. Princeton University Press, 2011.</small>
</p>
</div>

Dispersión
========================================================

<div style="float:left; width:40%" class="fragment">
<img src="figs/waterdrop.jpg" alt="Gota que cae en agua"><div style="float:center; width:100%">
</div>
<p style="text-align:center">
<small>Cortesia de Pixabay </small>
</p>
</div>

 
<div style="float:left; width:60%">
<ul>
<li> Como cuando una piedra que cae en un estanque inmóvil produce ondas en la superficie del agua, eventualmente desaparecen y se desvanecen
</li>
<li>
Un rayo de luz puede extenderse cuando viaja a través de diferentes medios.
</li>
<li> La dispersión temporal y la difracción espacial se deben a la dependencia del índice de refracción de la frecuencia y la longitud de onda
</li>
<li>Ambos causan un ensanchamiento espacial y temporal de la luz.
</li>
</ul>
</div>


<div class='footer'>
<small>Yang J., "Nonlinear waves and nonintegrable systems", Ed. SIAM, 2010</small>
</div>



Ecuaciones de Maxwell
========================================================

La luz es una <b>onda electro-magnética</b> que consiste de un campo eléctrico  y un campo magnético oscilando a una tasa muy alta ($10^{14}$ Hz) viajando en el espacio con una dirección perpendicular a ambos campos vectoriales

<div style="float:left; width:30%">
<ul style="list-style-type:none;">
<li>
$$\begin{align}
\nabla\times\mathbf{E}=&-\frac{\partial\mathbf{B}}{\partial t}\\
\nabla\times\mathbf{H}=&\mathbf{J}+\frac{\partial\mathbf{D}}{\partial t}\\
\nabla\cdot\mathbf{D}=&\rho_{v}\\
\nabla\cdot\mathbf{B}=&0
\end{align}$$
</li>
</ul>
</div>

<div style="float:left; width:40%">
<ul style="list-style-type:none;">
<li> 
</br>$\mathbf{E}$ campo eléctrico [$V/m$]
</br>$\mathbf{B}$ densidad de flujo magnético [$T$]
</br>$\mathbf{H}$ campo magnético [$A/m$]
</br>$\mathbf{D}$ densidad de flujo eléctrico [$C/m^2$]
</br>$\mathbf{J}$ densidad de corriente eléctrica  [$A/m^2$]
</li>
</ul>
</div>

<div style="float:left; width:30%">
<ul style="list-style-type:none;">
<li></br> $\mathbf{D}=\varepsilon \mathbf{E}$
</br>$\mathbf{B}=\mu \mathbf{H}$
</br>$\mathbf{J}=\sigma \mathbf{E}$
</br></br>$\varepsilon= \varepsilon_0 \varepsilon_r$ dielectric permittivity
</br>$\mu= \mu_0 \mu_r$ permeability
</br>$\sigma$ electric conductivity
</li>
</ul>
</div>

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
</ul>
</div>



<div style="float:left; width:100%">
<ul>
<h2>Ecuación de onda</h2>
<li>El campo vectorial eléctrico satisface la ecuación de onda
$$\nabla^2 \mathbf{E}(\mathbf{r},t)-\frac{1}{c^2}\frac{\partial^2 \mathbf{E}(\mathbf{r},t)
}{\partial t^2}=0$$
</li>
<li>T-simetría: ecuación es <strong>invariante</strong>  w. r. t. tiempo $t\rightarrow -t$
</li>
<li>
</li>
</ul>
</div>

<div class='footer'>
<small>Wartak, Computational photonics, Cambridge Univeristy Press, 2013</small>
</div>



Óptica lineal vs no lineal
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li><b style="color:#1b9e77"> Lineal </b>: las ondas electromagnéticas inducen una separación de las cargas en el material, es decir, una <i>polarización</i> $P_L$, la cual es <b style="color:#1b9e77">directamente proporcional</b> al campo eléctrico
$$P = \varepsilon_0 \chi^{(1)} E$$
donde   $\varepsilon_0$ es la <i>permitividad del vacío</i> y
$\chi^{(1)}$ es la constante de <i>susceptibilidad</i>.
</li>
</ul>
</div>

<div style="float:left; width:100%">
<ul>
<li> Interacción de la luz con la materia <b style="color:#1b9e77">no modifica</b> las propiedades de onda
</li>
<li>Ejemplos de fenómenos ópticos lineales:
</li>
</ul>
</div>


<div style="float:left; width:11%" class="fragment">
<img src="figs/cat.jpg" alt="Reflejo de un gato en un espejo"><div style="float:center; width:100%"></div>
<p style="text-align:center"><small>
Reflexión
</small></p>
</div>


<div style="float:left; width:14%" class="fragment">
<img src="figs/pencil.jpg" alt="Ejemplos de fenómenos ópticos lineales"><div style="float:center; width:100%">
</div>
<p style="text-align:center"><small>
Refracción
</small></p>
</div>



<div style="float:left; width:33%" class="fragment">
<img src="figs/photochomic-vs-transition-lenses.jpg" alt="Lentes photocromaticos"><div style="float:center; width:100%">
</div>
<p style="text-align:center"><small>
Photocromia
</small></p>
</div>


<div style="float:left; width:42%">
<ul style="list-style-type:none">
<li>$\diamond$ Linealidad es una suposición que solo es válida para <b style="color:#1b9e77">bajas intensidades</b>
</li>
<li></br>
</li>
<li>$\diamond$ Casi todos los materiales tienen algunos efectos no lineales si la fuente de luz solo es lo suficientemente potente  <b style="color:#d95f02">altas intensidades</b>
</li>
</ul>
</div>

<div class='footer'>
   <small>Source</small>
</div>



Óptica no lineal
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li><b style="color:#d95f02">No lineal</b>: describe el comportamiento de la luz en medios  en   cual   el   componente   dieléctrico   de la <i>polarización</i> responde a la forma no lineal del campo eléctrico de la luz $E$
$$P=\varepsilon_0  \chi^{(1)}E + \varepsilon_0 \chi^{(2)}E^2 +  \varepsilon_0 \chi^{(3)}E^3+\dots$$
</li>
</ul>
</div>

<div style="float:left; width:100%">
<ul>
<li> 2nd order susceptibility $$\chi^{(2)} \approx 1.94\times10^{-12}\;m/V$$
</li>
<li> 3rd order susceptibility$$\chi^{(3)} \approx 3.78\times10^{-24}\;m^2/V^2$$
</li>
<li> Para fibras de <strong>sílice</strong> $SiO_2$ el effecto de segundo orden es despreciable
</li>
<li> $\chi^{(3)}$ está asociada al <strong>effecto Kerr</strong>
</li>
<li>Polarizacion total: lineal + no lineal 
$$P(\omega) = \varepsilon_0 \chi^{(1)}E(\omega)+3\varepsilon_0\chi^{(3)}|E(\omega)|^2E(\omega)  $$
</li>
<li>Effective susceptibility
$$\chi_{eff} = \chi^{(1)}+3\chi^{(3)}|E(\omega)|^2 $$
</li>
<li>Está ligada al índice de refracción 
$$\bar{n} = 1+\chi^{(3)}=\bar{n}_0 +\bar{n}_2\;I$$
</li>
</ul>
</div>


Óptica no lineal: effecto Kerr 
========================================================
 

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li> Descubierta por John Kerr en 1875
</li>
<li> Describe situaciones donde el índice de refracción depende de el campo eléctrico como 
$$\bar{n}(\omega, |E|^2)=\bar{n}_0(\omega) + \bar{n}_2(\omega)|E|^2$$
</li>
<li>Para sílice es $1.3\times10^{-22}\; m^2/V^2$
</li>
</ul>
</div>


Derivación de la ecuación de Schrödinger
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li>En medio Kerr el índice de refracción depende de la intensidad del campo eléctrico $I(t)$
$$\bar{n}(t)=\bar{n}_0 + \bar{n}_2 I(t), \;\;\;I(t)=2\bar{n}_0\varepsilon_0 c |A(z,t)|^2$$
</li>
<li> y 
$$E(z,t)=A(z,t)e^{i(\omega_0 t-\beta _0 z)}$$
</li>
<li>Aplicando transformada de Fourier del campo óptico
$$E(z,t)=\int_{-\infty}^{\infty} \tilde{E}(z,\omega)e^{i(\omega t - \beta z)} \;d\omega$$
</li>
<li>Considerar la expansion de Taylor de la constante de propagación
$$\beta(\omega) = \beta_0 + \beta _1 (\omega - \omega_0 )+\frac{1}{2}\beta_2 (\omega - \omega_0)^2 + \Delta \beta_{NL}$$
</li>
<li>Sustituir
$$\begin{align}
E(z,t)=&e^{-i\beta_0 z}\int_{-\infty}^{\infty} \tilde{E}(z,\omega)e^{i\omega t - i\beta_1 z \Delta \omega - i\frac{1}{2}\beta_2 z \Delta \omega^2-iz\Delta\beta_{NL} } \;d(\Delta\omega)\\
=&e^{i(\omega_0t-\beta_0 z)}\int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega)e^{it\Delta\omega-i\beta_1 z \Delta \omega - i\frac{1}{2}\beta_2 z \Delta \omega^2-iz\Delta\beta_{NL}} \;d(\Delta\omega)\\
\equiv&e^{i(\omega_0 t-\beta _0 z)} A(z,t)
\end{align}$$
</li>
</ul>
</div>

<div class='footer'>
<small>Wartak, "Computational photonics", Cambridge Univeristy Press, 2013</small>
</div>



Derivación de la ecuación de Schrödinger
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li> Hemos definido 
$$A(z,t) = \int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega)e^{it\Delta\omega-i\beta_1 z \Delta \omega - i\frac{1}{2}\beta_2 z \Delta \omega^2-iz\Delta\beta_{NL}} \;d(\Delta\omega)
=\int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega)e^{ig(z,t)} \;d(\Delta\omega)$$
</li>
<li> Derivar
$$\begin{align}
\frac{ \partial A(z,t)}{\partial t}  =&\int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega)i\Delta \omega e^{ig(z,t)} \;d(\Delta\omega) \\
\frac{ \partial^2 A(z,t)}{\partial t^2}  =&\int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega)(i\Delta \omega)^2 e^{ig(z,t)} \;d(\Delta\omega) \\
\frac{ \partial A(z,t)}{\partial z}  =&\int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega)(-i\beta_1  \Delta \omega - i\frac{1}{2}\beta_2 \Delta \omega^2-i\Delta\beta_{NL}) e^{ig(z,t)} \;d(\Delta\omega) 
\end{align}$$
</li>
<li>Combinar
$$\frac{ \partial A(z,t)}{\partial z} +  \beta_1 \frac{ \partial A(z,t)}{\partial t} -i\frac{1}{2}\beta_2 \frac{ \partial^2 A(z,t)}{\partial t^2} =  \int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega) \left[  ... \right]e^{ig(z,t)} \;d(\Delta\omega)$$
</li>
<li> La expresion en $[...]$ es $-i\bar{n}_2k_0 I$
</li>
<li>Entonces
$$\frac{ \partial A(z,t)}{\partial z} +  \beta_1 \frac{ \partial A(z,t)}{\partial t} -i\frac{1}{2}\beta_2 \frac{ \partial^2 A(z,t)}{\partial t^2} =  -i\bar{n}_2k_0I \int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega) e^{ig(z,t)} \;d(\Delta\omega)$$
</li>
</ul>
</div>

<div class='footer'>
<small>Wartak, "Computational photonics", Cambridge Univeristy Press, 2013</small>
</div>


Derivación de la ecuación de Schrödinger
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li>
</li>
<li>Entonces
$$\frac{ \partial A(z,t)}{\partial z} +  \beta_1 \frac{ \partial A(z,t)}{\partial t} -i\frac{1}{2}\beta_2 \frac{ \partial^2 A(z,t)}{\partial t^2} =  -i\bar{n}_2k_0 I \int_{-\infty}^{\infty} \tilde{E}(z,\omega_0 +\Delta \omega) e^{ig(z,t)} \;d(\Delta\omega)$$
</li>
<li>
$$``\qquad" \qquad =  -i\bar{n}_2k_0 I A(z,t)$$
</li>
<li> Por lo tanto 
</li>
</ul>
</div>


<div style="border: 1px solid blue;border-color:#287EC7; color:black;position: fixed; top:40%; text-align:center;left:5%;padding:1em;" class="fragment">
<ul style="list-style-type:none;">
<li>
$$\frac{ \partial A(z,t)}{\partial z} +  \beta_1 \frac{ \partial A(z,t)}{\partial t} -i\frac{1}{2}\beta_2 \frac{ \partial^2 A(z,t)}{\partial t^2} = i\gamma |A(z,t)|^2A(z,t)-\frac{\alpha}{2}A(z,t)$$
</li>
</ul>
</div> 


<div class='footer'>
<small>Wartak, Computational photonics, Cambridge Univeristy Press, 2013</small>
</div>


Ecuación discreta no lineal de Schrödinger
========================================================


<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li> 
Considere la dinámica de propagación en un arreglo <b>discreto</b> de fibras ópticas descrita por la ecuación discreta de Schrödinger no lineal (DNLS)
$$\begin{equation}\label{eq:DNLSE}
i \frac{dc_n}{dz} =  \epsilon_n c_n  - k(c_{n+1}+c_{n-1}) + \sigma|c_n|^2c_n,
\end{equation}$$
</li>
<li>$c_n$: amplitudes complejas,  en el sitio $n$, que dependen de la dirección de la variable de propagación $z\in\mathbb{R}$
</br>$k$: fuerza uniforme de acoplamiento con el vecino más cercano
</br>$\epsilon_n$ perfil de índice de refracción in-situ
</br>$\sigma$: fuerza de no linealidad
</li>
<li>$\diamond$ El hamiltoniano que da lugar a las ecuaciones de movimiento viene dado por la ecuación
$$\begin{equation}\label{eq:hamiltonian}
H_D = \sum_n \epsilon_n|c_n|^2 + \frac{\sigma}{2}|c_n|^4 - k\left(c_{n+1}c_n^*+c^*_{n+1}c_n  \right).
\end{equation}$$
</li>
<li>Configuración ideal de guías de ondas ópticas idénticas, donde $\epsilon_n$ es una constante fija $\epsilon$.
</li>
</ul>
</div>


<div style="float:left; width:60%;padding-left:20%" class="fragment">
<img src="figs/flatarray.png" style="width:100%" alt="Surface with positive orientation"><div style="float:left; width:100%">
</div>
<p style="text-align:center"><small>
Representación esquemática de un arreglo de guías de ondas ópticas planar. $r_n$ es el radio de cada núcleo en particular
</small></p>
</div>


Parity-Time (PT) simetría
========================================================

<div style="float:center; width:100%">
<ul style="list-style-type:none;">
<li>
<table style="font-size: 40px; width: 100%; text-align: center; " class="minimalistBlack">
<tr>
  <th>Quantum Mechanics</th>
  <th>Optics</th>
</tr>
<tr>
  <td>Schrödinger equation</td>
  <td>Paraxial equation</td>
</tr>
<tr>
  <td>$i\hslash\frac{\partial\Psi}{dt}+\frac{h^{2}}{2m}\frac{\partial^{2}\Psi}{\partial x^{2}}-V\left(x\right)\Psi=0$</td>
  <td>$i\lambda\frac{\partial E}{\partial z}+\frac{\lambda^{2}}{2}\frac{\partial^{2}E}{\partial x^{2}}+n\left(x\right)E=0$</td>
</tr>
<tr>
  <td>time </td> <td>propagation distance</td>
</tr>
<tr>
  <td>$t$</td>  <td>$z$</td>
</tr>
<tr>
  <td>Plank's constant </td> <td>Wavelength</td>
</tr>
<tr>
  <td>$\hslash$</td>  <td>$\lambda=\frac{1}{k}$</td>
</tr>
<tr>
  <td>Probability amplitude </td> <td>Electric field envelope</td>
</tr>
<tr>
  <td>$\Psi\left(x,t\right)$</td>  <td>$E\left(x,z\right)$</td>
</tr>
<tr>
  <td>Complex potential</td> <td>Complex refraction</td>
</tr>
<tr>
  <td>$V\left(x\right)=V_{R}\left(x\right)+iV_{I}\left(x\right)$</td>  <td>$n\left(x\right)=n_{R}\left(x\right)+in_{I}\left(x\right)$</td>
</tr>
</table>
</li>
</ul>
</div>


Parity-Time (PT) simetría
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none">
<li>Bender consideró si un sistema hamiltoniano mecánico cuántico con un potencial complejo puede tener un espectro real. 
</li>
<li><center>
P: $\hat{x}\rightarrow -\hat{x}\;$ y $\;\hat{p}\rightarrow -\hat{p}$</br>
T: $\hat{x}\rightarrow \hat{x}\;$, $\;\hat{p}\rightarrow -\hat{p}\;$, y  $\;i\rightarrow -i$ </center>
</br>$\hat{p}$: momentum operator.
</br>$\hat{x}$: space operator.
</li>
<li>
<p style="border:3px; border-style:solid; border-color:#287EC7; padding: 1em;"> <strong> Condición de PT-simetría</strong>
$$V(x) = V^*(-x)\qquad n(x)= n^*(-x)$$ 
</p>Esto se traduce en el potencial complejo cuya parte real es una función par mientras que la parte imaginaria es impar.
</li>
<li> $\circ$ Hamiltoniano PT-simétrico
<ul>
<li> Puede tener un eigen-espectro real
</li>
<li> Eigen-estados PT-simétricos puede que occurran para cierto régimen paramétrico
</ul>
</li>
</ul>
</div>


<div class='footer'>
<small>Bender, "Making sense of non-Hermitian Hamiltonians", Reports on Progress in Physics 2007</small>
</div>


Parity-Time (PT) simetría
========================================================

<div style="float:left; width:50%" class="fragment">
Sistemas ópticos acoplados convencionales y PT-simétricos. 
<img src="figs/nphys1515-f1.png"><div style="width:100%">
</div>
<p style="text-align:center"><small>Rüter et al., Nature Physics, 2010
</small></p>
</div>

<div style="float:left; width:35%" class="fragment">
Propagación del haz en dos guías de ondas PT-simétricas no lineales.
<img src="figs/ramezani_img.jpg" alt="Metasuperficie"><div style="float:center; width:100%">
</div>
<p style="text-align:center"><small> Ramezani et al. PR A 2010
</small></p>
</div>

<div style="float:left; width:60%;padding-left:20%" class="fragment">
Dispersor recubierto con una metasuperficie ultrafina con pérdida y ganancia equilibradas. 
<img src="figs/invisibility.jpg" alt="Metasuperficie"><div style="float:center; width:100%">
</div>
<p style="text-align:center"><small>Sounas et al., Phys. Rev. Applied 2015
</small></p>
</div>


Fibras  multi-núcleo helicoidales y PT-simétricas
========================================================

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li> Considere la dinámica de propagación del haz en una fibra discreta de múltiples núcleos de $N$ sitios dispuestos igualmente espaciados en un anillo de radio $R_0$ donde cada núcleo tiene un radio $r_0$, descrito por las ecuaciones de modos acoplados
Dinámica de propagación en una matriz discreta de fibras ópticas descrita por la ecuación discreta de Schrodinger no lineal (DNLS)
$$i\frac{{dc_{n}}}{dz}=k\left(e^{-i\phi}c_{n+1}+e^{i\phi}c_{n-1}\right)+i\gamma_{n}c_{n}+\sigma|c_{n}|^{2}c_{n}$$
</li>
<li>$c_n$: representa amplitudes complejas,  en el sitio $n$, que dependen de la dirección de la variable de propagación $z\in\mathbb{R}$
</br>$k$: fuerza uniforme del acoplamiento con el vecino más cercano
</br>$\phi$: Peierls phase 
</br>$\gamma_n$:tasa de ganancia óptica ($\gamma_n> 0$) o pérdida ($\gamma_n <0$) 

</li>
</ul>
</div>


<div style="float:left; width:50%;padding-left:25%" class="fragment">
<img src="figs/twisted_multicore.png" alt="Esquema de una fibra optica torcida"><div style="float:center; width:100%">
</div>
<p style="text-align:center"><small>Esquema de fibra óptica helicoidal con PT-simétrica
</small></p>
</div>


Title
========================================================


<div style="float:left; width:40%" class="fragment">
<img src="figs/pt_wave_guide_ring_array.png" alt="Esquema de una fibra óptica torcida"><div style="float:center; width:100%">
</div>
</div>

<div style="float:left; width:100%">
<ul style="list-style-type:none;">
<li>
</li>
<li>
</li>
<li>
</li>
</ul>
</div>











