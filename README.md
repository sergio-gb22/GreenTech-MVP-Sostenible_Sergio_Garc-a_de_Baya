# GreenTech-MVP-Sostenible_Sergio_García_de_Baya
    
Concepto	            Original	          Refactorizado    	          Reducción
Peso total	          ~398 KB	               ~10.8 KB	                   97.3%
Peticiones HTTP	        6	                    1 (imagen)	                83%
Dependencias externas  	5	                    0	                          100%
Imagen hero	          3000px (~2.5 MB)	      Responsive (180-500 KB)     ~90%
Fuentes	            Montserrat (descarga)    	System fonts	              100%
Iconos	            Font Awesome (63 KB)	    SVG inline (0.5 KB)	        99.2%
JavaScript	         3 librerías (317 KB)	      0	                        100%


##Impacto Ambiental Estimado
Por 10,000 visitas mensuales:

Datos ahorrados: 3.87 GB
Energía eléctrica ahorrada: ~0.65 kWh
CO₂ equivalente evitado: ~0.28 kg
Batería de usuario ahorrada: ~45 minutos de navegación

##Principales Cambios Técnicos
###1. Eliminación de Dependencias
diff
- Bootstrap CSS (187 KB)
- Font Awesome (63 KB)
- Google Fonts (variable)
- jQuery (87 KB)
- Bootstrap JS (176 KB)
- Moment.js (54 KB)
+ CSS nativo con variables
+ SVG inline para iconos
+ Fuentes del sistema
+ JavaScript vanilla minimalista

###2. Optimización de Imágenes
html
<img srcset="imagen-480w.jpg 480w,
             imagen-1024w.jpg 1024w,
             imagen-1920w.jpg 1920w"
     sizes="(max-width: 480px) 480px,
            (max-width: 1024px) 1024px,
            1920px"
     loading="lazy">
###3. Footer Estático vs Dinámico
diff
- $(document).ready(function() {
-   const anio = moment().format("YYYY");
-   $("body").append("<footer>...</footer>");
- });
+ <footer>GreenTech Solutions © 2025</footer>

##Referencias Bibliográficas
[1] W3C, "Web Sustainability Guidelines (WSG) 1.0," World Wide Web Consortium, 2023. [Online]. Available: https://www.w3.org/TR/wsgl/

[2] Green Software Foundation, "Green Software Practitioner Course," 2024. [Online]. Available: https://learn.greensoftware.foundation/

[3] R. Verdecchia, P. Lago, I. Malavolta, and G. Procaccianti, "Green IT and Green Software Engineering: A Systematic Mapping Study," arXiv preprint arXiv:2102.04945, 2021. [Online]. Available: https://arxiv.org/abs/2102.04945

Autor: Sergio García ce Baya
Fecha: 23 de Marzo 2026
Versión: 1.0 - MVP Sostenible
Repositorio: GreenTech-MVP-Sostenible_Sergio_García_de_Baya
