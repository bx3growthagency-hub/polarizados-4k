# Polarizados 4K — Web

Sitio web comercial de **Polarizados 4K**, centro de polarizados/PPF/cerámicos automotrices en Barranquilla. Proyecto de **BX3 Growth Agency**.

> Antes de tocar código, lee `docs/HANDOFF.md` — tiene el estado real del proyecto, las tareas priorizadas de Fase 1 y las decisiones ya tomadas. `CLAUDE.md` tiene las reglas de trabajo de este repo.

## Stack

React + TypeScript + Vite, exportado como sitio estático. Sin backend, sin CMS, sin base de datos (ver `CLAUDE.md` para el porqué).

## Cómo clonar y correr

```bash
git clone https://github.com/bx3growthagency-hub/polarizados-4k.git
cd polarizados-4k
npm install
npm run dev
```

## Scripts

| Comando | Qué hace |
|---|---|
| `npm run dev` | Servidor de desarrollo con hot reload |
| `npm run build` | Build de producción a `dist/` (incluye chequeo de TypeScript) |
| `npm run preview` | Sirve el build de `dist/` localmente para probarlo |
| `npm run lint` | Lint con oxlint |

## Despliegue

Pensado para exportarse estático (`dist/`) y subirse a Hostinger (hosting compartido o VPS — cualquiera de los dos funciona con este enfoque). No hay confirmación todavía de dominio/plan contratado — ver `docs/HANDOFF.md`.

## Estructura del proyecto

```
polarizados-4k/
├── docs/                    # contexto de negocio + HANDOFF.md (estado del proyecto)
├── tasks/                   # tareas priorizadas de Fase 1
├── references/              # material crudo de Drive (PDFs pesados, video) — no versionado en git
├── public/assets/
│   ├── logos/                # logo oficial de Polarizados 4K
│   ├── brand-partners/       # logos de marcas aliadas (3M, Spectra)
│   └── photos-raw/           # 22 fotos sin curar, pendientes de selección/optimización
└── src/
    ├── pages/                # páginas de Fase 1 (pendientes de construir)
    ├── components/           # componentes reutilizables (pendientes de construir)
    ├── data/                 # contenido en JSON, separado de la UI (contact, products, projects, faq)
    ├── styles/                # tokens.css — paleta y tipografía
    └── lib/                   # utilidades (WhatsApp, analytics — pendientes)
```

## Variables de entorno

Copiar `.env.example` a `.env.local` y completar cuando el cliente entregue IDs de Analytics/Meta Pixel, número de WhatsApp confirmado, etc. Nunca commitear `.env.local`.

## Regla de oro del contenido

Ningún dato comercial (precio, garantía, dirección, certificación, testimonio) se publica sin estar marcado `confirmed_repeated` en `src/data/*.json`. Ver `docs/CONTEXTO_MAESTRO_POLARIZADOS_4K.md` para el porqué.
