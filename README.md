💸 Monitor Dólar Oficial (Alerta > $1500)

Workflow automatizado en n8n para seguimiento de tipo de cambio en tiempo real.

⏱️ Trigger: El nodo Schedule Trigger inicia la ejecución cada 15 minutos.

🔗 Nodos: HTTP Request (API Dolar) → Edit Fields (Limpieza) → IF (Lógica) → Gmail (Envío).

🧠 Condicional: El nodo IF evalúa la expresión precio_venta > 1500 para definir prioridad.

🔔 Notificación: Si es True envía "ALERTA"; si es False envía "Reporte". Ambos inyectan el precio actual.

✅ Best Practices: Normalización de datos previa, cobertura total de caminos (sin cajas negras) y credenciales seguras.
