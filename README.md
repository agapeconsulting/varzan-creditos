# Seguimiento Analista de Créditos — Varzan Hnos. S.A.

Plataforma de seguimiento del área de Créditos. Dos páginas, ambas HTML autocontenido:

| Archivo | Qué es | URL |
|---|---|---|
| `index.html` | CRM de Seguimiento (4 pestañas) | la raíz del sitio |
| `tablero.html` | Tablero de Indicadores y Comisiones | `/tablero.html` |

Los datos **no** viven acá: viven en la planilla de Google
`Base_Operativa_Varzan`, a la que las páginas acceden mediante un Web App de
Google Apps Script. Estos archivos son solo la interfaz.

## Para actualizar una versión

1. Entrar al archivo (`index.html` o `tablero.html`).
2. Botón del lápiz (**Edit this file**) o **Upload files** para reemplazarlo.
3. **Commit changes**. GitHub Pages republica solo en uno o dos minutos.

## Versiones

- `index.html` — CRM v21: columna "Observación del Analista", recuperación de
  horas convertidas por Google Sheets, y guarda de concurrencia que impide que
  una pestaña desactualizada sobrescriba la planilla.
- `tablero.html` — Tablero v2: indicadores sobre los campos nuevos, indicador 1
  por coherencia resolución × observación, escala del indicador 3 en
  ≤6 h → 100 · ≤12 → 80 · ≤24 → 60 · ≤48 → 35.
