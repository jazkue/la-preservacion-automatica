---
title: "La Preservación Involuntaria"
author: "Javier de Azkue"
output:
  # word_document:
    # reference_doc: styles/style.docx
  custom_document:
    path: /Exports/test.pdf
    toc: true
    pandoc_args: ["--csl", "references/apa.csl"]
toc-title: "Indice"
header-includes: |
    \usepackage{sectsty}
    \sectionfont{\clearpage}
bibliography: references/bib.bib
---

# Resumen
La Preservación Involuntaria es un trabajo de tesis que estudia técnicas híbridas de arte digital, entendiendo esta hibridación como una combinación de arte por computadora con procesos, formatos y soportes analógicos no-digitales que pueden llevar a la preservación en el tiempo de estas obras electrónicas, voluntaria o involuntariamente. La tesis estudia estos conceptos, analiza las problemáticas de la preservación digital y propone un camino de experimentación y reflexión de arte híbrido, con técnicas ligadas a la fotografía, la animación y la programación.

En la tesis se analizan las diferencias entre preservación y acceso, los archivos cinematográficos, los archivos de internet, las obras de artistas audiovisuales independientes y su distribución, el avance tecnológico en el campo de la informática en paralelo a las prácticas y experimentaciones artísticas, la piratería digital, y hasta el avance, proliferación y ocaso de los Token No Fungibles (NFTs). Al mismo tiempo, se estudian autores con prácticas artísticas o archivísticas en línea con la tesis para ilustrar el estilo formal y estético al que se apunta investigar.  

En el campo práctico se propone un trayecto de experimentación híbrido entre analógico y digital, a través de obras por computadora con iteraciones y generaciones en distintos formatos y medios. La propuesta busca evidenciar el dispositivo, reflexionar sobre la historia de los soportes y las tecnologías, y sumar al universo estético y formal de la tesis. En estas relaciones se busca que el interlocutor reflexione sobre el valor de la responsabilidad y la dimensión del tiempo en la preservación digital.  


# Prólogo

Nací en 1992 en la ciudad de San Carlos de Bariloche. Al estar tan lejos de la capital siento que siempre tuvimos cierto “delay” con la llegada de algunas tecnologías, lo que creo que me hizo creativo y resolutivo, y también me hizo conocer diferentes generaciones de computadoras y dispositivos audiovisuales. A pesar de ser un millenial tengo recuerdos de estar en el techo de mi casa girando la antena de TV para mejorar la señal del único canal de aire que nos llegaba, o de limpiar los cabezales de la videocasetera y hacer las conexiones de video con la tele.  

Cuando era muy chico un tío de Buenos Aires nos instaló un par de videojuegos en una vieja laptop Toshiba del 89 que había traído mi papá de afuera. Estábamos entonces jugando videojuegos de los 80 en los años 90, cuando ya estaban estrenadas la Nintendo 64 y la Playstation.  

Por otro lado, teníamos cientos de fotos en papel y en diapositivas, las cuales proyectábamos un par de veces al año sobre una tabla blanca. Recuerdo que había un par de diapositivas de la película Toy Story que me llamaban mucho la atención. Esa película que yo tenía en VHS aparecía de repente en un fotograma, proyectada en casa en grande y con luz.  

Cuando terminé jardín de infantes me regalaron un video con grabaciones nuestras. Recuerdo que de este video me llamaban la atención los títulos electrónicos que precedían a cada parte, no entendía cómo sería el proceso y me fascinaba. Recuerdo también mi sorpresa cuando en el primario se proyectó un corto sobre Facundo Quiroga que habían filmado los de 7mo grado con la ayuda del papá de alguien, que trabajaba en publicidad en Bariloche. Me sorprendía por un lado la proyección “hogareña”, y por otro lado, de nuevo, los títulos “electrónicos” del film. Más adelante mi madre volvería de Suecia por trabajo y nos traería una cámara digital, y con su capacidad de grabar video, sería mi puerta de entrada a mis primeros experimentos audiovisuales.  

Años más tarde me mudé a Buenos Aires y estudié Diseño Imagen y Sonido en la UBA. Como todos (supongo), entré queriendo dirigir como Tarantino, pero al final terminé más interesado en la técnica. Para la tesis de la carrera estaba interesado en el tema de “la resolución”: había visto en el BAFICI del 2014 una restauración en 4k de La Épica del Everest, de John Noel, y me fascinó poder ver esas imágenes del pasado en “tan buena calidad”. Quería trabajar en esta línea, me interesaba el género del found footage.  

