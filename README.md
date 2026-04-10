# Adquisiciones 2026

Sistema web para la gestión y seguimiento del plan de adquisiciones de equipamiento médico 2026. Conecta con Google Sheets como base de datos y permite visualizar el estado de cada proceso de compra en tiempo real.

## ¿Qué hace?

- **Dashboard** con métricas generales: equipos únicos, hospitales, monto total estimado y progreso por estado
- **Vista por proyecto**: agrupa los equipos según el proyecto de adquisición y muestra montos y estados
- **Vista de equipos**: tabla completa con filtros por hospital, tipo de proyecto y estado del proceso
- Indicador de días hasta la fecha de apertura de cada licitación
- Modo oscuro automático

## Estados del proceso

| Estado | Descripción |
|--------|-------------|
| 🔘 Sin avance | Sin inicio de trámite |
| 🟣 Armado de pliego | En preparación de documentación |
| 🔵 Publicación | Licitación publicada |
| 🟡 En evaluación | Ofertas recibidas, en análisis |
| 🟢 Adjudicado | Proveedor seleccionado |
| 🔴 Fracasado | Proceso sin ofertas válidas |
| ⚪ Desierto | Sin presentaciones |
| 🔴 No se compró | Proceso cancelado |

## Tecnologías

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=flat&logo=google-sheets&logoColor=white)

## Estructura de datos (Google Sheets)

El sistema espera una hoja con las siguientes columnas:

`HOSPITAL` · `EQUIPO` · `TIPO` · `Q SOLICIT.` · `P. UNIT` · `P. TOTAL` · `NOMBRE PROYECTO` · `TIPO PROYECTO` · `AÑO ENTREGA` · `EXPEDIENTE` · `LICITACION` · `FECHA DE APERTURA` · `ESTADO` · `CHEQUEADO CON SP`

## Uso

1. Publicar el Google Sheet como API mediante Google Apps Script
2. Reemplazar `API_URL` en el `index.html` con la URL del script publicado
3. Abrir `index.html` en el navegador

---
Desarrollado por [Malena Motta](https://github.com/malenavmotta-sketch) · Buenos Aires, Argentina
