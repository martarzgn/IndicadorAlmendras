# Milestones

## Milestone 0: análisis del problema de la HU001

Es un milestone interno y corresponde al objetivo 2 de la asignatura. Trabaja con el
problema de la [HU001](historias_de_usuario.md#hu001-no-sé-si-el-precio-de-la-almendra-de-esta-semana-está-alto-de-verdad)
y para analizarlo se sigue diseño dirigido por el dominio (Domain Driven Design).

Al acabar este milestone, en el repositorio estará representado en código lo que aparece
en la HU001: el precio de cada semana de la Lonja de Albacete y los datos que tiene
(qué variedad es, la fecha, la unidad, que es €/kg de pepita, y a qué campaña pertenece).
No se podrá guardar un precio negativo. 
Cuando la Lonja pone "-" para una variedad en una semana, el código guardará esa 
semana sin precio para esa variedad, en vez de rechazarla como un precio incorrecto.
Lo que todavía no podrá decir es si el precio de esta semana está alto de verdad.

Es válido si se ha seguido la metodología. Lo compruebo viendo que:
- los issues salen de la HU001 y de lo que enlaza (los journeys y lo que se entiende por
  precio alto de verdad) y plantean problemas, no tareas;
- en los issues se usa el mismo vocabulario que usan mis padres, mi tío y la cooperativa;
- cada parte del código responde a uno de esos issues, donde se justifica por qué es lo
  que es;
- se han tenido en cuenta los errores que pueden darse al crear cada parte.

## Milestone 1: lógica del problema de la HU001 comprobada con tests

Es un milestone interno y corresponde al objetivo 4. Parte de lo que se entrega en el
milestone 0 y sigue con el mismo problema y la misma metodología, dividiéndolo en
problemas más pequeños que se puedan comprobar con un test.

Al terminar este milestone, en el repositorio se podrá saber si el precio de esta semana
está alto de verdad, comprobado con tests.

Es válido si todos los tests pasan con una sola orden y comprueban que se resuelve el
problema de la HU001 tal como está descrito. Además lo compruebo viendo que:
- cada test responde a un issue, y cada issue a la HU001;
- los tests siguen los principios F.I.R.S.T.
