🚀 Gestión de Leads y Segmentación Automática

Descripción:
Este flujo de trabajo en n8n automatiza la recepción de leads desde formularios web, realiza una limpieza profunda de datos mediante JavaScript
y segmenta a los interesados según criterios geográficos y de contacto para optimizar la respuesta comercial.

Características Principales:
Normalización de Datos: Utiliza un Code Node para estandarizar nombres y países (ej. convierte "argentina" en "ARGENTINA"), eliminando fallos en la lógica por errores de tipeo.

Segmentación Inteligente: Aplica un filtro doble (País + Validación de Email) para asegurar que el equipo de ventas solo reciba prospectos calificados.

Prevención de Duplicados: Implementa una lógica de Append or Update para mantener una base de datos limpia y sin registros repetidos.

Omnicanalidad: Registra a todos los ingresantes en un "Registro Maestro" y notifica por Gmail a los perfiles aprobados de forma simultánea.

Nodos Utilizados:
Google Sheets Trigger: Captura en tiempo real cada nueva respuesta del formulario.

Set Node (Datos limpios): Filtra el ruido y mapea solo los campos esenciales (Nombre, Email, Pais).

Code Node (Normalización): Script en JavaScript para la transformación y estandarización de strings.

If Node: Cerebro lógico para la división de ramas (Aprobados vs. No aptos).

Gmail Node: Envío de alerta profesional personalizada con los datos del lead.

Google Sheets Node (Registro): Gestión de base de datos para leads descartados y registro maestro.

Desarrollado para Itera Digital Hub
