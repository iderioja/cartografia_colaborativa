### Guía para la edición colaborativa de la cartografía del Gobierno de La Rioja

Este proyecto tiene como objetivo principal crear un espacio de trabajo en el que podáis participar de forma activa en la producción geográfica de nuestro territorio.

Lo hemos bautizado como **"Cartografía Colaborativa"**, aunque esta fórmula que también se está empezando a utilizar en otros países, se conoce como "Crowd-Mapping".

Es un hecho que la sociedad en que vivimos avanza imparable hacia fórmulas cooperativas de generación de información. La cartografía no podía ser menos y por ello, las administraciones como principales proveedoras de datos geográficos, tenemos la obligación  de poner los medios necesarios para que esta participación sea posible.

Pero en esta fórmula de colaboración el elemento más importante de la ecuación eres tú, tú como gran conocedor de los pequeños detalles del territorio que pisas y habitas a diario.

Desde el Gobierno de La Rioja estamos haciendo un esfuerzo importante para poner a tu alcance distintos mecanismos de participación, éste es uno más. Así que si te gusta la información geográfica y piensas que tienes algún dato interesante que aportar a la comunidad...¡ANÍMATE!, ya no tienes excusa, **¡saca el cartógrafo que llevas dentro y colabora con nosotros!**.

#### 0 - Comenzando

Entre las múltiples plataformas de colaboración posibles para llevar a cabo este proyecto, hemos elegido una solución **Git**, ya que nos parece la más operativa desde un punto de vista técnico.

Si hasta ahora no conoces Git, ¡no te asustes!, realmente estás de suerte ya que te ofrecemos la excusa perfecta para iniciarte en este [Sistema de Control de Versiones] que, estamos seguros que antes o después te resultará personalmente muy útil en otros ámbitos.

Para poder funcionar, hemos creado un espacio de trabajo común (repositorio) y lo hemos alojado en "[GitHub]". GitHub es un servidor Git de uso público y gratuito, en el que se desarrollan de forma colaborativa muchos e importantes proyectos de software libre.

Para participar, solo necesitas tener una cuenta de usuario [GitHub], que como te puedes imaginar, es gratuita.

Si antes no has trabajado con Git... ¡NO PROBLEM!, nosotros te explicamos de forma rápida cómo hacerlo. ¡Vamos a ello!.

#### 1 - Directorios

Antes de comenzar tienes que tener en cuenta que en este esquema de colaboración existen tres directorios, dos de ellos imprescindibles y uno opcional:

- El **`REPOSITORIO PRINCIPAL`**: Es el espacio GitHub en el que se alojan los datos ya consolidados.

  En nuestro caso es un repositorio que podrás encontrar en la url: https://github.com/iderioja/cartografia_colaborativa.

  Ten en cuenta que en este repositorio NO PUEDES REALIZAR DIRECTAMENTE NINGÚN CAMBIO O MODIFICACIÓN, ya que solamente el administrador de la cuenta "iderioja" tiene permisos de escritura. Si quieres disponer de una copia de este directorio en tu propio espacio GitHub en el que SÍ TENGAS PERMISO DE ESCRITURA, es necesario ejecutar una operación que en el argot Git se denomina `fork`. Pero esto lo trataremos más adelante.

- El **`TU REPOSITORIO GITHUB`**: Es una copia inicial (clon) del Repositorio Principal que se genera en tu cuenta GitHub.

  En él podrás guardar las modificaciones que vayas realizando, bien de forma "on line" desde GitHub o si lo prefieres, en modo local.

- **`TU REPOSITORIO LOCAL`**: Este es un repositorio que puedes tener almacenado en tu propio equipo, sobre el que puedes trabajar directamente. No podía ser de otra manera ya que se trata de tu ordenador.
  
  ESTE REPOSITORIO ES OPCIONAL y solo tiene sentido en aquellos casos en que optes por instalar Git en tu máquina para trabajar de forma local.

#### 2 - Creación de una cuenta de usuario en GitHub