Para esto, yo sabía de la existencia entre mi familia de una película en 16 mm de mi abuelo Horacio. “El viaje del Henrietta”: un registro amateur de una travesía al extremo sur de sudamérica a bordo de un velero en 1938. Le habían prestado a mi abuelo una cámara y se unió a la tripulación después de terminar sus estudios de arquitectura. Increíbles imágenes del Estrecho de Magallanes, los glaciares en Punta Arenas y las canoas de los pueblos Káwescar embarcando el velero para pedir comida y cigarrillos. Unas imágenes muy inspiradoras. En los 90 algún familiar se encargó de pasarlo a VHS, y en 2014 un primo lo digitalizó y compartió por mail. Me interesaban las imágenes, pero más aún me interesaba encontrar el original en fílmico. Apareció en la casa de una tía en San Luis, y fue traído por un tío a Buenos Aires.  

La película estaba muy mal, padecía de síndrome del vinagre, un proceso de deterioro que actúa en películas de acetato de celulosa cuando son expuestas a condiciones adversas de humedad y calor. La película libera ácido acético, el responsable de su particular olor a vinagre y del deterioro de la película. Es un proceso irreversible y que se contagia de película a película a través del aire.  

El proyecto se transformó en otra cosa: pasé de la búsqueda por la “buena resolución” al interés de salvar esas imágenes de la destrucción total (al menos en su forma fílmica). Como la película no se podía reproducir por medios mecánicos ni mandar a digitalizar, terminé diseñando un sistema de digitalización cuadro por cuadro con un escáner de diapositivas, inspirado en el trabajo de un alemán entusiasta del film llamado W. Kurz[^1]. El proyecto derivó luego en una videoinstalación y ganó algunos premios y reconocimientos[^2].  

Este trabajo fue muy grato, y me acercó al Museo del Cine de Buenos Aires a través de Carolina Cappa, investigadora de la institución. Empecé como voluntario y luego conseguí un contrato y me desarrollé en la cineteca del museo. En determinado momento aquí también pusimos en práctica el mismo método de digitalización que había usado en Henrietta para digitalizar distintos materiales. El mismo sistema se utilizó para digitalizar los fotogramas del libro Nitrato argentino, una historia del cine de los primeros tiempos, editado por C. Cappa y el museo[^3]. Este sistema de digitalización y conservación del 2014 me acompañó hasta el día de hoy y es, en una versión más nueva, una de las herramientas de experimentación que se llevará a cabo en la presente tesis.  

En paralelo cursé la Maestría en Artes Electrónicas en la Universidad Nacional de Tres de Febrero, donde me desarrollé en programación, diseño de instalaciones interactivas y electrónica enfocada al arte, lo que generó un estilo híbrido entre el campo audiovisual (digital/analógico) y el campo interactivo de tiempo real.  

Cuando uno trabaja con distintos soportes físicos y digitales al mismo tiempo tiende a dejar un trazo en el proceso. Se suceden distintas copias, iteraciones y generaciones, y el proceso perdura, se preserva, quizás guardado en un cajón, en un disco rígido, en un papel o en la nube. Este tipo de hibridación e iteración genera una preservación involuntaria: las decisiones estéticas y técnicas que uno toma son más importantes de lo que uno cree, y cuando menos lo esperemos, quizás determinan la única copia que queda de algo importante que queremos recordar.  

[^1]: https://wkurz.com/home/productsEN.html. Accedido 6 de febrero de 2024. Ver https://vimeo.com/22015773  
[^2]: Un Paisaje de Acontecimientos, CC San Martín, Buenos Aires (2016); Mención especial en Festival FAB, Bariloche (2015); Mención especial en Festival de Cine Latinoamericano Rosario (2015); FASE7, Centro Cultural Recoleta, Buenos Aires (2015); Orphan Films, MALBA, Buenos Aires (2015); Premio mejor cortometraje experimental Festival REC, La Plata(2015); Let it VJ Club Cultural Matienzo (2015); Muestra Satélite XI en el Centro Hipermediático Experimental Latinoamericano (2014).  
[^3]: Cappa, Carolina. et al. Nitrato argentino, una historia del cine de los primeros tiempos. Museo del Cine, 2019.   


# Introducción
## Una obligación incuestionable
En el prólogo al libro Clasificar para Preservar del investigador español en cine Alfonso del Amo García se plantea la “obligación incuestionable” de las civilizaciones de “preservar la memoria y la historia”. El texto asevera que “mediante la palabra repetida y atesorada en piedra, pergamino y papel, sabemos quiénes somos y cuál es nuestro lugar en el mundo” [@amogarciaClasificarParaPreservar2008]. Es un libro muy reconocido y consultado en el ambiente de los archivos y la preservación cinematográfica en la mayoría de los países de habla hispana. Considerando las diferentes realidades socioeconómicas e históricas de los archivos del mundo, el autor presenta el libro no como un “manual de preservación” sino como una especie de guía y manifiesto. Además de resaltar la importancia del compartir y el acceso a las películas, prioriza la clasificación en los archivos y el conocimiento técnico de los materiales como fuente de poder frente a la acción implacable del tiempo. De la era del cine silente en Estados Unidos se estima que al menos el 70% de las películas están completamente perdidas [@pierceSurvivalAmericanSilent2013, p.136].

