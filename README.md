# TagDrive

## Problema a tratar

Las plataformas de almacenamiento en nube que puedes encontrar se basan en una clásica estructura jerárquica, similar a la mayoría de sistemas de archivos. Esta estructura jerárquica presenta varios problemas:
- Con archivos que pueden caer dentro de dos categorías o posibles clasificaciones, por ejemplo unos apuntes de una asignatura que estás cursando en dos años diferentes;
- A la hora de recordar dónde está cada archivo, por ejemplo si tienes todos los resguardos de pagos en un sitio y las cosas de la universidad en otro, puede que no recuerdes dónde habías guardado el resguardo de matrícula;
- Y creándose duplicados, por ejemplo si tienes una carpeta que comprimir para entregar y tienes que reutilizar documentación de una entrega anterior, la duplicarías para ello.

Personalmente, he vivido esto tanto en la universidad, con asignaturas que he llegado a cursar en diferentes años y teniendo que saltar de año en año navegando carpetas para encontrar los apuntes que buscaba, o presidiendo una asociación en la que la documentación para presentar en convocatorias tenía que duplicarse y buscarse entre múltiples carpetas para cada convocatoria.

## Lógica de negocio requerida

En adición a las operaciones CRUD de subida, descarga y eliminación de archivos y edición de etiquetas, la implementación requerirá lógica para:
- La realización de búsquedas con sentencias lógicas complejas, incluyendo variables dinámicas como la fecha y hora en el momento de la búsqueda.
- Analizar los archivos subidos calculando su hash e impedir la creación de archivos duplicados, realizando las fusiones de etiquetas pertinentes.
- Diferenciar entre nombres duplicados y archivos duplicados, gestionando adecuadamente la subida de nombres duplicados sin perder archivos.

![Fotografía de la tarjeta de rol](tarjeta.jpg)

## Configuración

En el siguiente archivo se puede encontrar la configuración de Git y GitHub para realizar la subida de los archivos: [docs/configuracion.md](docs/configuracion.md).
