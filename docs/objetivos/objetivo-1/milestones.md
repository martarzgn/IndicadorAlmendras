# Milestones

## Milestone 0: análisis del problema de la HU001

**Historia de usuario:** 
Trabaja con el problema de la [HU001](historias_de_usuario.md#hu001-no-sé-si-el-precio-de-la-almendra-de-esta-semana-está-alto-de-verdad)

**Cómo se hace:** 
Es un milestone interno.
Se parte de la HU001 y de los journeys de mis padres y de mi tío, y de lo que ellos 
consideran un precio alto de verdad. A partir de ahí se abren issues que plantean 
los problemas que aparecen en la historia de usuario y se van solucionando con 
diseño dirigido por el dominio, usando las palabras que usan ellos y la cooperativa.

**Cómo compruebo que es válido:**
Voy revisando los issues y lo compruebo viendo que:
- los issues salen de la HU001 y de lo que enlaza, y plantean problemas, no tareas;
- en los issues se usa el mismo vocabulario que usan mis padres, mi tío y la cooperativa;
- en cada issue se razona la decisión antes de llevarla al código;
- en los issues se discute qué situaciones no pueden darse según la HU001 y cómo se rechazan.

## Milestone 1: lógica del problema de la HU001 comprobada con tests

**Historia de usuario:** 
[HU001](historias_de_usuario.md#hu001-no-sé-si-el-precio-de-la-almendra-de-esta-semana-está-alto-de-verdad),
la misma que en el milestone 0.

**Cómo se hace:**
Es un milestone interno.
Se parte del código del milestone 0 y se sigue un desarrollo guiado por tests: el 
problema de la HU001 se divide en problemas más pequeños, cada uno en un issue, y 
para cada uno primero se escribe el test que comprueba si está resuelto y después 
el código que lo resuelve.

**Cómo compruebo que es válido:**
- los tests se ejecutan automáticamente con una sola orden y pasan;
- comprueban, con semanas pasadas de la Lonja de Albacete, que se 
  sabe decir si el precio estaba alto de verdad comparado con esas 
  mismas semanas de otras campañas;
- cada test responde a un issue, y cada issue a la HU001.
