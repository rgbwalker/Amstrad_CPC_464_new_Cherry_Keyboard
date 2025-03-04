# Amstrad_CPC_464_new_Cherry_Keyboard
Mechanical PCB keyboard for CPC 464 with Cherry switches




# Scroll down to see the english version.

# Versión en español:

# Contando la aventura.

![image](/_IMAGENES_/Teclado_2D_V1_0.jpg)

Fue en marzo de 2024 cuando acudí por primera vez a “Retro Parla”. Para quien no conozca este evento, es una reunión de usuarios de “informática retro” al sur de Madrid, a la que animo a ir a todo el mundo.

Por ejemplo, entre muchas de las cosas que descubrí había un Amstrad CPC 464 montado a mano desde cero. Todos los componentes eran nuevos y estaban soldados a mano en una PCB recreada basada en el CPC 464 “teclas altas”, con una carcasa artesanal fabricada con metacrilato transparente. Por su parte, el teclado estaba hecho a base de teclas tipo Cherry MX, cableadas y montadas sobre un bastidor realizado en impresora 3D a medida. Incluía un cpcduino con sus correspondientes pantalla y teclas de control, que suplía al casette original. Su propio circuito de audio, con interruptor, altavoz y control de volumen.

Todo aquello funcionaba a la perfección, este Amstrad tan impresionnte era obra de Manuel Cuenca,  (@manuelcuencammchip).

En cuanto lo vi me interesó, y acosé con mil preguntas a Manuel Cuenca que muy amablemente respondió. Y me dijo que la PCB era obra de Bob´s Bits y se podía conseguir en tindie:

https://www.tindie.com/products/bobsbits/amstrad-cpc464-replica-pcb/

Si echáis un vistazo al enlace veréis que es una recreación genial y 100% funcional de los primeros modelos CPC 464 “teclas altas”. ¡Buen trabajo Bob!

Si queréis conocer un poco más del proceso, a cargo del mismo Manuel Cuenca, en su canal de Youtube encontrareis una muy buena explicación:

https://www.youtube.com/watch?v=fhV4mdnoMto

Por mi parte no tardé mucho en decidirme a fabricar otro para mi. Eso si, conté con la inestimable ayuda y paciencia de Manuel Cuenca.

Como punto de partida, la PCB la conseguí en la web de tindie de Bob´s Bits, a la que poco a poco se fueron sumando el resto de componentes.

Llegó entonces el momento de enfrentarse a la fabricación del teclado. Pero, como no tenía experiencia en diseño con aplicaciones e impresoras 3D, descarté la posibilidad de hacer un soporte o marco para sostener los pulsadores tipo Cherry MX.

Y tras buscar alternativas, preguntando aquí y allá, terminé por decidirme (o más bien debería decir aventurarme a probar suerte… jejeje) a hacer yo mismo una PCB para el teclado del CPC 464.

En este punto he de agradecer al usuario de Telegram llamado Mac, que me habló de EasyEda y me animó a hacer este proyecto. EasyEda es la aplicación de diseño online del fabricante PCBs, JLCPCB (entre otras múltiples cosas). Para poner las cosas en contexto, aquí hay que decir que NUNCA ANTES había diseñado una PCB ni tenía experiencia previa en abordar el diseño de toda una placa. Sí que me había aventurado a alguna prueba con KiKad, aunque en su momento me pareció algo mas complicado de lo que ha resultado EasyEda. Finalmente, descargué la versión offline de la aplicación y me puse a investigar cómo era el proceso.

Pude consultar el esquema eléctrico de la matriz del teclado en el Manual de Servicio del CPC 464, el cual podéis encontrar por la red. En cpcwiki se puede descargar del siguiente enlace:

https://www.cpcwiki.eu/index.php/Service_Manuals

En la página 11 del manual encontrareis el esquema de la matriz del teclado.

![image](/_IMAGENES_/Matriz_Teclado.jpg)

Tras semanas de pruebas, pruebas y más pruebas con el propio programa, tras varias versiones y más versiones, comprobaciones y más comprobaciones, además de solucionar dudas y errores, por fin obtuve una versión final que parecía funcional. Y aquí está el resultado.

Eso sí, he de decir que no habría podido sin la ayuda de otro compañero de Telegram, Abalore, quien también me animó y aconsejó con el asunto, el cual posee un interesante canal de YouTube donde muestra algunos de sus proyectos:

