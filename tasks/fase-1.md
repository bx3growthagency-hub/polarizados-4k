# Fase 1 — Web comercial (sin simulador)

Tareas priorizadas para construir el sitio dentro del alcance de los 500.000 COP. Orden sugerido — no es obligatorio seguirlo exacto, pero los primeros 3 bloques son dependencias del resto.

## 0. Curación de assets (antes de maquetar cualquier página)

- [ ] Revisar las 22 fotos en `public/assets/photos-raw/`, descartar duplicados (`IMG_1674(1)`, `IMG_1690(1)`, `IMG_2954(1)`), elegir 8-15 finales.
- [ ] Optimizar las elegidas a WebP (ej. con `sharp`, `squoosh` o el optimizador de imágenes que se prefiera — justificar si se agrega como dependencia de build).
- [ ] Samplear el hex exacto del rojo del logo (`public/assets/logos/logo-4k-completo.png`) y confirmar/ajustar `--color-accent` en `src/styles/tokens.css`.
- [ ] Reemplazar `public/favicon.svg` (genérico de Vite) por un ícono real de la marca.

## 1. Layout base

- [ ] `src/components/Header.tsx` — logo + navegación a las 6 páginas.
- [ ] `src/components/Footer.tsx` — contacto básico, redes, año.
- [ ] `src/components/WhatsAppButton.tsx` — flotante, mobile-first, mínimo 44×44px, mensaje pre-cargado configurable por página.
- [ ] `src/lib/whatsapp.ts` — helper que arma el link `wa.me/<numero>?text=<mensaje>` a partir del número en `src/data/contact.json`.
- [ ] Router (agregar `react-router` — único paquete nuevo justificado para Fase 1, dado que se confirmó sitio multipágina) y layout compartido.

## 2. Páginas

- [ ] `Home` — hero, propuesta de valor, resumen de servicios con link a cada página, marcas trabajadas (solo si autorización 3M/Spectra está confirmada), 3-4 proyectos destacados, CTA WhatsApp, ubicación, FAQ resumida.
- [ ] `Polarizados` — tecnologías desde `src/data/products.json` (campo `polarizados`), comparación simple, CTA "cotiza tu vehículo".
- [ ] `Ppf` — qué protege, zonas (ver `docs/Contexto_maestro_web_Polarizados_4K_2026-08-20.md` sección 8.3 del doc de negocio), CTA cotización.
- [ ] `OtrosServicios` — cerámicos, wraps, accesorios, insonorización agrupados en una sola página.
- [ ] `Proyectos` — galería desde `src/data/projects.json`, con las fotos curadas del paso 0.
- [ ] `Nosotros` — corta, solo lo confirmado (sin historia/fundadores/años inventados).
- [ ] `Contacto` — WhatsApp, dirección (marcar "pendiente de confirmar" si `src/data/contact.json` sigue en `pending_validation`), mapa (si hay URL), formulario corto: nombre, marca, modelo, año, tipo de servicio, necesidad. Sin campo de presupuesto obligatorio.

## 3. SEO on-page

- [ ] Título + meta description únicos por página.
- [ ] Un H1 claro por página, jerarquía H2/H3 coherente.
- [ ] URLs limpias (`/polarizados`, `/ppf`, `/servicios`, `/proyectos`, `/nosotros`, `/contacto`).
- [ ] `sitemap.xml` y `robots.txt`.
- [ ] Alt text real (no genérico) en todas las imágenes.
- [ ] Open Graph básico (título, descripción, imagen) para compartir en redes.

## 4. Rendimiento y QA (antes de dar por terminada la Fase 1)

- [ ] `npm run build` sin errores.
- [ ] Revisión responsive real: móvil, tablet, desktop (no solo desktop).
- [ ] Todos los botones de WhatsApp abren con el mensaje correcto por página.
- [ ] Lighthouse básico (performance/accesibilidad/SEO) — sin bloquear por puntaje perfecto, pero sin regresiones obvias.
- [ ] Ningún dato en pantalla que no esté marcado `confirmed_repeated` en `src/data/*.json`.
- [ ] `docs/HANDOFF.md` actualizado con el estado real antes de cualquier pausa larga.

## Explícitamente fuera de esta lista

Simulador visual, cotizador automático, blog, panel admin, CRM, multi-idioma, testimonios sin verificar — ver `CLAUDE.md` para el porqué. No agregar sin aprobación explícita de Leandro (BX3).
