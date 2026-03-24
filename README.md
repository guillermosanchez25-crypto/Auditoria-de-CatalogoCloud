¿Cuántas líneas de código habéis ahorrado al usar grupos?
- He ahorrado entre 30 y 35 lineas de código, sobre todo donde mas lineas de codigo he ahorrado ha sido en la mision 1
¿Qué error os da VS Code si intentáis poner dos servidores con el mismo ID?
- El error que aparecerá en el panel de problemas y al pasar el ratón sobre la línea roja tendrá las siguientes características:
Violación de la restricción de identidad: VS Code te indicará que se ha producido una violación de una "identity constraint" (restricción de identidad)
.
Referencia al campo duplicado: El mensaje especificará que el valor del nodo (definido en el <xs:field> del XSD) no es único dentro del ámbito del selector
.
Identificación de la regla: Normalmente, el error mencionará el nombre específico que le asignaste a la restricción en tu esquema (por ejemplo, unicoEmail o unicoID), facilitando que sepas exactamente qué regla de negocio se está rompiendo
.
Error de validación semántica: A diferencia de los errores de "bien formado" (como una etiqueta mal cerrada), este se clasifica como un error de validación semántica, lo que significa que el analizador (parser) ha procesado la estructura pero rechaza el contenido por no ser coherente con el esquema
.
En resumen, verás un subrayado rojo y un mensaje técnico avisando que el valor ya existe en otro elemento del mismo grupo, asegurando así la integridad de tu base de datos XML