https://www.youtube.com/@abalore

Y a quien agradezco desde aquí su apoyo y ayuda.

# Objetivo.

Este NO es un teclado pensado para SUSTITUIR el teclado original de un CPC 464. Y no lo es por varios motivos. El principal objetivo es poder darle su propio teclado a un CPC 464 realizado desde cero, con lo cual no tiene por qué ser “idéntico milimétricamente” al original. De hecho, con componentes estándar del mercado NO PUEDE SER IGUAL.

Entre las diferencias de este teclado con el original tenemos:

- Compuesto de pulsadores de 2 pines tipo Cherry MX: sencillos sin luces led ni RGB y no hay membrana como en el original.
- Teclas (caps) estandar, lo cual supone:
	* Tecla “ENTER” formato ISO: más pequeño que el original, lo que obliga a que las 	teclas “DEL”, y “SHIFT” derecha sean más pequeñas que las originales, (para que 	terminen todas la teclas alineadas sin que sobresalgan por el costado derecho unas por 	encima de otras).
	* Tecla “DEL” de 1 unidad.
	* Tecla “SHIFT”, derecha de 1,75 unidades.
	* Tecla “SPACE”, de 7 unidades, (la original es de 9 unidades, completamente fuera del 	estándar de hoy día, o al menos no he sido capaz de encontrar nada de ese tamaño). Lo 	que obliga a centrar la tecla “SPACE” y recolocar la tecla “CTRL”.

Por todos estos detalles, NO encajaría esta PCB en la carcasa de un CPC 464 original. O, al menos, no encajaría como un guante como el teclado original. Tampoco los orificios de fijación están pensados para ser usados con la carcasa original.

Aun así, ¿podría usarse en un CPC 464 original?

El conector que va a la PCB principal es el necesario para la versión recreada por Bob´s Bits, que como decía, es como los primeros modelos de “Teclas altas”: con un conector de 20 pines en una sola línea, mientras que las posteriores versiones tienen dos líneas de fajas tipo “flex”.

Todo esto significa que, si lo vas a usar en una placa CPC 464 “Teclas altas”, eléctricamente funcionará, (aunque no encaje en la carcasa). Pero, si lo vas a usar en una de las placas posteriores (yo no lo he hecho), con conector en dos líneas tipo “flex”, sería necesario hacer un adaptador entre ambos conectores. En este caso sería cuestión de ver dónde va cada pista en el conector de 20 pines de una sola línea, o “20x1” para redirigirlo donde tenga que ser en el conector de 2 líneas de “flex”. Pero es algo que yo, repito, no he probado.

# Para fabricarlo.

BOM:

- PCB de teclado: lógicamente… jejeje.
- Cherry MX: de dos pines (los que más te gusten, el mundo Cherry es inmenso).
- Caps: como los Cherry, los que más te gusten mientras cumplan con las especificaciones que he indicado antes.
- Estabilizadores: en total son 3, uno para el “ENTER” tipo ISO, otro para el “SHIFT” izquierda, de 2,25 unidades y otro para el “SPACE”, de 7 unidades.
- Conector SMD de 1x20pin: para conectar a la PCB principal.
- Cable dupont de 20pin hembra hembra.

Yo he usado los siguientes:

- PCB: la que encontrarás aquí mismo.

![image](/_IMAGENES_/Teclado_01.jpg)

- Cherry MX: en total necesitas 74 Cherrys.

![image](/_IMAGENES_/Cherry_Switch_01.jpg)

https://es.aliexpress.com/item/1005005969664035.html?spm=a2g0o.order_list.order_list_main.123.74c7194dZw9qxL&gatewayAdapt=glo2esp

- Caps: mientras cumplan las dimensiones indicadas, elige el que más te guste.

![image](/_IMAGENES_/Teclas_01.jpg)

https://es.aliexpress.com/item/1005006897485536.html?spm=a2g0o.order_list.order_list_main.78.74c7194dZw9qxL&gatewayAdapt=glo2esp

OJO: yo he usado teclas con perfil XDA, ¿el motivo? Veamos este esquema:

![image](/_IMAGENES_/Key_Caps_01.jpg)

