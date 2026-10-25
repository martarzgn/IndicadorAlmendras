# Milestones

## Milestone 0: análisis del problema de la HU001

Es un milestone interno y corresponde al objetivo 2 de la asignatura. Trabaja con el
problema de la [HU001](historias_de_usuario.md#hu001-no-sé-si-el-precio-de-la-almendra-de-esta-semana-está-alto-de-verdad)
y para analizarlo se sigue diseño dirigido por el dominio (Domain Driven Design).

El código, todavía sin lógica, en el que cada parte sale de un issue en el que se ha
aplicado esa metodología a la HU001.

Es válido si se ha seguido la metodología. Lo compruebo viendo que:
- los issues salen de la HU001 y de lo que enlaza (los journeys y lo que se entiende por
  precio alto de verdad) y plantean problemas, no tareas;
- en los issues se usa el mismo vocabulario que usan mis padres, mi tío y la cooperativa;
- cada parte del código responde a uno de esos issues, donde se justifica por qué es lo
  que es;
- se han tenido en cuenta los errores que pueden darse al crear cada parte;
- cada commit cierra o referencia un issue.

## Milestone 1: lógica del problema de la HU001 comprobada con tests

Es un milestone interno y corresponde al objetivo 4. Parte de lo que se entrega en el
milestone 0 y sigue con el mismo problema y la misma metodología, dividiéndolo en
problemas más pequeños que se puedan comprobar con un test.

El código del milestone 0 con la lógica que resuelve el problema de la HU001 y los tests
que la comprueban, incluidos los de los errores, que se ejecutan con una sola orden.

Es válido si todos los tests pasan con una sola orden y comprueban que se resuelve el
problema de la HU001 tal como está descrito. Además lo compruebo viendo que:
- cada test responde a un issue, y cada issue a la HU001;
- los tests siguen los principios F.I.R.S.T.;
- cada commit cierra o referencia un issue.
