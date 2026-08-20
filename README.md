# EQUIPA — Equipamiento de desarrollos (antes CANTO)

Landing B2B de mobiliario comercial (sillas, mesas, bancos de barra, lounge) importado directo de fábrica en China, para restaurantes, cafeterías, bares y oficinas en México.

- **Vivo:** https://studioamr.github.io/equipa
- **Local:** puerto 4346 (`python3 -m http.server 4346 -d equipa` desde ~/claude)
- **Referencia de concepto:** mobiliarioenmexico.com.mx (contract B2B, precios visibles, cierre por WhatsApp)

## Estructura
- `index.html` — **catálogo tipo tienda** (espejo de mobiliarioenmexico.com.mx): topbar WhatsApp, header con menú, banner amarillo, slider, carruseles por categoría con badges "Ahorra %", modal de producto, carrito de cotización (localStorage) que se envía por WhatsApp, búsqueda, newsletter (guarda correos en localStorage `canto-news`).
- `concepto.html` — la landing editorial de marca (v1).
- 21 productos en el array `P` de index.html; precios = preventa, calibrados con la investigación de mercado (debajo del rango medio de competidores). Fotos de producto en `img/p/` (Pexels/Unsplash, licencia comercial libre) — sustituir por fotos reales de fábrica tras el viaje.

## Modelo
Curación en fábrica (Foshan/Guangzhou) → contenedor propio con inspección → entrega directa en el local del cliente. Sin showroom ni distribuidores.

## CONFIG (vacío a propósito)
En `index.html`, objeto `CONFIG`: `whatsapp` (formato 521...), `email`. Mientras estén vacíos, los botones de WhatsApp explican que los canales abren con el Catálogo 01 (el carrito no se pierde). Llenar cuando existan los canales reales.

## Kit de ventas (`ventas/`)
- `EQUIPA-KIT-DESARROLLADORES.pdf` — 6 páginas A4 para mandar a constructoras/desarrolladores (portada, modelo, 4 paquetes tipo con precio, catálogo resumen, proceso en 5 pasos, contraportada con QR). Se regenera desde `kit.html` con Chrome headless (`--print-to-pdf`).
- `mensajes.md` — guiones de prospección: WhatsApp (desarrollador, restaurantero, despacho), email formal, seguimiento, pitch de 30 s y manejo de objeciones.

## Investigación
Ver carpeta `investigacion/`:
- `mercado-mexico.md` — competidores, precios y huecos del mercado contract en México
- `sourcing-china.md` — playbook del viaje: Foshan, ferias, MOQ, logística y aranceles

## Pendientes
- Validar nombre **EQUIPA** en IMPI — clases 20 y 35, búsqueda fonética en Marcanet
- Fechas exactas de Canton Fair / CIFF según investigación
- Precios objetivo por colección cuando haya números FOB reales
- Fotos reales de fábrica y muestras después del viaje (regla: la página crece con hechos, no promesas)
