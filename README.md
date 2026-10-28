# IndicadorAlmendras

Marta Ruiz González

## El problema

Mis padres tienen una plantación de almendros de la variedad Lauranne. Es nueva,
llevan dos campañas cogiendo almendra. Toda la cosecha la venden de una vez, en
cáscara, a una cooperativa, que les paga según el rendimiento en pepita y el precio
de la almendra Comuna en la Lonja de Albacete (la Lonja de Albacete no cotiza la
Lauranne, así que la cooperativa la paga como Comuna).

El día de vender lo eligen ellos, y la almendra se puede guardar sin coste, así que
pueden esperar si quieren. El problema es que no saben si les conviene vender ya o
esperar unas semanas. Ahora venden "cuando el precio está alto", pero eso lo saben
sobre todo por lo que se comenta entre vecinos y otros agricultores del pueblo. No
tienen ninguna forma de saber si esperar les va a dar más dinero o menos.

Ya les ha pasado vender y que poco después el precio subiera sobre un 7 %.
Como venden la cosecha de golpe, ese porcentaje se pierde sobre todo lo del año.
Además, la cosecha cambia mucho de un año a otro: el año pasado cogieron unos
1000 kg y este año 500 kg por la helada, así que cuando hay poca almendra cada
céntimo por kilo pesa.

Lo que necesitan es que, cada semana de la campaña, alguien les diga si es mejor
vender esa semana o esperar, y cuánto dinero se juegan con su cosecha en un caso
y en otro.


## A quién le pasa

- Mis padres, que son con quien he hablado y de donde sale la idea.
- En mi familia todos tienen almendros, y les influye.
- En general pequeños agricultores de almendra que venden a una cooperativa,
    deciden ellos el día y se guían por lo que se comenta en el pueblo.


## Datos

- **Precios de la Lonja de Albacete**: uso esta lonja y no otra porque es la que
    usa la cooperativa para pagar a mis padres. Da igual lo que cotice la almendra
    en otras lonjas, lo que cobran depende de la Comuna de Albacete.
    El histórico está en
    [Synergynuts - Lonja de Albacete](https://synergynuts.upct.es/precio-almendra/lonja-albacete/),
    desde el 17/06/2021 (en aquel entonces estaba a 2,95 €/kg) hasta ahora, o sea,
    unas cinco campañas. No hay dato todas las semanas: sale más o menos uno cada
    una o dos semanas, y en verano hay huecos de uno a tres meses sin precio (por
    ejemplo, de finales de mayo a finales de agosto de 2025). Como la Lauranne se
    coge en agosto-septiembre y lo que importa son las semanas después de la cosecha,
    esos huecos afectan poco, pero hay que tenerlos en cuenta.
    Los datos están en una tabla HTML en una sola página. Para sacarlos voy a leer
    el HTML con mi propio código y quedarme con las columnas Fecha y Comuna.

- **Ventas de mis padres**: las liquidaciones que les da la cooperativa cuando
    venden. De la campaña pasada hay 2 papeles, en foto (la cosecha de este año
    todavía no la han vendido). De cada uno saco la fecha de la venta, los kilos en
    cáscara, el rendimiento en pepita y el precio pagado (€/kg).
    Son pocas ventas porque la plantación es nueva, pero sirven para comprobar que,
    con el precio de la Comuna de esa semana y el rendimiento, me sale lo que les
    pagaron de verdad, y para saber cuánto habrían cobrado vendiendo otra semana.
    Hay algunas cosas a tener en cuenta al sacar los datos:
    - No hay precio todas las semanas: en agosto, por ejemplo, se salta semanas, porque no se suele recoger la almendra en esas fechas.
    - Algunas semanas una variedad no tiene precio y sale un guion (–).
    - Las fechas no siempre vienen igual: unas veces `6/8/2026` y otras `1/07/2021`, con el cero delante del mes.
    - Los decimales van con punto, no con coma.




## Por qué en la nube

Los precios de la lonja salen cada semana, así que hay que ir recogiéndolos de forma
continua. Y quien lo tiene que consultar son mis padres, desde el móvil y en el
momento en que están pensando si vender.


## Lógica de negocio

No basta con guardar y mostrar precios. Con el histórico hay que:

- Decidir, para una semana concreta de la campaña, si conviene vender o esperar,
    a partir de cómo se ha movido el precio en las mismas semanas de campañas
    anteriores y de cómo viene en las últimas semanas.
- Pasarlo a euros con los kilos y el rendimiento de mis padres, porque lo que les
    importa es cuánto cobran, no el €/kg de la lonja.
- Comprobar que la decisión funciona de verdad con el histórico: coger cada campaña
    pasada, hacer como si estuviera en cada semana sin saber lo que pasó después,
    aplicar la decisión y ver cuánto habrían cobrado. Eso se compara con vender
    justo después de la cosecha y con lo que vendieron mis padres de verdad. Si no
    saca más dinero, no sirve.


## Referencias

Hay webs que publican precios de almendra de varias lonjas, como
[Synergynuts](https://synergynuts.upct.es/precio-almendra/). Dan el precio de cada
semana, pero no te dicen si te conviene vender ya o esperar, ni cuánto te juegas tú
con tu cosecha, que es lo que mis padres no tienen.

## Planificación (objetivo 1)
- [Personas](docs/objetivos/objetivo-1/personas.md)
- [User Journeys](docs/objetivos/objetivo-1/user-journeys.md)
- [Historias de Usuario](docs/objetivos/objetivo-1/historias_de_usuario.md)
- [Milestones](docs/objetivos/objetivo-1/milestones.md)

## Configuración del repositorio y juego de rol

[Ver configuración y juego de rol](docs/objetivos/objetivo-0/configuracion.md)

## Licencia

Este proyecto tiene licencia [GPL-3.0](LICENSE).
