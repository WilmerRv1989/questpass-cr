# Matriz de trazabilidad

Relación entre los requerimientos del proyecto QuestPass CR y la página donde se atiende cada uno en el primer avance.

| Código | Requerimiento | Página | Cómo se atiende |
|---|---|---|---|
| RF-01 | Navegación funcional y consistente; el nombre QuestPass CR enlaza al inicio | Todas | Menú de Bootstrap igual en las siete páginas, con la página actual marcada con `aria-current="page"` |
| RF-02 | Presentar QuestPass CR y explicar cómo reservar | index.html | Portada con enlaces a experiencias y reserva, y lista ordenada con los pasos para reservar |
| RF-03 | Mostrar las seis experiencias oficiales | experiencias.html | Una tarjeta por experiencia con código, categoría, fecha y hora, modalidad, ubicación, cupos y precio |
| RF-04 | Mostrar la información completa de QST-001 | detalle.html | Tarjeta con los datos oficiales de El Archivo 47 y ruta de navegación |
| RF-05 | Formulario de reserva con nombre, correo, teléfono, experiencia, cantidad y condiciones | reservar.html | Campos agrupados en dos `fieldset`, todos con `required` y su `label` visible |
| RF-06 | Aceptar el teléfono en formato 8888-8888 u 88888888 | reservar.html | Campo `tel` con `maxlength="9"` y `pattern="[0-9]{4}-?[0-9]{4}"`, con texto de ayuda |
| RF-07 | Permitir de 1 a 4 entradas por reserva | reservar.html | Campo `number` con `min="1"`, `max="4"` y `step="1"` |
| RF-08 | Elegir la experiencia por su código oficial | reservar.html | Lista `select` con las seis experiencias y `value` igual al código |
| RF-09 | Formulario de contacto con nombre, correo, asunto y mensaje | contacto.html | Campos con validación nativa y área de texto para el mensaje |
| RF-10 | Formulario de inicio de sesión con correo y contraseña | login.html | Campos `email` y `password` sin validar credenciales |
| RF-11 | Panel de administración con la sección Experiencias | admin.html | Tabla con las seis experiencias oficiales |
| RF-12 | Panel de administración con la sección Reservas | admin.html | Tabla vacía con el mensaje "Aún no hay reservas registradas" |
| RNF-01 | Diseño responsive para móvil y escritorio | Todas | Columnas de Bootstrap y breakpoints propios en `estilos.css` para móvil y escritorio |
| RNF-02 | Accesibilidad: un solo `h1`, labels visibles, foco visible y contraste legible | Todas | Jerarquía de encabezados, enlace para saltar al contenido y estilo de foco propio |
