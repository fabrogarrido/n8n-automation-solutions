# n8n-automation-solutions
# 📦 Control de Inventario Automatizado

## Descripción
Este flujo de trabajo en n8n permite monitorear el stock de productos en una planilla de Google Sheets y enviar alertas automáticas por Gmail cuando el inventario baja de un umbral crítico.

## Características Principales
- **Prevención de Duplicados:** Utiliza una lógica de filtrado para no re-enviar correos de productos ya notificados.
- **Sincronización:** Actualiza el estado en la base de datos una vez realizada la acción.
- **Eficiencia:** Solo procesa ítems que cumplen las condiciones de "Bajo Stock" y "No notificado".

## Nodos Utilizados
- **Google Sheets Trigger:** Monitorea cambios cada minuto.
- **Filter Node:** Aplica lógica condicional (Stock < 10 AND Notificación != Verdadero).
- **Gmail Node:** Envía el aviso profesional al encargado.
- **Google Sheets Node (Update):** Marca el ítem como notificado.

---
*Desarrollado para Itera Digital Hub*
