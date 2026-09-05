# AbogAI Chile

Orientador jurídico chileno para comprender una situación, identificar el área jurídica y preparar una consulta informada con un abogado.

## Principios
- No sustituye asesoría jurídica profesional.
- No inventa artículos, plazos ni jurisprudencia.
- Las conclusiones jurídicas futuras deben respaldarse con recuperación desde fuentes oficiales vigentes.
- Corpus versionado por norma, artículo/inciso y período de vigencia.
- No genera automáticamente demandas, querellas ni escritos para presentar en juicio.

## Arquitectura Idea
Proyecto independiente. No usa Forestín Forge.

- Frontend: React + Vite, GitHub Pages.
- `knowledge/catalog.json`: catálogo y esquema del corpus.
- Próxima capa: ingesta/versionado BCN LeyChile + índice de recuperación + API de orientación.

## Estado v0.1
Interfaz y catálogo implementados. Código Civil, Penal, Comercio y Trabajo tienen fuente oficial enlazada. Los demás módulos están declarados como pendientes de ingesta; la UI no simula que el corpus completo ya fue descargado.

## Seguridad jurídica
La versión estática clasifica y organiza consultas, pero deliberadamente no entrega citas legales específicas sin una capa de recuperación/verificación. Esa capa es el siguiente hito.
