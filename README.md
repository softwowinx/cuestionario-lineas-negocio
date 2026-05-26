# Cuestionario · Líneas de negocio wowinX

Cuestionario interactivo de una sola página para mapear cómo trabajamos por dentro
nuestras tres líneas de negocio: **Inversión**, **Patrocinios** y **Desarrollos a medida**.

Lo rellena una persona (Iker). Las respuestas se guardan automáticamente en el
navegador (`localStorage`) y pueden exportarse como texto plano desde "Ver resumen → Copiar todo".

## Características
- Un único `index.html`, vanilla HTML/CSS/JS. Sin dependencias salvo Google Fonts.
- Navegación libre entre líneas, progreso guardado, indicador de líneas completadas.
- Tipos de pregunta: opción única, opción múltiple y ordenar.
- Cada pregunta admite un texto libre opcional ("Matizar / añadir").

## Editar las preguntas
Todas las preguntas viven en el array `LINEAS` dentro del `<script>` de `index.html`.
Cada pregunta es `{ id, tipo: 'unica' | 'multiple' | 'orden', texto, opciones: [...] }`.

## Logo
La cabecera carga `wowinx_logo.jpeg` (fondo negro, isotipo blanco). Si el archivo no
está presente, se muestra automáticamente el texto "wowinX" como respaldo.

## Ver en local
```bash
python3 -m http.server 8000
# abrir http://localhost:8000
```
