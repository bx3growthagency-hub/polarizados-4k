# CLAUDE.md — Polarizados 4K

Contexto permanente para trabajar en este repo. Léelo antes de tocar código. El estado actual del proyecto (qué está hecho, qué falta, próxima tarea) vive en `docs/HANDOFF.md`, no acá — este archivo es de reglas estables, no de estado.

## Qué es este proyecto

Sitio web comercial para Polarizados 4K (polarizados, PPF, cerámicos, wraps, accesorios automotrices — Barranquilla). Vendido por BX3 Growth Agency como primer proyecto formal de desarrollo web/software, con valor comercial de 500.000 COP — un presupuesto simbólico, no un proyecto enterprise. El alcance debe reflejar eso: sitio comercial pulido, sin sobreingeniería.

Historia: este repo se generó a partir de dos documentos maestros de negocio (`docs/CONTEXTO_MAESTRO_POLARIZADOS_4K.md` y `docs/Contexto_maestro_web_Polarizados_4K_2026-08-20.md`) y un export de assets de Google Drive. El plan de arquitectura completo (decisiones, alternativas consideradas, riesgos) está documentado — pedir a Leandro (BX3) si hace falta el detalle completo del proceso de planeación.

## Regla más importante: no inventar información comercial

Los documentos maestros son explícitos y hay que tratarlos como ley: **nunca** inventar años de experiencia, fundadores, cifras de clientes, premios, certificaciones, alianzas, porcentajes técnicos, testimonios, garantías o precios. Si un dato no está marcado `confirmed_repeated` en `src/data/*.json`, no se publica como hecho — se omite o se resuelve con "Cotiza por WhatsApp".

Esto no es una sugerencia de estilo, es la regla que más le importa al cliente y a BX3 (ver sección 1 y 21 de `docs/CONTEXTO_MAESTRO_POLARIZADOS_4K.md`). Si hace falta un dato que no está en `src/data/`, hay que pedirlo — no rellenarlo con algo plausible.

Nombre de marca: siempre **"Polarizados 4K"**, nunca "4K Polarizados".

## Alcance de Fase 1 (lo que sí se construye ahora)

Web comercial multipágina: Inicio, Polarizados, PPF, Otros servicios, Proyectos, Nosotros, Contacto. CTA de WhatsApp en todo. SEO local básico. Sin backend, sin CMS, sin autenticación, sin base de datos.

**Fuera de alcance** (documentado en `docs/HANDOFF.md`, no descartado — son fases futuras con presupuesto propio): simulador visual de polarizados/PPF, cotizador automático de precios, blog, panel administrativo, CRM, multi-idioma, testimonios (hasta tener reseñas reales verificadas).

No agregar nada de la lista de "fuera de alcance" sin que Leandro lo apruebe explícitamente primero — es fácil justificar "ya que estoy" pero cambia el presupuesto y el tiempo de entrega.

## Stack y reglas de código

- React + TypeScript + Vite, build estático (`dist/`).
- Sin Tailwind ni librerías de UI — CSS con las variables de `src/styles/tokens.css`. El sitio es mayormente contenido/marketing, no justifica esa dependencia.
- Antes de instalar cualquier paquete nuevo: confirmar que no se puede resolver con lo que ya hay, y decir en una línea por qué hace falta.
- Contenido separado de la UI: todo lo que pueda cambiar (productos, precios, proyectos, FAQ, contacto) vive en `src/data/*.json`, no hardcodeado en componentes.
- Mobile-first. Ningún componente se da por terminado si solo se probó en desktop.
- Rendimiento: imágenes en WebP, lazy loading, evitar JS innecesario. Las fotos en `public/assets/photos-raw/` son originales sin optimizar — no usarlas directo en producción, hay que procesarlas primero.

## Comandos

```bash
npm install
npm run dev       # desarrollo
npm run build     # build de producción (incluye chequeo de TypeScript)
npm run preview   # sirve el build local
npm run lint       # oxlint
```

## Git

Commits en hitos naturales (una página completa, un lote de componentes relacionados), no después de cada archivo suelto. Nunca commitear `.env.local` ni credenciales — usar `.env.example` como referencia de qué variables existen. `references/` está en `.gitignore` a propósito (PDFs/video pesados) — no forzar su versionado.

## Colaboración BX3 (Colombia/España) + Hurtado

Este proyecto lo continúa Hurtado desde Colombia. No asumas que quien lee el código estuvo en la conversación donde se tomaron las decisiones — si tomás una decisión de arquitectura o de alcance no trivial, dejala escrita en `docs/HANDOFF.md`, no solo en el historial de chat.
