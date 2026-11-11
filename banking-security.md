# Seguridad para servicios bancarios

- Clasificar datos y aplicar minimización.
- No registrar DNI completo, número de cuenta, PAN, CVV, PIN, tokens ni credenciales.
- Enmascarar identificadores cuando el diagnóstico lo requiera.
- TLS y validación de certificados activos; secretos externalizados.
- Validar autorización en cada operación y evitar IDOR.
- Timeouts, límites de tamaño y concurrencia para dependencias.
- Reintentos solo para operaciones idempotentes o protegidas contra duplicidad.
- No convertir indiscriminadamente errores técnicos en respuestas 4xx ni ocultarlos como vacío.
- Revisar dependencias y configuración de despliegue.
- La plantilla no certifica cumplimiento PCI DSS, ISO 27001 ni normativa local.
