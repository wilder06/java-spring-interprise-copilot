# WebFlux / Reactor

## Principios
- El event loop debe permanecer libre de operaciones bloqueantes.
- Composición reactiva de extremo a extremo cuando las dependencias lo permitan.
- `map`: transformación síncrona. `flatMap`: composición asíncrona.
- `zip`: combinación de fuentes independientes; revisar comportamiento si una fuente completa vacía.
- `switchIfEmpty`: ausencia de emisión. `onErrorMap`: traducción de error.
- No usar `block`, `subscribe` ni `join` en el flujo de request productivo.

## Ausencia de datos
Definir explícitamente el contrato: lista vacía, 404, error de negocio u otra respuesta. No asumirlo por el tipo `Mono`/`Flux`.
