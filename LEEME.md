# Pace Lab Crew — maqueta del sitio

Sitio de ejemplo (navegable, sin backend) para **Pace Lab Crew**, club de running.
Muestra las tres etapas que imagina el club: (1) sitio con noticias, fotos y videos,
(2) gestión de socios y cuotas con pago en línea, (3) tienda de merchandising.

## Cómo abrirlo

Haz doble clic en **`index.html`** (tema oscuro). Para ver la versión clara abre
**`claro.html`**. No necesita servidor ni instalación.

```
index.html      → versión principal, fondo negro (trae botón Claro/Oscuro)
claro.html      → la misma página con el tema claro activado por defecto
fotos/          → las fotos de ejemplo (ver fotos/CREDITOS.md)
```

Único recurso externo: las tipografías de Google Fonts (Anton y Plus Jakarta Sans).
Todo lo demás (HTML, CSS, JavaScript, fotos) está en esta carpeta.

## Cómo personalizarlo

| Qué quiero cambiar | Dónde |
|---|---|
| Colores de marca | `index.html`, bloque `:root` al inicio del `<style>`: `--negro`, `--lima`, `--violeta` |
| Tema claro | Bloque `html.tema-claro` (más abajo en el mismo `<style>`) |
| Logo | Función `selloPLC()` en el `<script>`; arriba está el comentario `>>> REEMPLAZAR POR EL LOGO OFICIAL <<<` |
| Fotos | Reemplaza los archivos de `fotos/` manteniendo el mismo nombre |
| Productos y precios | Arreglo `productos` en el `<script>` |
| Noticias | Arreglo `noticias` en el `<script>` |
| Horarios | Sección `#entrenamientos` en el HTML |

Si cambias `index.html`, puedes regenerar la versión clara copiando el archivo y
cambiando `class="tema-oscuro"` por `class="tema-claro"` en la etiqueta `<html>`.

## Qué es de ejemplo (y qué no)

Todo lo que aparece es **de muestra**: nombres, fotos, fechas, horarios, precios,
stock, montos y estados de pago. El sitio no envía datos a ningún servidor ni cobra
nada; los formularios, el pago de cuotas, el carrito y el portal del socio son
demostraciones visuales.

Lo que sí funciona de verdad en la maqueta: el menú, el buscador del panel de
administración, el carrito (agregar, quitar, total), la descarga del CSV de socios
y la validación del formulario de contacto.

---

Sitio de ejemplo desarrollado por **Bobba System**.
