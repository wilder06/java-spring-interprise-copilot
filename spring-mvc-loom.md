# Spring MVC + Loom

## Modelo
Spring MVC mantiene el modelo Servlet imperativo. Virtual Threads permiten atender más tareas bloqueantes con menor coste de hilo, pero los recursos downstream siguen siendo limitados.

## Checklist
- Confirmar Spring Boot y soporte de la propiedad `spring.threads.virtual.enabled`.
- Medir pool JDBC, HTTP, AS400, límites de conexiones y CPU.
- Establecer timeouts y límites de concurrencia por dependencia.
- No crear pools ilimitados de conexiones.
- No asumir que toda librería bloqueante funciona correctamente sin pruebas en virtual threads.
- Comparar latencia p50/p95/p99, throughput, errores y saturación.
