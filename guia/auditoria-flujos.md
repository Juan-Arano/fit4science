# Auditoría de flujos Fit4Science (6 marzo 2026)

## Alcance auditado

- App web/SPA: `https://fit4science-app.vercel.app/planner.html`
- Página de confirmación/reset: `https://fit4science.vercel.app`
- Código fuente auditado: `planner-app/planner.html`
- Evidencia visual usada en la guía: `guia/assets/screenshots/*`

## Metodología

1. Revisión de UI real con capturas.
2. Revisión de estructura DOM y handlers en `planner.html`.
3. Clasificación de cada flujo:
   - `Verificado`: recorrido con captura real.
   - `Parcial`: flujo detectado en interfaz/código, pero sin recorrido end-to-end completo en la auditoría.

## Resultado resumido

- Flujos solicitados: **30**
- Verificados con captura real: **13**
- Parciales (detectados en UI/código): **17**

## Capturas incluidas

- `auth-login.png`
- `auth-register.png`
- `auth-reset-request.png`
- `email-confirmed.png`
- `reset-link-status.png`
- `home-start.png`
- `home-macros.png`
- `add-food-modal.png`
- `barcode-scanner.png`
- `ai-analysis-modal.png`
- `more-options.png`

## Notas de auditoría

- El flujo de Google Login está visible en UI y detectado en código, pero no se cerró el ciclo OAuth en esta ejecución.
- Hay flujos de soporte (sugerencias/bugs/conversaciones) detectados en UI/DOM y con handlers, pendientes de validación funcional completa con backend en entorno final.
- Historial, perfiles, mediciones, categorías/horarios y sincronización se detectan como funcionalidad existente; esta guía los documenta como rutas disponibles y recomienda completar captura adicional en siguiente iteración.
