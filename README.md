# n8n-automatizacion

Ecosistema de Automatizacion IA Autonomo para Negocios. Entrega Final, Coderhouse, IA Automation.

Autor: Alan Gutierrez

## Que hace el flujo

Un lead nuevo se carga en una base de Notion (Leads). n8n lo detecta, lo clasifica como VIP o No VIP con un modelo de IA (OpenRouter, GPT-4o-mini), y si es VIP pide aprobacion humana por Slack (Human in the loop) antes de enviarle un email de contacto por Gmail. Todo el ciclo de vida del lead queda registrado en la propia base de Notion mediante la columna Estado.

## Enlaces

Base de datos de Leads en Notion, vista publica de solo lectura: https://powerful-clematis-555.notion.site/Ecosistema-Final-Clasificaci-n-de-Leads-VIP-3e751928d6018087b671cd08168cb8c9

Repositorio de este proyecto: https://github.com/alanlucianogutierrez/n8n-automatizacion

## Contenido de la carpeta entrega-final

workflow.json: export del flujo de n8n, sanitizado, sin credenciales.

architecture_diagram.png: diagrama de arquitectura del sistema.

01_arquitectura.pdf: Entregable 1, mapa de arquitectura del sistema.

02_estructuras_datos.pdf: Entregable 2, esquema de la base de Notion y JSON de cada integracion (trigger, IA, Slack, Gmail).

03_optimizacion_costos.pdf: Entregable 3, matriz comparativa de modelos de IA y justificacion de costos.

04_seguridad_resiliencia.pdf: Entregable 4, minimizacion de datos, manejo de errores y puntos de control humano.

## Stack

Notion (base de datos y trigger), n8n (orquestacion), OpenRouter con GPT-4o-mini (clasificacion IA), Slack (aprobacion humana), Gmail (contacto al lead).