Dado que necesitas disponer de un repositorio propio con derechos de escritura, es imprescindible que estés registrado en [GitHub]. Si todavía no lo estás, puedes hacerlo en la página web https://github.com/


#### 3 - Hacer una copia local del repositorio principal (fork)

Para comenzar a trabajar, tal como hemos indicado anteriormente, tienes que empezar por hacerte una copia del `REPOSITORIO PRINCIPAL` en tu espacio GitHub.

Para ello debes acceder a https://github.com/ e introducir tu usuario y contraseña.

Una vez identificado, debes conectarte con la url del Repositorio Principal  https://github.com/iderioja/cartografia_colaborativa

Hecho esto, comprueba que puedes ver los contenidos del repositorio *iderioja/cartografia_colaborativa* y que en la parte superior derecha de la página se indica tu nombre de usuario.

Ahora pulsa sobre el botón `Fork` que encontrarás también en la parte superior derecha.

Finalizada la operación comprobarás que se ha creado una copia del `REPOSITORIO PRINCIPAL` en tu propio espacio de usuario, que se debería denominar "*tunombredeusuario*/cartografia_colaborativa*". Este es `TU REPOSITORIO GITHUB` en el que SÍ TIENES PERMISOS DE ESCRITURA.

#### 4 - Podemos comenzar a editar datos geográficos

Una vez duplicado el `REPOSITORIO PRINCIPAL` en tu propia cuenta GitHub, ya puedes comenzar a editar cartografía.

GitHub permite visualizar en forma de mapa los ficheros de datos geográficos de cualquier repositorio, siempre y cuando estos se encuentren almacenados en el formato **"Geojson"**.

Ahora... ¡pruébalo!. Si pulsas sobre uno de los ficheros geojson de `TU REPOSITORIO GITHUB`, comprobarás que puedes ver su contenido sobre un mapa y que el visualizador geográfico te ofrece la opción de `"Editar"`.

Esta opción te permite modificar alfanuméricamente los datos de un fichero geográfico, aunque editar así resulta extremadamente complicado y desesperante, pero... no te desanimes tan pronto, ya que desde hace muy poco tiempo GitHub nos ofrece la posibilidad de realizar una edición geográfica "on line" conectándonos a la url http://geojson.io

Desde esta página puedes conectarte a `TU REPOSITORIO GITHUB` y editar gráficamente cualquiera de tus ficheros.

Esta forma de editar datos geográficos está bastante bien ¿no?, pero si todavía quieres algo más cómodo, puedes instalar este editor como extensión en el navegador Google Chrome. Esta última opción tiene la ventaja de que es automáticamente reconocida por GitHub y en consecuencia, si abres un fichero geojson en gitHub, se muestra un botón que te ofrece la posibilidad de editarlo gráficamente con geojson.io.

Si tu intención es utilizar únicamente esta fórmula "on line" para la edición geográfica, salta directamente al punto 9 de nuestra guía donde te contamos cómo enviar tus aportaciones al `REPOSITORIO PRINCIPAL` de IDErioja.

Pero si prefieres editar los ficheros geográficos localmente en tu equipo y aprovechar así toda la potencia que te ofrece Git para llevar un control de versiones de tu propio trabajo (opción recomendada), sigue leyendo...


#### 5 - Instalación local del cliente Git

Si eres un tipo intrépido, amante del riesgo y has optado por la edición local, ¡enhorabuena!, pero antes de comenzar ten en cuenta que es imprescindible instalar en tu equipo la aplicación "Git". En http://git-scm.com/downloads puedes encontrar la última versión para tu sistema operativo.

#### 6. Hacer una copia (clon) de TU REPOSITORIO GITHUB en tu equipo local
 
Dado que has llegado hasta este punto, asumimos que has optado por la edición en modo local, así que lo primero que debes hacer para empezar a funcionar es hacer una copia de `TU REPOSITORIO GITHUB` en tu equipo local. Si recuerdas, este repositorio lo habíamos bautizado como `TU REPOSITORIO LOCAL`

