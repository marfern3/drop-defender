# Drop Defender

Demo técnica de detección de **bots de reventa** en drops de stock limitado.

Cuando una marca lanza un drop limitado con mucho hype, los bots de reventa compran antes que los compradores reales y luego revenden caro. Esta demo simula ese escenario y muestra un motor que, pedido a pedido y en tiempo real, clasifica cada compra como **persona real** o **bot**, protegiendo el stock para la comunidad.

👉 **[Ver la demo](https://marfern3.github.io/drop-defender/)**

## Qué hace

- Simula el flujo de pedidos de un drop limitado (más demanda que stock, como en la realidad).
- Clasifica cada pedido entrante en vivo: **REAL ✓** o **BOT ✕**, con el motivo.
- Muestra cuánto stock se salva para compradores reales y cuánto se bloquea a la reventa.

## Señales que evalúa el motor

| Señal | Qué detecta |
|---|---|
| **Velocidad** | Compra en milisegundos tras abrir el stock (inhumana). |
| **Repetición** | Mismo pago o misma huella de dispositivo en ráfaga. |
| **Automatización** | Navegador headless, sin interacción humana real. |
| **Reputación** | Cuentas recién creadas, IPs de centros de datos, envíos en bloque. |

## Alcance de la demo

Los pedidos son **datos simulados generados en el navegador**: nada real, ninguna web ni sistema de terceros ha sido accedido o probado. La lógica de clasificación está simplificada para la demo. Un sistema de producción se entrena con los pedidos reales de la tienda (p. ej. vía API de Shopify) y mejora con cada drop.

## Stack

HTML, CSS y JavaScript sin dependencias. Una sola página, se despliega como estático en GitHub Pages.

## Autor

**Marco Fernández** — Sistemas · Seguridad · IA
[github.com/marfern3](https://github.com/marfern3) · [linkedin.com/in/marcofer3](https://linkedin.com/in/marcofer3)