Las teclas con perfil XDA, a diferencia de muchas otras de otros perfiles, se pueden intercambiar entre filas del teclado. Esto significa que una tecla que debería ir, por ejemplo, en la fila 1, puede ser colocada en, por ejemplo, la fila 4 sin que haya diferencias estéticas. Y es que las teclas tipo XDA tienen el mismo perfil, altura y forma, e incluso son simétricas horizontal y verticalmente, pudiendo además ser rotadas o colocadas “boca abajo” si fuera necesario.

Esto puede no parecer relevante, pero es RELEVANTE y mucho, ya que las teclas estándar que se pueden adquirir hoy día están pensadas para PC. Ademas el Amstrad CPC tiene otro mapa de teclado diferente con varios signos de puntuación que no coinciden (sin entrar en diferencias entre idiomas tanto de teclados PC como de teclados de Amstrad CPC), por lo que es necesario andar moviendo teclas entre filas adecuando en lo posible al mapa de teclado que le pongas al CPC464 (que dependerá de la ROM que tenga la PCB principal).

La distribución y las medidas de las teclas a las que hay que prestar más atención, por ser de una medida superior a 1 unidad, o por haber sufrido cambio de tamaño con respecto al original, es la siguiente:

![image](/_IMAGENES_/Medidas_01.jpg)

- Estabilizadores: tienen que ser del grosor de la PCB, 1,6mm.

![image](/_IMAGENES_/Estabilizadores_01.jpg)

![image](/_IMAGENES_/Estabilizadores_02.jpg)

https://es.aliexpress.com/item/1005004477672434.html?spm=a2g0o.order_list.order_list_main.73.74c7194dZw9qxL&gatewayAdapt=glo2esp

- Conector SMD de 1x20pin: selecciona el tipo 1x20P.

![image](/_IMAGENES_/20pin_SMD_01.jpg)

![image](/_IMAGENES_/20pin_SMD_02.jpg)

https://es.aliexpress.com/item/1005007462247870.html?spm=a2g0o.order_list.order_list_main.53.74c7194dZw9qxL&gatewayAdapt=glo2esp

- Cable dupont de 20pin hembra – hembra: selecciona 10cm-F-F-20pin, o 15cm-F-F-20pin.

![image](/_IMAGENES_/Dupont_20pin_H_H.jpg)

https://es.aliexpress.com/item/1005007032334210.html?spm=a2g0o.order_list.order_list_main.28.74c7194dZw9qxL&gatewayAdapt=glo2esp

# Versiones:

- V1.0. 09/02/2025.
	* Primera version pública.

- V1.2. 04/03/2025.
	* Añadida nueva huella del conector 20pin THT (CP002, cable Dupont a la PCB principal) se mantiene la huella del conector SMD para que el usuario pueda elegir cual de ambas soldar.
 	* Recolocado de orificios de fijacción de manera mas conveniente, se añade alguno nuevo.
  	* Se añade serigrafia con creditos del proyecto.

![image](/_IMAGENES_/Dupont_20pin_H_H.jpg)


# Agradecimientos:


Aunque han sido nombrados a lo largo de este texto, me gustaría reunirlos aquí.

A mi padre y a mi hermano, por ayudarme en el proyecto de montar un CPC 464 entero. Y por animarme a ello.
¡Gracias a ambos!

A Bárbara, por ayudarme a redactar este documento, por aguantar mis pesadas conversaciones sobre ello y hacerlo con una sonrisa.
¡Gracias Bárbara!

A Manuel Cuenca, por haber respondido con suma amabilidad todas mis preguntas en distintas ocasiones.
¡Gracias  Manuel!

A Bob´s Bits por recrear la PCB del CPC 464. Fantástico trabajo.
¡Gracias Bob!

A Mac, por mostrarme EasyEda, animarme a realizar mi propia PCB y aclararme todas las dudas que tuve con el manejo del programa.
¡Gracias Mac!

A Abalore, por su amabilidad y por resolver más de una duda que surgió durante el proceso.
¡Gracias Abalore!



# English version.



# Telling the adventure.

![image](/_IMAGENES_/Teclado_2D_V1_0.jpg)

It was in March 2024 when I went to "Retro Parla" for the first time. For those who don´t know this event, it is a meeting of "retro computing" users in the south of Madrid, which I encourage everyone to go.

