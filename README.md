# CANTO — Mobiliario contract

Landing B2B de mobiliario comercial (sillas, mesas, bancos de barra, lounge) importado directo de fábrica en China, para restaurantes, cafeterías, bares y oficinas en México.

- **Vivo:** https://studioamr.github.io/canto
- **Local:** puerto 4346 (`python3 -m http.server 4346 -d canto` desde ~/claude)
- **Referencia de concepto:** mobiliarioenmexico.com.mx (contract B2B, precios visibles, cierre por WhatsApp)

## Modelo
Curación en fábrica (Foshan/Guangzhou) → contenedor propio con inspección → entrega directa en el local del cliente. Sin showroom ni distribuidores.

## CONFIG (vacío a propósito)
En `index.html`, objeto `CONFIG`: `whatsapp` (formato 521...), `email`. Mientras estén vacíos, la página muestra "Canales en apertura". Llenar cuando existan los canales reales.

## Investigación
Ver carpeta `investigacion/`:
- `mercado-mexico.md` — competidores, precios y huecos del mercado contract en México
- `sourcing-china.md` — playbook del viaje: Foshan, ferias, MOQ, logística y aranceles

## Pendientes
- Validar nombre **CANTO** en IMPI (como siempre)
- Fechas exactas de Canton Fair / CIFF según investigación
- Precios objetivo por colección cuando haya números FOB reales
- Fotos reales de fábrica y muestras después del viaje (regla: la página crece con hechos, no promesas)
