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
3. Abre `index.html` con Live Preview.
## Decisiones que tomé
 
- En la tabla de agenda decidí agregarle `border` para que se organizara mejor y por estética.
- Muchas veces elegí la lista desordenada porque me parece más agradable a la vista.
- En ponentes elegí agregar `width="140"` y `height="140"` para que las imágenes se vieran mejor y más organizadas.
### Qué observé al enviar el formulario
 
La barra de direcciones de `gracias.html` muestra algo así:
 
```
gracias.html?nombre=Samuel+P%C3%A9rez&correo=samuel%40correo.com&celular=3001234567&ciudad=medellin&momento=empezando&temas=datos-sql&temas=python&taller_bot=si&talla=M&comentarios=
```
 
**¿Qué aparece después del `?`?**
Los datos que llené en el formulario, uno tras otro, con la forma `name=valor` y separados por `&`. Por eso cada campo necesita su `name`: sin él, el dato no se envía. Los checkboxes marcados se repiten (`temas=datos-sql&temas=python`).
 
**¿Cómo se ven los espacios, las tildes y la arroba?**
El navegador los codifica para que la URL sea válida:
 
- El espacio se vuelve `+`.
- La `é` se vuelve `%C3%A9`.
- La `@` se vuelve `%40`.
**¿Qué pasa con los campos que no llené?**
 
- Los campos de texto vacíos sí aparecen, pero sin valor (por ejemplo `comentarios=`).
- Los checkboxes sin marcar y los radios sin elegir no aparecen en la URL.
**¿Por qué un formulario con contraseñas nunca debería usar `method="get"`?**
Porque con `get` los datos viajan visibles en la URL. Así quedan en el historial del navegador y en los registros del servidor, y los puede ver cualquiera que mire la pantalla o reciba el enlace. Con `post` los datos van en el cuerpo de la petición y no se ven en la URL. Para contraseñas se usa `post` y además HTTPS.
 
## Lo que aprendí
 
- Aprendí a implementar mapas.
- Aprendí a implementar formularios y a enviarlos a otra página.
- Aprendí a manejar mejor la sintaxis y el orden del código.
## Hecho por
 
Samuel Andrés Patiño Pérez · [GitHub](https://github.com/samthekiller17)
 
## Captura de pantalla de resultados del Lighthouse
 
<img width="1916" height="993" alt="Resultados de Lighthouse" src="https://github.com/user-attachments/assets/cb63e5c6-dc61-4ce0-9c7b-a3e83d3bc787" />