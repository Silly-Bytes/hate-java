Why do I hate Java
==================


Todo es un objeto...
--------------------

... No, no lo es!



No todo es un objeto. Ha leído alguna vez código Java? Está repleto de acciones
disfrazadas como objetos: Mutator, Traverser, Factory, Maker, Creator,
Generator, Mediator, Eliminator. De forma que no se *muta*, *recorre* o *crea*
nada, en cambio se **fuerza** un **objeto** que puede hacerlo.

Ok, algunas de esas cosas pueden resultar legítimamente útiles para patrones de
diseños *bien utilizados* y obtener un buen diseño, pero la mayor parte del
tempo no lo es!

No fuerce objetos por todas partes. Las clases son buenas cuando se ajustan a la
idea y un buen lenguaje cuenta con capacidades OOP como una **característica**.

Como Steve Yegge lo planteó en su articulo: [Execution in kingdom of nouns](
http://steve-yegge.blogspot.com/2006/03/execution-in-kingdom-of-nouns.html),
los verbos no deberían ser ciudadanos de segunda.

La estupidez de Java causa [asombro y comportamientos a los que uno está forzado
a acostumbrarse.]( http://www.j-paine.org/objects/objects/objects.html)


S.O.S
-----

Ok, Se topó con un problema, *javac* lanza un error completamente incomprensible
y, por supuesto, se dirige a Google esperando obtener respuestas, y las
consigue:

- Click sobre ese botón
- Una ventana emergente aparece
- Llene aquellos campos de texto
- Marque ese check box
- Click sobre el icono amarillo
- Click "ok"
- Luego reiniciar el IDE

> Me estas jodiendo?


El desgraciado 99% de las "soluciones" que se encuentran son una secuencia de
clicks y acciones en una interfaz gráfica de usuario de un IDE, Qué ocurre si no
estoy usando ese IDE en particular? Quizás no estoy ni siquiera en una sesión
Xorg y estoy escribiendo mi código desde la comodidad de mi editor de texto
preferido en una agradable sesión de Tmux o Screen, cómo estoy supuesto a hacer
"click" aquí o allá? No tengo iconos!

Cómo es posible que un error producido por que Java no puede localizar una
librería o algo similar requiere una secuencia de acciones en una GUI usando un
mouse? Y peor aun, cómo es posible que es la UNICA solución!?

Ustedes están consientes de que el código es texto plano verdad?... VERDAD??


Usa un IDE!
-----------

James Gosling (el padre de Java) dice: [No use
Emacs](http://www.computerworld.com.au/article/207799/don_t_use_emacs_says_java_father/).

Claro, si se escribe Java y no se usa un IDE sino un buen editor de texto, uno
se somete a momentos difíciles, pero esto debido a una buena razón.

La programación en Java se torna difícil con Vim o Emacs por que Java apesta
mucho, y este síntoma habla más sobre el lenguaje que sobre los editores.

El lenguaje necesita y es *dependiente* de un enorme, sobrecargado y algunas
veces lento programa creado para usar el lenguaje. El IDE se convierte un
soporte para sostener todo aquello en lo que el lenguaje fracasa.

Así que el lenguaje que no está pensado para humanos, requiere una capa
adicional, una interfaz (el IDE) para el real uso del usuario.

Más sobre el tema en el post: [Por qué odio los
IDEs](http://silly-bytes.blogspot.com/2016/03/why-do-i-hate-ides.html)


Proyectos dependientes de un IDE
--------------------------------

Si su proyecto usa, digamos, Eclipse, la otra persona deberá usarlo también si
no quiere morir en el intento de mantenerlo en Netbeans por ejemplo. Si es
posible, pero se obtienen dolores de cabeza.

Encontró un ejemplo útil en Internet sobre algo que necesita? Genial! Roguemos
por que use exactamente el mismo IDE...

Ha intentado compilar un proyecto generado en un IDE sin el IDE? Si no se siente
extremadamente aventurero o no esta dispuesto a hacerlo sin varios horribles
hacks, entonces mejor instale ese estúpido IDE.

Proyectos dependientes de un IDE ya son lo bastante malos, pero proyectos
dependientes de una **versión** especifica de un IDE?? Si... Podría también
simplemente dispararse en la cabeza ahora.


Para qué documentación cuanto tienes un mouse?
----------------------------------------------

La documentación real es casi inexistente si el IDE tiene un botón *automagico*
de la GUI para hacerlo, así que si tiene que hacerlo, más le vale usar el IDE de
forma que pueda presionar el condenado botón!

Intentando escribir una interfaz SOAP para una aplicación JSF? No hay problema,
solo haga Click aquí y allá!. Pero si no use el IDE entonces está bastante
jodido por que documentación sobre como **escribir** la funcionalidad es
estúpida o no existe.

La documentación se vuelve opcional si el IDE tiene un botón para hacerlo.

La automatización es buena!, pero si se **tiene que** usar un IDE para
implementar un servicio web SOAP en una estúpida aplicación JSF porque no hay
otra forma en la que no se necesite atravesar un proceso traumático, entonces
usted está enterrado en mierda!

Nótese que estoy usando SOAP como ejemplo únicamente por el beneficio del
argumento, existen varios otros ejemplos, cada uno de los cuales tiene más o
menos documentación.


Conclusión
----------

- Existen muchos programadores estúpidos, y Java es una de las cosas a las que
[culpar](http://www.joelonsoftware.com/articles/ThePerilsofJavaSchools.html).

- Si no puede escribir software cómodamente sin un IDE, entonces el lenguaje es
  una porquería.

- Debido a la dependencia de Java con los IDEs como (posibilitadores de malos
  lenguajes)[https://dzone.com/articles/ide-bad-programming-language], **muchos
  de los problemas de Java no son más que la intersección con los problemas con
  los IDEs.**