Para obtener un duplicado local de `TU REPOSITORIO GITHUB`, es conveniente comenzar realizando una clonación de este repositorio. Para ello, si funcionas con Windows, tienes que abrir un entorno de ejecución de comandos. Aunque existen otras formas de hacerlo que seguramente irás descubriendo, esta por ahora es la más directa.

Te mostramos a continuación la sintaxis de los comandos para un entorno Windows:

.. Para abrir la ventana de comandos en Windows, pulsa el botón `Inicio` y selecciona `Ejecutar`. Escribe **cmd** y pulsa `Aceptar`.

En la nueva ventana, cambia si fuera necesario tu unidad de trabajo

``` 
> cd letradetuunidad:
```

Con el comando CD, te permite ubicarte hasta el nivel de directorio donde tengas previsto crear tu repositorio de trabajo.

El siguiente comando en un solo paso crea `TU REPOSITORIO LOCAL` junto con sus archivos Git de control de versiones y además clona en él `TU REPOSITORIO GITHUB`

``` 
> git clone https://github.com/tunonmbredeusuario/cartografia_colaborativa.git nombreopathdetudirectoriolocaldetrabajo
```

Comprueba que ahora existe en tu equipo local el directorio local que has especificado en el comando clone.
Dentro de dicho directorio se han copiado los ficheros geojson y, aunque posiblemente no los veas, se ha creado también un subdirectorio oculto denominado ".git". Si lo ves, ¡cuidado!, ¡no lo borres!, ya que aquí se almacena todo lo que Git necesita para gestionar el control de versiones.

Somos conscientes de que el procedimiento que hemos seguido es un tanto arcaico, pero es el más elemental para empezar. No obstante si tu curiosidad te arrastra más allá y quieres imbuirte de lleno en el universo Git, te recomendamos utilizar la aplicación visual [SmartGit] (Windows). Puedes encontrar otros muchos clientes para distintas plataformas aquí: http://git-scm.com/downloads/guis

#### 7 - Edición geográfica

En este punto, suponemos que ya dispones de una copia completa del directorio *https://github.com/iderioja/cartografia_colaborativa* en tu equipo local, así que ya puedes comenzar a editar cualquiera de los archivos que contiene o crear nuevos ficheros de datos geográficos.

Para la edición geográfica puedes usar un programa comercial o bien utilizar software libre. En este caso y puesto que el formato geográfico que utilizaremos será "Geojson", déjanos sugerirte la aplicación "Quantum GIS", conocida también como [QGIS] que te puedes descargar gratuitamente de http://www.qgis.org/

En cuanto a la edición, no olvides un detalle: ES IMPORTANTE QUE TODA LA INFORMACIÓN GEOGRÁFICA QUE PRODUZCAS LA ALMACENES EN COORDENADAS GEOGRÁFICAS LONGITUD, LATITUD EN EL SISTEMA GEOGRÁFICO DE REFERENCIA WGS84 O ETRS89. Estos sistemas tienen los códigos *EPSG:4326* y *EPSG:4258*.

#### 8. Guardar tu trabajo en GitHub

Como suponemos que a estas alturas ya tienes instalado Git en tu equipo local, puedes llevar un control de los cambios que vas realizando utilizando principalmente los comandos Git `add` y `commit`.

Si no estás muy ducho en la materia pero tienes algún conocimiento del idioma de Shakespeare, te recomendamos el libro *Git: Version Control for Everyone. Beginner's Guide* de *Ravishankar Somasundaram*. Se trata de un manual de introducción a Git muy fácil de digerir. Si tienes un estómago fuerte, no te será muy difícil encontrar platos más pesados.

El blog http://aprendegit.com/ puede ser también una fuente de información de gran ayuda.

Sigamos... una vez hayas concluido tus modificaciones en los ficheros geográficos de tu equipo local y tu Git local se haya hecho eco de ellos mediante comandos `add` y `commit`, puedes subir tu trabajo de `TU REPOSITORIO LOCAL` a `TU REPOSITORIO GITHUB`.

