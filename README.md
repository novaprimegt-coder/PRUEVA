# Restaurante El Sol del Pueblo — V1.11.2

Sitio web de demostración para Restaurante El Sol del Pueblo, Chiantla, Huehuetenango.

## Archivos publicados

- `index.html`: página principal (conservada sin cambios), con información del restaurante, fotografías, carrusel de «El lugar y los sabores», fondo animado y consulta de reservaciones.
- `carta.html`: carta digital independiente V1.11.2, con cinco categorías: Desayunos, Almuerzos, Cenas, Postres y Bebidas.

## Actualización V1.11.2

- Presentación de platillos mediante galería curva inspirada en `CircularGallery`: renderizado WebGL2 y alternativa visual para navegadores incompatibles.
- Desplazamiento táctil, ratón, controles y navegación por teclado.
- Se conserva el acceso «Volver a la página», dirigido a `index.html#menu`.
- Se mantienen los 20 registros de categoría-producto de la versión anterior y las consultas por WhatsApp.
- No existe botón «Toda la carta». No se añadieron nombres, precios ni fotografías de platillos sin confirmar.
- La galería utiliza portadas tipográficas para evitar asociar fotografías no verificadas con productos.

Ambos HTML son autocontenidos respecto a sus estilos y scripts propios; las tipografías web pueden requerir conexión a Internet.

**Aviso:** Los productos, precios, disponibilidad de cenas y reservas deben confirmarse con el restaurante. Las restricciones de copia y zoom no garantizan impedir capturas o descarga de recursos.

**Repositorio:** `novaprimegt-coder/PRUEVA` · **Rama:** `main`.

## Corrección V1.11.2
- Se mantiene exclusivamente el selector de las cinco categorías, sin el botón «Toda la carta».
- El botón «Volver al sitio» y el logotipo regresan a la portada principal sin el ancla `#menu`.
- En caso de que el navegador conserve la versión anterior, abrir `carta.html?v=1.11.1` para solicitar una copia actualizada.

## Corrección de origen V1.11.2
- Causa identificada: el `index.html` anterior contenía un script de demostración que generaba una carta antigua mediante `Blob` y reemplazaba sus enlaces. Ese script se retiró.
- Los tres accesos desde la portada ahora abren `carta-v112.html`, una ruta nueva sin la caché de la carta anterior.
- `carta.html` también está corregida, sin el botón «Toda la carta», conservando las cinco categorías.
- «Volver al sitio» y el logotipo regresan a `https://novaprimegt-coder.github.io/PRUEVA/index.html?v=1.11.2`, evitando las rutas `blob:` y los anclajes antiguos.
- Sin cambios en productos, diseño de la carta ni animaciones existentes.