For example, among many of the things I discovered was an Amstrad CPC 464 hand assembled from scratch. All new components were soldered by hand on a recreated PCB based on the CPC 464 "high keys", with a hand crafted enclosure made of transparent methacrylate. For its part, the keyboard was made of Cherry MX keys, wired and mounted on a frame made in a custom 3D printer. It included a cpcduino with its corresponding screen and control keys, which replaced the original casette. Its own audio circuit, with switch, speaker and volume control.

All that works fine, this impressive Amstrad was the work of Manuel Cuenca, (@manuelcuencammchip).

As soon as I saw him I was interested, and I harassed Manuel Cuenca with a thousand questions, who very kindly answered. And he told me that the PCB was the work of Bob's Bits and could be obtained on tindie:

https://www.tindie.com/products/bobsbits/amstrad-cpc464-replica-pcb/


If you take a look at the link you will see that it is a cool and 100% functional recreation of the first CPC 464 "high keys" models. Great job Bob!

If you want to know a little more about the process, by Manuel Cuenca himself, on his Youtube channel you will find a very good explanation:

https://www.youtube.com/watch?v=fhV4mdnoMto

For my part, it didn't take long for me to decide to make another one for myself. Of course, I had the invaluable help and patience of Manuel Cuenca.

As a starting point, I got the PCB on the Bob's Bits tindie website, to which the rest of the components were gradually added.

Then it was time to face the manufacture of the keyboard. But, since I had no experience designing with applications and 3D printers, I ruled out the possibility of making a bracket or frame to hold the Cherry MX type switches.

And after looking for alternatives, asking here and there, I finally deciding (or rather I should say venture to try my luck... hehehe) to make a PCB for the CPC 464 keyboard.

At this point I have to thank the Telegram user called Mac, who told me about EasyEda and encouraged me to do this project. EasyEda is the online design application of the PCB manufacturer, JLCPCB (among many other things). To put things in context, here it must be said that I had NEVER BEFORE designed a PCB or had prior experience in tackling the design of an entire board. I had ventured into some tests with KiKad, although at the time it seemed a bit more complicated than EasyEda has turned out. Finally, I downloaded the offline version of the app and started researching what the process was like.

I was able to check the electrical schematics of the keyboard matrix in the CPC 464 Service Manual, which you can find on the web. On cpcwiki you can download it from the following link:

https://www.cpcwiki.eu/index.php/Service_Manuals

On page 11 of the manual you will find the schematic of the keyboard matrix.

![image](/_IMAGENES_/Matriz_Teclado.jpg)

After weeks of testing, testing, and testing with the program itself, after several versions and more versions, checks and more checks, as well as fixing doubts and bugs, I finally got a final version that looked functional. And here's the result.

Of course, I have to say that I would not have been able to do it without the help of another Telegram colleague, Abalore, who also encouraged and advised me on the matter, he has an interesting YouTube channel where he shows some of his projects:

https://www.youtube.com/@abalore

And whom I thank from here for their support and help.


# Objective.

This is NOT a keyboard intended to REPLACE the original CPC 464 keyboard. And it is not for several reasons. The main objective is to be able to give its own keyboard to a CPC 464 made from scratch, so it does not have to be "millimetrically identical" to the original. In fact, with standard components on the market IT CANNOT BE THE SAME.

Among the differences between this keyboard and the original we have:

- Composed of 2 pin Cherry MX type switches: simple without LED or RGB lights and there is no membrane as in the original.
- Standard keys (caps), which means:
	* "ENTER" key ISO format: smaller than the original, which forces the “DEL" and 	right "SHIFT" keys to be smaller than the original ones, (so that all the keys end up 	aligned without protuberances on the right side above each other).
	* "DEL" key of 1 unit .
	* Right "SHIFT" key, of 1.75 units.
	* "SPACE" bar of 7 units, (the original is 9 units, completely out of today's standard,
	or at least I haven't been able to find anything of that size). This forces you to center 	the "SPACE" bar and reposition the "CTRL" key.


For all these details, this PCB would NOT fit into the housing of an original CPC 464. Or, at least, it wouldn't fit like a glove like the original keyboard. The fixing holes are also not intended to be used with the original housing.

Still, could it be used in an original CPC 464?

The connector that goes to the main PCB is the one needed for the version recreated by Bob's Bits, which as I said, is like the first "High Keys" models: with a 20-pin connector in a single line, while the later versions have two lines of "flex" type bands.

All of this means that if you're using it on a CPC 464 "High Keys" board, it will work electrically (even if it doesn't fit into the case). But, if you are going to use them on one of the later boards (I haven't done it), with a connector in two "flex" lines, it would be necessary to make an adapter between both connectors. In this case it would be a matter of seeing where each track goes on the single line 20 pin connector, or "20x1" to redirect it where it needs to be on the 2 line "flex" connectors. But it is something that, I repeat, I have not tried.

To make it.

BOM:

- Keyboard PCB: logically... hehehe.
- Cherry MX: two pin (the ones you like, the Cherry world is immense).
- Caps: the most as long as they meet the specifications I have indicated before.
- Stabilizers: there are 3, one for the ISO type "ENTER”, another for the left "SHIFT", of 2.25 units and another for the "SPACE", of 7 units.
- 1x20pin SMD connector: to connect to the main PCB.
- 20pin female to female dupont cable.

I have used the following:

- PCB: the one you'll find right here.

![image](/_IMAGENES_/Teclado_01.jpg)

- Cherry MX: 74 Cherrys are needed.

![image](/_IMAGENES_/Cherry_Switch_01.jpg)

https://es.aliexpress.com/item/1005005969664035.html?spm=a2g0o.order_list.order_list_main.123.74c7194dZw9qxL&gatewayAdapt=glo2esp

- Caps: As long as it keeps the indicated  dimensions, choose the one likes you.

![image](/_IMAGENES_/Teclas_01.jpg)

https://es.aliexpress.com/item/1005006897485536.html?spm=a2g0o.order_list.order_list_main.78.74c7194dZw9qxL&gatewayAdapt=glo2esp

NOTE: I have used keys with XDA profile, the reason? Take a look at this scheme:

![image](/_IMAGENES_/Key_Caps_01.jpg)

The keys with an XDA profile, unlike many other keys, can be swapped between rows on the keyboard. This means that a key that should go, for example, in row 1, can be placed in, for example, row 4 without any aesthetic differences. XDA keys have the same profile, height and shape, and are even symmetrical horizontally and vertically, and can also be rotated or placed "upside down" if necessary.

This may not seem relevant, but it is RELEVANT and so much, since the standard keys that can be purchased today are designed for PC. In addition, the Amstrad CPC has a different keyboard map with several punctuation marks that don´t match (without going into differences between languages of both PC keyboards and Amstrad CPC keyboards), so it is necessary to move keys between rows adapting as much as possible to the keyboard map that you put to the CPC464 (which will depend on the ROM that the main PCB has).

The distribution and measurements of the keys to which you should pay more attention, because they are larger than 1 unit, or because they have undergone a change in size with respect to the original, is as follows:

![image](/_IMAGENES_/Medidas_01.jpg)

- Stabilizers: they have to be the thickness of the PCB, 1.6mm.

![image](/_IMAGENES_/Estabilizadores_01.jpg)

![image](/_IMAGENES_/Estabilizadores_02.jpg)

https://es.aliexpress.com/item/1005004477672434.html?spm=a2g0o.order_list.order_list_main.73.74c7194dZw9qxL&gatewayAdapt=glo2esp

- 1x20pin SMD connector: select the 1x20P type.

![image](/_IMAGENES_/20pin_SMD_01.jpg)

![image](/_IMAGENES_/20pin_SMD_02.jpg)

https://es.aliexpress.com/item/1005007462247870.html?spm=a2g0o.order_list.order_list_main.53.74c7194dZw9qxL&gatewayAdapt=glo2esp

- 20pin dupont female to female cable: select 10cm-F-F-20pin, or 15cm-F-F-20pin.

![image](/_IMAGENES_/Dupont_20pin_H_H.jpg)


# Thanks:

Although they have been named throughout this text, I would like to bring them together here.


To my father and my brother, for helping me in the project of assembling an entire CPC 464 from scratch. And for encouraging me to do so.
Thank you both!

To Barbara, for helping me write this document, for putting up with my heavy conversations about it and doing it with a smile.
Thank you Barbara!

To Manuel Cuenca, for having answered all my questions with great kindness on different occasions.
Thank you Manuel!

To Bob's Bits for recreating the CPC 464 PCB. Fantastic work.
Thank you Bob!

To Mac, for showing me EasyEda, encouraging me to make my own PCB and clarifying all the doubts I had with the use of the program.
Thank you Mac! 

To Abalore, for his kindness and for resolving more than one question that arose during the process. Thank you Abalore!
