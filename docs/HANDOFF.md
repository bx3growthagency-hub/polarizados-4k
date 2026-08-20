# HANDOFF — Polarizados 4K

**Proyecto:** Polarizados 4K (web comercial)
**Cliente:** Polarizados 4K
**Agencia:** BX3 Growth Agency
**Valor comercial:** 500.000 COP
**Estado:** Arquitectura lista — Fase 1 (desarrollo del sitio) sin empezar
**Última actualización:** 2026-08-20

---

## 1. Qué es esto

Este repo reemplaza a la carpeta `Polarizados 4k/` que vivía dentro del repo general de BX3 (`C:\Users\ASUS\BX3\BX3\`). Se separó a su propio repositorio Git independiente porque es un proyecto de software real (no un documento de agencia) y porque el repo de BX3 no debía cargar con 849MB de media sin tracking. La carpeta original sigue existiendo por ahora en `C:\Users\ASUS\BX3\BX3\Polarizados 4k\` — no se borró nada, solo se copió acá. Confirmar con Leandro si esa carpeta original se debe eliminar una vez validado que este repo tiene todo.

## 2. Completado

- Lectura completa y verificada de los dos documentos maestros de negocio.
- Inventario completo de los 28 assets exportados de Google Drive (logos, fotos, PDFs, video).
- Confirmación visual del logo real y la paleta de marca (rojo del isotipo + grafito/negro del local — ver `src/styles/tokens.css`).
- Repositorio Git propio inicializado, con estructura base de carpetas.
- Scaffold de Vite + React + TypeScript funcional (`npm run dev` / `npm run build` probados).
- Assets organizados: logos y badges de marca en `public/assets/`, 22 fotos sin curar en `public/assets/photos-raw/`, material pesado (2 PDFs + 1 video, ~309MB) en `references/` (fuera de git, ver sección 6).
- Modelo de datos inicial en `src/data/*.json` (contacto, productos, proyectos, FAQ), con cada dato marcado `confirmed_repeated`, `pending_validation` o `not_available` según los documentos maestros — **nada inventado**.
- `CLAUDE.md` con las reglas permanentes del repo.

## 3. En progreso

Nada — esta sesión fue solo de arquitectura y organización, no de construcción de páginas. El sitio real (Fase 1) todavía no tiene ni una página construida.

## 4. Siguiente tarea

Ver `tasks/fase-1.md` para la lista priorizada completa. La primera tarea concreta es: construir `Header`, `Footer` y `WhatsAppButton` (los tres se repiten en todas las páginas), y después la página `Home`.

## 5. Decisiones tomadas (y por qué)

- **Repo separado del repo de BX3**: el folder original estaba 100% sin trackear en git, sin ninguna referencia cruzada en el backlog/decision register de BX3, y con 849MB de binarios — mezclarlo con el repo de contratos/docs de la agencia no tenía sentido. Decisión confirmada con Leandro.
- **Simulador visual fuera de Fase 1**: los documentos maestros lo presentan como el diferenciador principal, pero construirlo bien (fotografía por capas, máscaras alineadas, motor de composición, recomendador) es un proyecto aparte — no cabe en el presupuesto simbólico junto con el resto del sitio. Queda documentado como Fase 2 futura, cotizable aparte. Decisión confirmada con Leandro.
- **Sin Tailwind, sin CMS, sin backend**: el sitio es mayormente contenido/marketing con CTA a WhatsApp — no hay necesidad demostrada de esa complejidad en Fase 1.
- **Multipágina en vez de landing única**: los documentos maestros piden SEO local fuerte por servicio (polarizados, PPF, etc.), lo que se sirve mejor con URLs propias por página que con una sola landing.
- **Precios no se publican en Fase 1**: las tablas de precios de los documentos tienen inconsistencias internas sin resolver (ej. 3M Ceramic IR aparece en $1.600.000 y $1.700.000 según la tabla) y los propios documentos piden no publicarlos sin aprobación final. El patrón usado es "Cotiza tu vehículo por WhatsApp".

## 6. Pendiente del cliente (Polarizados 4K) — bloquea publicación, no bloquea desarrollo

Lista completa en `docs/CONTEXTO_MAESTRO_POLARIZADOS_4K.md` sección 23 (28 ítems). Los más importantes:

1. Confirmar dirección y WhatsApp definitivos (hay dos versiones registradas — ver `src/data/contact.json`).
2. Resolver el nombre correcto: **BlackFlint** vs **Black Film**.
3. Confirmar autorización vigente de 3M y Spectra antes de usar esos logos/badges en el sitio.
4. Aprobar o corregir la lista de precios (hay inconsistencias sin resolver).
5. Confirmar garantías exactas por producto.
6. Horarios de atención, correo corporativo, redes oficiales (Facebook/TikTok) — hoy no existen en la memoria del proyecto.
7. Logo vectorial (hoy solo hay PNG en alta resolución — suficiente para web, no ideal para todo uso).
8. Seleccionar/autorizar fotos y testimonios reales para publicar.

**El material pesado sin optimizar** (catálogo PDF de 162MB, manual PDF de 74MB, video de Autofest de 74MB) vive en `references/` en este repo pero **no está en git** — son demasiado pesados para versionar. Si Hurtado necesita ese material y no tiene acceso al Google Drive original de Polarizados 4K, pedirle a Leandro que comparta la carpeta de Drive directamente (no re-subir a git).

## 7. Cómo clonar y ejecutar (Hurtado, desde Colombia)

```bash
git clone https://github.com/bx3growthagency-hub/polarizados-4k.git
cd polarizados-4k
npm install
npm run dev                        # http://localhost:5173
```

Build de producción:

```bash
npm run build      # genera dist/
npm run preview     # sirve dist/ localmente para probarlo antes de subir
```

Despliegue: pensado para exportarse estático (`dist/`) y subirse a Hostinger. No hay dominio/plan confirmado todavía — ver sección 6.

Nada de esto requiere backend, base de datos ni variables de entorno para arrancar en local. Copiar `.env.example` a `.env.local` solo cuando haya IDs reales de Analytics/Meta Pixel que agregar (todavía no existen).

## 8. Problemas conocidos / riesgos

- 22 fotos en `public/assets/photos-raw/` están sin curar: hay 3 pares duplicados exactos, ningún nombre descriptivo, y no hay pares "antes/después" identificados. Hay que revisarlas visualmente y elegir 8-15 para producción, optimizadas a WebP.
- El zip original de Drive (423MB, con estructura anidada `Polarizados 4K/Polarizados 4K/`) no se copió a este repo — solo los 28 archivos ya extraídos. Si aparece contenido nuevo en Drive más adelante, hay que repetir el proceso de extracción/curación, no asumir que este repo ya tiene todo lo que hay en Drive.
- El favicon (`public/favicon.svg`) sigue siendo el genérico de Vite — pendiente de reemplazar por un ícono real de la marca en Fase 1.
