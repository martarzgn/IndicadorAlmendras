
# StudyRadar UGR
# Marta Ruiz González


# ---------------------------------------------------------------------


## Descripción del problema

Los estudiantes universitarios de Granada pasamos entre 8 y 10 horas al día estudiando fuera de casa, sobre todo en periodo de examenes. 

El problema de los estudiantes no es encontrar las bibliotecas, el dilema es que salen de su piso sin saber van a encontrar una mesa útil cuando lleguen en media hora.

Esto supone un desperdicio de tiempo y desplazamientos ineficaces entre las bibliotecas de las facultades (Ciencias, ETSIIT, Derecho, Cartuja, PTS, o la Biblioteca Provincial).

La información provista de las instituciones (horarios de apertura y cierre, aforo máximo) resulta insuficiente frente a la veracidad real y dinámica el entorno. 

Con encontrar una mesa útil nos referimos a:
 1. **Ocupación fantasma ("Efecto toalla"):** Puestos bloqueados de forma intencionada por otros estudiantes con apuntes, estuches, mochilas o abrigos.

 2. **Escasez de tomas eléctricas:** La disponibilidad de enchufes funcionales por mesa es un elemento determinante a la hora de elegir biblioteca por los estudiantes, ya que estos utilizan ordenadores portátiles para su actividad académica.

3. **Nivel de ruido real:** Hay diferencias notables de ruido según la biblioteca y la franja horaria.


## Lógica del problema y necesidad de cálculo

La resolución del problema consiste en un motor de procesamiento que ejecuta las siguientes operaciones analíticas sobre los datos de observación:
* **Ponderamiento por decaimiento temporal**: Aplicar una función de pérdida de vigencia sobre cada sala según su antigüedad para que los reportes recientes predominen sobre observaciones pasadas.
* **Filtrado de anomalias y discrepancias**: Depurar y descartar reportes contradictorios y maliciosos sobre una sala en una misma ventana de observación.
* **Validación de disponibilidad real** de puestos libres útiles frente a aquellos bloqueados por ocupación fantasma.
* **Estimar la habitabilidad**: Detectar la probabilidad de encontrar tomas eléctricas libres, el nivel acústico tolerado y la disponibilidad física real.

El sistema ya poseerá datos estructurales de partida y no dependerá únicamente de la voluntad de los estudiantes.
El sistema atiende a datos bases preexistentes como el catálogo oficial de bibliotecas de la UGR, el aforo máximo histórico y la distribuicioón fija de tomas electricas.

El motor tendrá una interacción mínima, quien reporta sólo pulsará un indicador de estado puntual.

El estudiante sólo define sus restricciones y el sistema calcula la mejor opción.

El problema y las necesidades del usuario fueron definidas a partir de la dinámica de *Design Thinking* realizada para empatizar con las dificultades de acceso a los puestos de estudio:

![tarjeta de cliente](doc/img/tarjeta-cliente.jpg)
![tarjeta de desarrollador](doc/img/tarjeta-desarrollador.jpg)
![tarjeta de validación](doc/img/tarjeta-validacion.jpg)

## Configuración del entorno

Para ver los detalles de la configuración del entorno de desarrollo y del repositorio, ver [doc/configuracion.md](doc/configuracion.md)
