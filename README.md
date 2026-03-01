# Portfolio Dashboard

Dashboard interactivo para analizar carteras de inversión de GVC Gaesco / Fidelity / Pictet.

## 🚀 Deploy en Vercel

1. Sube este repositorio a GitHub
2. Ve a [vercel.com](https://vercel.com) → **New Project**
3. Importa el repositorio
4. Vercel detecta automáticamente que es un sitio estático — haz clic en **Deploy**
5. ¡Listo! Tu dashboard estará en `https://tu-proyecto.vercel.app`

## 📊 Cómo usar

1. Abre el dashboard en el navegador
2. Arrastra tu archivo `.zip` con los CSVs de GVC Gaesco (o haz clic para seleccionarlo)
3. El dashboard detecta automáticamente:
   - El CSV de transacciones (cualquier archivo con "transacc" u "operaci" en el nombre)
   - Los CSVs de cotizaciones históricas (archivos con "cotizac", "precio" o "hist" en el nombre)

## 📁 Formato del ZIP esperado

```
mi_cartera.zip
├── Todas_las_transacciones.csv   ← transacciones (Compra/Venta)
├── Cotizaciones_GVC_Horizonte.csv
├── Cotizaciones_GVC_Japon.csv
├── Cotizaciones_Fidelity_SP500.csv
└── ...
```

**El nombre del ZIP no importa.** Los archivos pueden estar en subcarpetas dentro del ZIP.

### Formato CSV de transacciones
```
Fecha;Tipo;Fondo;Títulos;Precio;Importe;...
2024-01-15;Compra;GVC Gaesco RF Horizonte A FI;10,5432;123,45;1298,76;...
```

### Formato CSV de cotizaciones
```
Fecha;Precio
2024-01-15;123,45
2024-01-16;124,10
```

## 🔒 Privacidad

**Todos los datos se procesan en tu navegador.** Ningún dato sale de tu dispositivo.

## 🛠️ Tecnologías

- HTML/CSS/JavaScript puro (sin frameworks)
- [Chart.js](https://chartjs.org) — gráficas
- [JSZip](https://stuk.github.io/jszip/) — lectura del ZIP en el navegador
- Google Fonts (Syne, DM Mono, Bebas Neue)