Con internet y la ley de Gordon Moore que estima que aproximadamente cada 2 años se duplica la cantidad de transistores en un microchip, el mundo estricto de los archivos se vio muy transformado. La existencia de los documentos, los sitios web y las imágenes dependen muchas veces de compañías privadas como Google o Facebook para sobrevivir, aunque existen excepciones que se verán más adelante, como el proyecto sin fines de lucro Internet Archive, o el proyecto de código abierto y descentralizado de sistema de archivos IPFS, Inter Planetary File System. Y hay un elemento interesante en toda esta tormenta tecnológica y es la colectividad y el carácter “abierto” de las computadoras e internet. En la web 2.0 se prioriza la creación de contenido por parte del usuario a través de sitios y aplicaciones.  

Por otro lado, así como Alfonso del Amo Cuarón destaca también en su guía las bondades de rescatar materiales fílmicos dando acceso a ellos (proyectándolos), es provechoso compararlo con la piratería, el exceso de imágenes, los remixes, los torrents. Hito Steyerl habla de la “imagen pobre” como “copias en movimiento”. La imagen pobre “...transforma la calidad en accesibilidad, el valor de exhibición en valor de culto, las películas en clips, la contemplación en distracción. La imagen es liberada de las criptas del cine y los archivos y empujada a la incertidumbre digital a costa de su propia sustancia" [@steyerlCondenadosPantalla2014]

Internet entonces no es sólo fuente de contenido sino también de inspiración. En esta dinámica, los creadores independientes pueden subir y compartir sus obras, y por la sola inercia de las tecnologías (y la capacidad de las computadoras) muchas obras perduran en el tiempo de forma automática. Hay excepciones a la regla: formatos irreproducibles, actualizaciones de hardware sin retrocompatibilidad, páginas web caídas, sitios de guardado de archivos como Megaupload eliminados por cuestiones legales, codecs de video corrompidos, o simplemente bugs.

## La Preservación Involuntaria
Un realizador experimental encuentra una película Super 8 junto a la basura caminando por su barrio. Inspirado, vuelve a su casa y decide pintar el celuloide a mano con marcadores y pinceles, influenciado por sus ídolos Len Lye, Norman McLaren y  Stan Brakhage. Digitaliza las películas cuadro a cuadro con un scanner de su casa y sin necesidad de un proyector reconstruye el movimiento en su computadora. Satisfecho con el resultado hace un backup en un disco externo y sube el video a Instagram y Vimeo. Recibe un par de likes. Algunos foros de animación publican su creación e incluso descubre que otros usuarios lo descargan y lo vuelven a subir.  

Es 2020: el realizador lee sobre el auge de las cripto y los NFT. Decide mintear su animación en la blockchain y sin entender mucho la pone a la venta en www.HicEtNunc.xyz en formato gif. Este .gif queda para siempre loopeando en estos sitios, respaldado por tecnologías de bloques, algoritmos y sistemas de guardado IPFS (Inter Planetary File System). Un anónimo le compra la obra por 20 tezos, la moneda que utiliza esa red. La obra ya se reprodujo y copió cientos de veces.  

Pasan los años, es el año 2050. El disco rígido se rompió hace mucho y los NFT nunca resultaron, y los foros de animadores experimentales están en su mayoría caídos. Y quizás no se supo más de este realizador experimental, sus discos y herramientas terminaron en un tacho de reciclables, y los foros solo existen en la Wayback Machine de Archive.org, que ahora es paga. Quizás la blockchain conserva el hash de la transacción, y quizás con un poco de búsqueda y esfuerzo y gracias a las redes descentralizadas el archivo sigue vivo en algunas computadoras del mundo. O quizás nada de esto sigue funcionando, pero aparece el Super 8 escondido en un cajón, en perfecto estado.  

Esta es la “hibridación” que me interesa. Como se menciona en el prólogo, uno podría pensar que en estas escaladas tecnológicas y en el flujo de trabajo de quienes “crean arte y lo suben a la web” hay una actitud de preservación involuntaria que a la larga, quizás, es una salvación para las obras digitales.  

Pero preservar es un verbo ambiguo: a pesar de su definición más pura de “conservar la forma original de algo a lo largo del tiempo”, en la idea que venimos describiendo de autores que preservan sus obras por utilizar determinados medios y soportes, no parece ocurrir intencionalmente. Sin embargo, es esa justamente la base de la búsqueda: el trazo que dejan los distintos soportes físicos y digitales; las copias, iteraciones y generaciones; y el proceso que perdura y se preserva.  

En este tipo de hibridación e iteración es que observo una preservación involuntaria: las decisiones estéticas y técnicas que quizás determinan la única copia que queda de algo importante que queríamos recordar.  

# Bibliografía