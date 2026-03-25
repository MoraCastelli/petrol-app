# petrol-app
Sistema de Monitoreo Operativo y Priorización de Intervención.

Aplicación web para operación de pozos que permite:
- Cargar parte diario desde formulario.
- Importar/normalizar datos desde Excel.
- Mostrar mapa de pozos con estado operativo/stop.
- Mostrar listado priorizado por criticidad.
- Ver ficha de cada pozo con:
  - datos técnicos
  - producción
  - horas operativas
  - observaciones
  - últimos registros
  - gráficos
- Generar dashboard técnico semanal y mensual.
- Emitir alertas automáticas por:
  - caída de producción
  - stop
  - muchas horas no operativas
  - desvíos vs promedio histórico
- Mandar avisos por WhatsApp y mail.
- Permitir predicción básica de comportamiento esperado.


La arquitectura para este proyecto es:
- Next.js: interfaz
- FastAPI: reglas de negocio, validación, cálculo, predicción
- MySQL: sistema de registro oficial
- Elasticsearch: búsqueda veloz y filtros
- n8n: automatizaciones y notificaciones
- Mapbox: visualización espacial
- Docker: local/dev y, si querés, algunos servicios auxiliares en server
- Linux server: despliegue principal de la app
  
