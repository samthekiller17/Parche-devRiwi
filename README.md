# Parche Dev 2026

Sitio oficial del encuentro Parche Dev 2026, construido solo con HTML semántico.
Reto individual del Módulo 1 · HTML y CSS, RIWI.

Sitio publicado: https://samthekiller17.github.io/Parche-devRiwi/

## Páginas

- Inicio
- Agenda
- Ponentes
- Inscripción y confirmación
- Código de conducta

## Cómo verlo en tu computador

1. Clona el repositorio.
2. Ábrelo en VS Code.
3. Abre index.html con Live Preview.

## Decisiones que tomé

- (Explica al menos tres decisiones: por qué elegiste una etiqueta y no otra.)
- En la tabla de agenda decidi agregarle "border" para que se organizara mejor y para estetica
- Muchas veces elegi la lista desordenada porque me parece mas agradable a la vista la verdad
- En ponentes elegi agregar width="140" height="140" para que vieran mejor y organizadas las imagenes

- La barra de direcciones muestra algo asi: gracias.html?nombre=Samuel+P%C3%A9rez&correo=samuel%40correo.com&celular=3001234567&ciudad=medellin&momento=empezando&temas=datos-sql&temas=python&taller_bot=si&talla=M&comentarios=
  
- Que aparece despues del ?: Todos los datos del formulario como pares name=valor, separados por &. Por eso es tan importante que cada campo tenga name: sin él, el dato no se envía. Los pares siguen el orden del formulario. Los checkboxes con el mismo name se repiten (temas=datos-sql&temas=python).
  
- Cómo se ven los espacios, las tildes y la arroba: 
Se codifican para que la URL sea válida:

El espacio se vuelve + (a veces %20).
La tilde de «é» pasa a %C3%A9, que es su código en UTF-8. Cada letra con tilde o la «ñ» se convierte en una secuencia así.
La arroba @ se convierte en %40.

- Qué pasa con los campos que no llenaste:
Depende del tipo de campo:

Los campos de texto o los <select> vacíos sí aparecen, pero sin valor: comentarios=.
Los checkboxes sin marcar y los radios sin elegir no aparecen, como si no existieran. Si no marcas el taller, taller_bot no está en la URL.

- Por qué un formulario con contraseñas nunca debería usar method="get": 
Porque los datos viajan dentro de la URL, y las URLs no son privadas:

Quedan en el historial del navegador y en los marcadores.
Quedan en los registros (logs) del servidor y de cualquier proxy intermedio.
Cualquiera que mire la pantalla las ve.
Pueden filtrarse a otros sitios por el encabezado Referer si el usuario hace clic en un enlace externo.
Se pueden compartir sin querer al copiar y pegar el enlace.

Con method="post", los datos van en el cuerpo de la petición y no en la URL. Aun así, para contraseñas hace falta HTTPS. GET se reserva para consultas que no cambian nada, como búsquedas y filtros.

## Lo que aprendí

- Aprendi a implementar mapas
- Aprendi a implementar formularios y que lo envie a una pagina
- Aprendi a manejar mejor la sintaxis y el orden del codigo

## Hecho por

Samuel Andres Patiño Perez · [GitHub](https://github.com/samthekiller17)

## Captura de pantalla de resultados del Lighthouse

<img width="1916" height="993" alt="image" src="https://github.com/user-attachments/assets/cb63e5c6-dc61-4ce0-9c7b-a3e83d3bc787" />