Te explicamos brevemente como hacerlo desde la pantalla de comandos:
```
> git status
(Este comando te informa del estado de tus ficheros en tu repositorio local)

> git add
(De esta manera marcas para seguimiento todos los ficheros que has modificado en tu repositorio. Puedes utilizar además wildcards)

> git commit -m "comentario acerca de los cambios efectuados"
(Los datos marcados para seguimiento se incorporan al control de versiones)

> git push origin master
(Este es el comando definitivo que sirve para actualizar TU REPOSITORIO GITHUB con los datos de TU REPOSITORIO LOCAL)
```

En este punto puedes comprobar que los datos que has modificado en `TU REPOSITORIO LOCAL` se encuentran actualizados en `TU REPOSITORIO GITHUB`.

Si te has decidido por el trabajo local, es imprescindible que eches un vistazo a los comandos `fetch` `merge` y `pull` que te permitirán mantener sincronizado `TU REPOSITORIO LOCAL` con los cambios que se puedan producir en `TU REPOSITORIO GITHUB`.

#### 9 - Integración de tus datos en el REPOSITORIO PRINCIPAL del proyecto

Para que el administrador *"iderioja"*,o sea nosotros, podamos integrar los datos que has editado en el `DIRECTORIO PRINCIPAL` del proyecto de cartografia colaborativa, es necesario que nos envíes una solicitud que en la jerga Git se conoce como `pull request`.

Esta operación se realiza directamente desde tu cuenta de GitHub. Detrás de este comando lo que se genera es un aviso que nos permite saber que tienes unos datos en `TU REPOSITORIO GITHUB` y que los quieres incorporar al `REPOSITORIO PRINCIPAL` IDErioja.

La incorporación la realiza el Administrador de la cuenta de "iderioja", o sea nosotros de nuevo. Para ello tendremos que hacer una serie de comprobaciones de integridad que en el caso de la información geográfica encierran cierta complejidad, pero esta pequeña dificultad es cosa nuestra.

#### 10 - Otro día más

Si dedicas un tiempo a explorar GitHub o haces una inmersión profunda en Git, comprobarás que es un universo enorme y que existen multitud de posibilidades para organizar flujos de trabajo complejos, cuyo detalle excede los objetivos de esta breve guía.

Desde estas páginas te animamos a participar en nuestro proyecto. La cartografía de La Rioja, es decir "todos", nos beneficiaremos de ello y como recompensa podrás adquirir y emplear un nuevo caudal de conocimiento. ¡El trato es justo!

No nos queremos despedir sin contarte un truco: Todos los mapas que tengas en `TU REPOSITORIO GITHUB` los puedes incrustar en tus páginas web simplemente añadiendo una sentencia con esta sintaxis:

```
<script src="https://embed.github.com/view/geojson/<username>/<repo>/<ref>/<path_to_file>"></script>
````

Puedes probar como funciona, pegando el siguiente código en un archivo de texto y guardándolo con la extensión .html 

``` html
<!DOCTYPE html>
<html>
<head>
  <meta http-equiv="content-type" content="text/html; charset=iso-8859-1" />
  <title>Municipios de La Rioja</title>
</head>
<body>
<script src="https://embed.github.com/view/geojson/iderioja/cartografia_tematica/master/municipios.geojson"></script>
</body>
</html>
````

Si tienes alguna sugerencia cuéntanosla, lo intentaremos mejorar, al fin y al cabo, este documento está pensado para ayudarte.

Muchas gracias por colaborar

El Equipo Técnico IDErioja


en revisión...


[GitHub]: https://github.com/
[Cartografía colaborativa]: https://github.com/iderioja/cartografia_colaborativa
[Git]: http://git-scm.com/
[Sistema de Control de Versiones]: http://es.wikipedia.org/wiki/Control_de_versiones
[Repositorio Principal]: https://github.com/iderioja/cartografia_colaborativa
[SmartGit]: http://www.syntevo.com/smartgithg/
[QGIS]: http://www.qgis.org/


