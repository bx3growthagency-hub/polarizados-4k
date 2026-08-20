# Contexto maestro — Web y simulador de Polarizados 4K

> Documento maestro de producto, experiencia, arquitectura, contenido y desarrollo.
>
> Fecha de elaboración: 20 de agosto de 2026.
>
> Proyecto: Página web premium y simulador automotriz para Polarizados 4K.

---

## 1. Propósito del documento

Este documento reúne en un solo lugar todo el contexto necesario para diseñar, desarrollar, alimentar y validar la nueva página web de **Polarizados 4K**, incluyendo un simulador visual de polarizados y protección PPF inspirado funcionalmente en el visualizador de SunTek.

Puede utilizarse como:

- Brief para un diseñador UI/UX.
- Especificación para un desarrollador front-end o full-stack.
- Documento de referencia para Polarizados 4K.
- Contexto maestro para una inteligencia artificial que vaya a generar la web.
- Base para presupuestar el proyecto.
- Lista de requisitos funcionales y criterios de aceptación.
- Guía para producir las imágenes y máscaras del simulador.

El análisis de SunTek corresponde a una revisión funcional de su página pública, su estructura HTML, sus recursos visibles, sus parámetros de configuración y su comportamiento como usuario. No representa acceso a su repositorio privado ni autoriza copiar código, imágenes, marcas o recursos protegidos.

Referencia analizada:

- [Simulador automotriz de SunTek](https://suntekfilms.com/la/es/paint-protection-film/automotive-film-simulator/)

---

## 2. Resumen ejecutivo

Polarizados 4K necesita una web que no sea simplemente una tarjeta de presentación. La página debe funcionar como un sistema comercial que eduque, genere confianza, permita comparar productos, muestre resultados, capture datos y convierta visitantes en conversaciones de WhatsApp, cotizaciones y citas.

El principal elemento diferenciador será un simulador visual donde el cliente pueda:

1. Elegir un tipo de vehículo.
2. Elegir su necesidad principal.
3. Seleccionar una película o recibir una recomendación.
4. Escoger las áreas que desea polarizar.
5. Aplicar tonos diferentes a cada grupo de vidrios.
6. Cambiar entre vistas interiores y exteriores.
7. Comparar el antes y el después.
8. Agregar coberturas PPF.
9. Ver un precio estimado o un precio “desde”.
10. Enviar toda la configuración a WhatsApp.

La referencia de SunTek demuestra que no es necesario construir un vehículo 3D para crear una experiencia convincente. Su sistema utiliza imágenes 2D prerenderizadas y capas alineadas. Para Polarizados 4K se recomienda mantener este principio, pero implementarlo con tecnología más ligera, imágenes de mayor calidad, una interfaz más comercial y una conexión directa con el portafolio real del negocio.

---

## 3. Contexto de Polarizados 4K

### 3.1. Naturaleza del negocio

Polarizados 4K es un negocio automotriz ubicado en Barranquilla, enfocado en protección, privacidad, confort térmico, seguridad y estética vehicular.

La marca debe proyectarse como un centro especializado, no como un instalador informal. La comunicación debe destacar:

- Calidad de instalación.
- Preparación y protección del vehículo antes de intervenirlo.
- Sala climatizada.
- Limpieza del entorno.
- Precisión en bordes, cortes y terminaciones.
- Productos originales.
- Respaldo de marcas reconocidas.
- Garantías verificables.
- Asesoría según la necesidad y el presupuesto.
- Certificación o condición de centro autorizado cuando corresponda.

### 3.2. Posicionamiento deseado

La página debe posicionar a Polarizados 4K como una alternativa premium, pero capaz de atender diferentes presupuestos.

El mensaje comercial no debe ser únicamente “vendemos polarizados”. Debe comunicar:

> Ayudamos a escoger la protección adecuada para cada vehículo, uso, presupuesto y nivel de confort esperado.

Una idea de comunicación recurrente de la marca es:

> La verdadera diferencia está en lo que no ves.

Esto permite explicar que dos películas pueden verse oscuras, pero diferenciarse en:

- Tecnología.
- Rechazo de calor.
- Protección UV.
- Claridad óptica.
- Durabilidad.
- Estabilidad del color.
- Compatibilidad con señales.
- Calidad del adhesivo.
- Garantía.
- Instalación.

### 3.3. Objetivos de negocio de la web

La web debe ayudar a:

- Aumentar conversaciones calificadas por WhatsApp.
- Reducir preguntas repetitivas.
- Explicar por qué existen diferencias de precio.
- Mostrar evidencia del trabajo.
- Apoyar las campañas de Meta Ads.
- Crear audiencias de remarketing.
- Mejorar el posicionamiento local en Google.
- Fortalecer el perfil de Google Business.
- Generar confianza antes de que el cliente visite el local.
- Facilitar el agendamiento.
- Identificar qué vehículos y productos generan mayor interés.

---

## 4. Portafolio conocido de Polarizados 4K

> Los productos, precios, garantías y especificaciones deben validarse antes de su publicación. Este apartado recoge información conocida del proyecto, pero no sustituye las fichas técnicas oficiales ni una lista comercial aprobada por Polarizados 4K.

### 4.1. Marcas y referencias mencionadas

#### 3M

- 3M Color Stable.
- 3M Ceramic IR.
- 3M Crystalline 75.

#### Spectra

- Spectra HD IR Plus.
- HD Spectra.
- Otras referencias del catálogo vigente por confirmar.

#### Otras líneas mencionadas

- BlackFlint.
- Dimension UV.
- 7H.

### 4.2. Precios internos conocidos

| Producto o referencia | Precio conocido | Estado antes de publicar |
|---|---:|---|
| 3M Ceramic IR | Desde $1.600.000 COP | Confirmar vehículos incluidos y extras |
| Cerámico Dimension UV | $1.100.000 COP | Confirmar nombre, cobertura y garantía de 5 años |
| 7H | $800.000 COP | Confirmar nombre, cobertura y garantía de 3 años |

También se ha mencionado una garantía de hasta 12 años para referencias Spectra. Se debe confirmar:

- Producto exacto.
- Condiciones.
- Cobertura.
- Si la garantía es del fabricante, distribuidor o instalador.
- Documentación que recibe el cliente.

### 4.3. Variables que pueden cambiar el precio

- Tipo y tamaño del vehículo.
- Cantidad y forma de los vidrios.
- Techo panorámico.
- Parabrisas.
- Referencia seleccionada.
- VLT seleccionado.
- Retiro de película anterior.
- Pegamento residual.
- Estado de desempañadores.
- Vidrios reemplazados o modificados.
- Servicios adicionales.
- Promociones vigentes.

La web debe poder mostrar precios exactos, rangos o precios “desde” mediante configuración administrativa.

### 4.4. PPF y protección de superficies

Servicios mencionados:

- Protección de piano black.
- Faros.
- Pantallas.
- Retrovisores.
- Bordes de puertas.
- Manijas.
- Posapiés.
- Área de carga del baúl.
- Capó.
- Defensa.
- Salpicaderas.
- Cobertura completa, si está disponible.

### 4.5. Otros servicios y accesorios

- Insonorización en doble capa.
- Switches y controles.
- Accesorios automotrices.
- Tapetes 5D, si pertenecen al portafolio vigente.
- Bombillos o iluminación, si pertenecen al portafolio permanente.

Cada producto deberá tener un estado administrable:

```json
{
  "id": "tapetes-5d",
  "name": "Tapetes 5D",
  "active": true,
  "showOnHome": false
}
```

---

## 5. Análisis funcional completo del simulador SunTek

### 5.1. Conclusión técnica principal

El simulador de SunTek **no es 3D** y no utiliza un modelo WebGL que gire en tiempo real. Es un configurador de imágenes 2D por capas.

Su flujo es:

```text
Selección de vehículo
→ selección de producto
→ selección de zonas
→ selección de tono o acabado
→ construcción de parámetros
→ composición de capas
→ imagen resultante
```

### 5.2. Categorías de vehículo

El visualizador ofrece:

- Sedan.
- SUV.
- Sport.
- Truck.
- Compact.
- CUV.

Cada categoría contiene:

- Miniatura normal.
- Miniatura de hover.
- Rutas de recursos propias.
- Configuración de capas por vista.
- Experience Fragment específico dentro de Adobe Experience Manager.

No permite elegir una marca, modelo o año específico.

### 5.3. Vistas disponibles

Se detectaron vistas independientes:

- Exterior delantero en tres cuartos.
- Exterior trasero en tres cuartos.
- Interior enfocado en ventanas laterales.
- Interior enfocado en parabrisas.

El botón Interior/Exterior cambia el grupo de imágenes. El carrusel no rota un objeto tridimensional.

Las imágenes inspeccionadas presentaron frecuentemente una resolución natural de 768 × 546 píxeles.

### 5.4. Zonas de polarizado

| Texto mostrado | Identificador interno |
|---|---|
| Ventana lateral trasera | `rearsidewindow` |
| Ventana lateral delantera | `frontsidewindow` |
| Ventana trasera | `backwindow` |
| Tira del visor | `visorstrip` |
| Ventana superior | `roof` |

### 5.5. Relación visual de tonos

| Categoría SunTek | VLT mostrado | Opacidad utilizada |
|---|---:|---:|
| Oscuro | 5–35 | `70` |
| Medio | 35–65 | `50` |
| Claro | 65–95 | `30` |
| Transparente | 95–100 | `0` |

El sistema no representa valores VLT individuales. Convierte rangos generales en opacidades visuales.

### 5.6. Personalización por vidrio

SunTek permite elegir un tono global y luego modificar zonas particulares.

Modelo lógico observado:

```js
{
  globalShade: "dark",
  selectedZones: [
    "rearSideWindow",
    "frontSideWindow",
    "backWindow"
  ],
  zoneShades: {
    rearSideWindow: "medium",
    frontSideWindow: "dark",
    backWindow: "dark"
  }
}
```

Prueba realizada:

- Laterales traseros: opacidad 50.
- Laterales delanteros: opacidad 70.
- Vidrio trasero: opacidad 70.

Esto confirma que la composición final utiliza un mapa independiente por zona.

### 5.7. Zonas PPF

| Texto mostrado | Identificador interno |
|---|---|
| Defensa | `frontbumper` |
| Capó | `hood` |
| Capó parcial | `partialhood` |
| Salpicaderas completas | `fender` |
| Salpicaderas parciales | `partialfender` |
| Espejo lateral | `sidemirror` |
| Paneles laterales | `rockerpanel` |
| Techo | `roof` |
| Puerta | `door` |
| Manijas | `doorhandle` |
| Bordes de puertas | `dooredges` |
| Maletero | `trunk` |
| Cobertura completa | `fullwrap` |

### 5.8. Acabados PPF

- Brillante.
- Negro.
- Mate.

El brillante transparente se representa temporalmente en azul:

```text
opac=70
op_colorize=0,125,197
```

El negro utiliza:

```text
opac=70
op_colorize=0,0,0
```

Las áreas PPF también tienen personalización independiente, mediante grupos como:

```text
frontbumper ppf customization
hood ppf customization
```

### 5.9. Recomendador PPF

SunTek presenta tres grupos de preguntas.

#### Tipo de vía

| Respuesta | Zonas resultantes |
|---|---|
| Autopistas | Capó, capó parcial, salpicaderas, defensa y espejos |
| Caminos suburbanos | Capó, capó parcial, salpicaderas, defensa y espejos |
| Caminos rurales | Paneles laterales bajos |
| Grava | Paneles laterales bajos |

#### Uso del vehículo

| Respuesta | Zonas resultantes |
|---|---|
| Ir a trabajar | Maletero, manijas y bordes de puertas |
| Fines de semana | Maletero |
| Terrenos naturales | Cobertura completa |
| Pista | Paneles laterales bajos |

#### Tipo de estacionamiento

| Respuesta | Zonas resultantes |
|---|---|
| Garaje de casa | Capó, capó parcial, salpicaderas, defensa y espejos |
| Estacionamientos o garajes | Bordes de puertas |
| Calles de ciudad | Cobertura completa |
| Calle del vecindario | Capó, capó parcial, salpicaderas, defensa y espejos |

El algoritmo une las zonas de todas las respuestas y elimina duplicados.

Caso probado:

```text
Autopistas
+ Ir a trabajar
+ Estacionamientos/Garajes

= frontbumper
+ hood
+ partialhood
+ fender
+ sidemirror
+ trunk
+ doorhandle
+ dooredges
```

No utiliza inteligencia artificial. Es una relación JSON entre respuestas y zonas.

### 5.10. Recomendador de polarizados

Los criterios son:

- Precio.
- Rechazo de calor.
- Habilitación de la señal.
- Apariencia.

La interfaz usa dos contenedores de arrastre:

```html
data-rbd-droppable-id="benefit-options"
data-rbd-droppable-id="priority-list"
```

Los elementos tienen identificadores como:

```html
data-rbd-draggable-id="precio"
data-rbd-draggable-id="rechazo-de-calor"
```

La aplicación convierte el orden en una clave:

```text
p1:precio,p2:apariencia,p3:rechazo-de-calor,p4:habilitación-de-la-señal
```

Luego busca esa clave en una tabla de correspondencias.

Productos configurados:

- Carbon.
- Ceramic.
- Dyed Charcoal.
- Metal Dyed.

Ejemplos encontrados:

| Prioridad principal | Resultado inicial frecuente |
|---|---|
| Precio | Dyed Charcoal + Carbon |
| Calor | Ceramic + Metal Dyed |
| Señal | Ceramic + Carbon |
| Apariencia | Ceramic + Dyed Charcoal |

Cada producto incluye título, descripción, imagen y enlace.

### 5.11. Composición de imágenes

El servicio de imágenes es Adobe Dynamic Media:

```text
https://media.eastman.com/is/image/eastman/
```

Patrón simplificado:

```text
imagen-base
?layer=18
&src=is(capa-ventana-delantera)
&opac=70
&layer=11
&src=is(capa-defensa-ppf)
&opac=70
&op_colorize=0,125,197
&preset-de-salida
```

Elementos de la composición:

1. Imagen base del automóvil.
2. Nombre de capa.
3. Imagen fuente de la máscara.
4. Posición u orden.
5. Opacidad.
6. Colorización opcional.
7. Preset de resolución y calidad.

### 5.12. Arquitectura web visible

#### CMS

Adobe Experience Manager, evidenciado por:

- `/etc.clientlibs/`.
- `aem-GridColumn`.
- `/content/eastman/.../jcr:content/`.
- Experience Fragments.
- Clientlibs de sitio y base.

#### Contenedor del visualizador

```html
<tint-viewer
  vehicletypesdata="...JSON..."
  apiendpoint="/content/.../tintviewer.json"
  bootstraped="true">
</tint-viewer>
```

`tint-viewer` funciona como contenedor semántico, no como Web Component nativo registrado. No utiliza Shadow DOM.

#### Configuración embebida

El atributo `vehicletypesdata` contiene aproximadamente 14.849 caracteres de JSON.

Claves principales:

```js
[
  "title",
  "description",
  "selectVehicleCTA",
  "renderMode",
  "information",
  "ppfCovLogic",
  "windowTintRecommendations",
  "vehicleInfo",
  "thumbnailPsdImg",
  "viewYourProductText",
  "dealerSearch",
  "surveyFormTitle",
  "windowTintRecommendationsMapping"
]
```

El valor de `renderMode` es `both`, indicando que soporta polarizado y PPF.

#### Front-end

Evidencias de React:

- Clases `.react-tabs`.
- Atributos `data-rttabs`.
- Renderizado dinámico.
- Componentes de drag and drop compatibles con React Beautiful DnD.

No se puede afirmar la versión exacta de React.

#### Carrusel

Swiper, evidenciado por:

```text
swiper-container
swiper-wrapper
swiper-slide
swiper-slide-duplicate
swiper-slide-active
```

#### Estilos responsivos

Clases similares a Bootstrap:

```text
col-md-2
col-4
d-md-none
d-md-block
```

### 5.13. Funciones adicionales

#### Interior y exterior

Cambian las imágenes disponibles en el carrusel.

#### Ocultar personalizaciones

Al ocultar los efectos, la aplicación vuelve a solicitar una imagen sin las capas seleccionadas. No se limita a ocultarlas con CSS.

#### Descarga

El botón ejecuta una acción JavaScript sin cambiar de página. Se utiliza para guardar la composición actual.

#### Contacto con instalador

El flujo contiene:

- Código postal.
- Búsqueda geográfica.
- Nombre.
- Apellido.
- Email.
- Teléfono.
- Servicios de interés.
- Marca, modelo y año.
- Preferencia de contacto.
- Comentarios.
- Consentimiento.

No se probó el envío final del formulario.

### 5.14. Problemas detectados en SunTek

- Traducciones incompletas: `Customize`, `Download`, `Get Recommendations`.
- Error de escritura: `Selecione`.
- Controles duplicados por el carrusel.
- Elementos interactivos anidados.
- Panel lateral con `aria-hidden="true"` mientras está abierto.
- Tipografía pequeña en algunas áreas.
- Espacios vacíos durante la carga.
- Imágenes limitadas para una experiencia realmente premium.
- Rangos VLT demasiado amplios.
- No muestra precios.
- No muestra legalidad local.
- No explica fichas técnicas en el propio simulador.
- La priorización por arrastre puede resultar incómoda en móvil.

---

## 6. Principios del simulador de Polarizados 4K

### 6.1. Qué se debe conservar de SunTek

- Selección por categoría de vehículo.
- Composición por capas.
- Configuración por zonas.
- Tonos independientes.
- Vistas interiores y exteriores.
- Combinación entre polarizado y PPF.
- Recomendación guiada.
- Resumen descargable o compartible.

### 6.2. Qué se debe mejorar

- Productos reales de 4K.
- Precios o rangos.
- VLT específicos por referencia.
- Interfaz más clara.
- Controles táctiles sencillos.
- Comparador antes/después.
- Explicación de beneficios.
- CTA permanente a WhatsApp.
- Resumen comercial automático.
- Imágenes de mayor resolución.
- Mejor accesibilidad.
- Carga progresiva.
- Seguimiento analítico.
- Recomendación por puntuación, no por una tabla gigantesca.

### 6.3. Qué no debe prometer

- Exactitud fotométrica absoluta.
- Resultado idéntico bajo toda iluminación.
- Valor técnico no respaldado.
- Legalidad universal de un tono.
- Precio definitivo si depende de inspección.

---

## 7. Experiencia del simulador 4K

### Paso 1: vehículo

MVP:

- Sedan.
- SUV.
- Camioneta/pickup.
- Hatchback.
- Deportivo.
- Crossover.

Fase futura:

- Marca.
- Modelo.
- Año.
- Color.

### Paso 2: necesidad

- Reducir calor.
- Obtener privacidad.
- Proteger de rayos UV.
- Conservar alta visibilidad.
- Mejorar apariencia.
- Proteger el interior.
- Trabajar con el vehículo.
- Conducir en carretera o finca.
- Elegir según presupuesto.

### Paso 3: producto

El usuario puede:

- Elegir manualmente.
- Responder preguntas.
- Ver una recomendación principal.
- Comparar una opción económica y una premium.

### Paso 4: zonas

- Laterales delanteros.
- Laterales traseros.
- Vidrio trasero.
- Parabrisas.
- Franja superior.
- Techo panorámico.

### Paso 5: VLT

Se deben utilizar valores reales disponibles por producto, por ejemplo:

- 5%.
- 15%.
- 20%.
- 35%.
- 50%.
- 70%.
- 75%.

No todos los productos ofrecerán los mismos VLT.

### Paso 6: visualización

- Exterior delantero.
- Exterior trasero.
- Interior lateral.
- Interior por parabrisas.
- Antes/después.
- Ocultar/mostrar efecto.
- Día y noche en una fase posterior.

### Paso 7: PPF

El cliente puede agregar:

- Capó.
- Defensa.
- Salpicaderas.
- Espejos.
- Faros.
- Piano black.
- Pantallas.
- Manijas.
- Bordes.
- Área de baúl.
- Cobertura completa.

### Paso 8: resumen

```text
VEHÍCULO: SUV
PRODUCTO: 3M CERAMIC IR
LATERALES DELANTEROS: 35%
LATERALES TRASEROS: 20%
VIDRIO TRASERO: 20%
TECHO PANORÁMICO: 70%
PPF: PIANO BLACK + MANIJAS
PRECIO ESTIMADO: DESDE $X
```

### Paso 9: WhatsApp

```text
Hola, vengo del simulador de Polarizados 4K.

Vehículo: SUV
Producto: 3M Ceramic IR
Laterales delanteros: 35%
Laterales traseros: 20%
Vidrio trasero: 20%
Techo: 70%
PPF: piano black y manijas

Quisiera confirmar el precio y agendar una cita.
```

---

## 8. Recomendador de productos 4K

### 8.1. Enfoque recomendado

En lugar de enumerar manualmente todas las permutaciones, cada producto recibe puntuaciones.

```json
{
  "id": "3m-ceramic-ir",
  "name": "3M Ceramic IR",
  "scores": {
    "heatRejection": 5,
    "uvProtection": 5,
    "privacy": 4,
    "opticalClarity": 4,
    "signalCompatibility": 5,
    "appearance": 4,
    "durability": 5,
    "budget": 2
  }
}
```

Las prioridades reciben pesos:

| Posición | Peso |
|---|---:|
| Primera | 5 |
| Segunda | 4 |
| Tercera | 3 |
| Cuarta | 2 |
| Quinta | 1 |

Fórmula conceptual:

```ts
score =
  product.heatRejection * heatWeight +
  product.privacy * privacyWeight +
  product.signalCompatibility * signalWeight +
  product.budget * budgetWeight;
```

### 8.2. Resultado

Mostrar:

- Recomendación principal.
- Alternativa más económica.
- Alternativa premium.
- Explicación en lenguaje sencillo.
- Precio desde.
- Garantía.
- CTA para aplicarla en el simulador.

### 8.3. Fuente de los valores

Los puntajes deben construirse con:

- Fichas técnicas oficiales.
- Catálogo vigente.
- Experiencia de instaladores.
- Garantías reales.
- Disponibilidad real.

No deben inventarse porcentajes de IR, UV o TSER.

---

## 9. Recomendador PPF de 4K

Preguntas sugeridas:

1. ¿Por dónde conduces con mayor frecuencia?
2. ¿Dónde estacionas?
3. ¿Qué partes te preocupan más?
4. ¿El vehículo es nuevo?
5. ¿Lo utilizas para carretera, finca o ciudad?
6. ¿Buscas protección puntual o completa?
7. ¿Cuál es tu presupuesto aproximado?

Reglas de ejemplo:

```json
{
  "highway": ["hood", "bumper", "fenders", "mirrors", "headlights"],
  "cityParking": ["doorEdges", "doorHandles", "mirrors"],
  "ruralRoad": ["rockerPanels", "bumper", "fenders"],
  "newVehicle": ["fullFront"],
  "panoramicInterior": ["pianoBlack", "screens"]
}
```

La respuesta debe explicar el riesgo:

> Te recomendamos proteger capó, defensa, espejos y faros porque son las zonas que reciben mayor impacto de piedras e insectos durante recorridos por carretera.

---

## 10. Arquitectura técnica propuesta

### 10.1. Front-end

Recomendado:

- React.
- TypeScript.
- Vite o Next.js.
- CSS Modules, Tailwind o sistema de diseño propio.
- Canvas para composición avanzada.
- Zustand o `useReducer` para estado.
- Swiper únicamente si se necesita carrusel táctil.

### 10.2. Decisión según Hostinger

Si el plan contratado es hosting compartido sin Node.js:

- React + Vite.
- Next.js con exportación estática.
- Archivos generados en `dist` u `out`.
- Despliegue por FTP, Git o administrador de archivos.

Si se utiliza VPS o plan compatible con Node:

- Next.js con renderizado dinámico.
- API propia.
- Panel administrativo.
- Generación de configuraciones compartibles.

### 10.3. Datos

Primera versión:

- JSON local.
- Productos.
- Precios.
- Vehículos.
- Capas.
- Proyectos.
- Preguntas frecuentes.
- Información de contacto.

Fase futura:

- Supabase.
- Firebase.
- CMS headless.
- Panel administrativo propio.

### 10.4. Recursos

- Cloudinary.
- Cloudflare Images.
- CDN de Hostinger.
- Supabase Storage.

La elección debe permitir caché, WebP/AVIF y entrega rápida en Colombia.

---

## 11. Modelo de estado

```ts
type VehicleType =
  | "sedan"
  | "suv"
  | "truck"
  | "hatchback"
  | "sport"
  | "crossover";

type VehicleView =
  | "frontExterior"
  | "rearExterior"
  | "sideInterior"
  | "windshieldInterior";

type TintZone =
  | "frontWindows"
  | "rearWindows"
  | "rearWindshield"
  | "windshield"
  | "visorStrip"
  | "panoramicRoof";

type PpfZone =
  | "hood"
  | "partialHood"
  | "frontBumper"
  | "fenders"
  | "mirrors"
  | "headlights"
  | "rockerPanels"
  | "doors"
  | "doorHandles"
  | "doorEdges"
  | "pianoBlack"
  | "screens"
  | "trunkArea"
  | "fullWrap";

interface SimulatorState {
  vehicleType: VehicleType | null;
  activeView: VehicleView;
  selectedProductId: string | null;
  tintZones: Partial<Record<TintZone, string>>;
  ppfZones: Partial<Record<PpfZone, "gloss" | "matte" | "black">>;
  priorities: string[];
  estimatedPrice: number | null;
  showCustomizations: boolean;
  comparisonPosition: number;
}
```

---

## 12. Modelo de producto

```ts
interface FilmProduct {
  id: string;
  brand: string;
  name: string;
  slug: string;
  category: "dyed" | "carbon" | "ceramic" | "premium";
  description: string;
  shortDescription: string;
  availableVlt: number[];
  warrantyYears: number | null;
  specs: {
    uvRejection?: number;
    irRejection?: number;
    tser?: number;
    glareReduction?: number;
    signalCompatible?: boolean;
  };
  scores: {
    heatRejection: number;
    privacy: number;
    opticalClarity: number;
    signalCompatibility: number;
    appearance: number;
    durability: number;
    budget: number;
  };
  prices: Record<string, number | null>;
  active: boolean;
}
```

Ejemplo provisional:

```json
{
  "id": "3m-ceramic-ir",
  "brand": "3M",
  "name": "Ceramic IR",
  "slug": "3m-ceramic-ir",
  "category": "ceramic",
  "description": "Película cerámica orientada al control de calor y la protección interior.",
  "availableVlt": [],
  "warrantyYears": null,
  "specs": {},
  "prices": {
    "sedan": 1600000,
    "suv": null,
    "truck": null
  },
  "active": true
}
```

Los campos vacíos deben completarse con información aprobada.

---

## 13. Producción visual del simulador

### 13.1. Fotografías base

Por cada categoría:

- Exterior delantero.
- Exterior trasero.
- Interior lateral.
- Interior parabrisas.

Resolución:

- Mínimo: 1600 × 1000.
- Recomendado: 2400 × 1500.
- Mantener relación uniforme.

### 13.2. Requisitos de fotografía o render

- Cámara fija.
- Perspectiva consistente.
- Iluminación controlada.
- Fondo limpio.
- Carro inmóvil.
- Reflejos controlados.
- Vidrios visibles.
- Diferenciación clara entre interior y exterior.
- Suficiente espacio alrededor para la interfaz.

### 13.3. Máscaras

Todas las máscaras deben:

- Tener las mismas dimensiones de la base.
- Mantener el mismo origen.
- Usar transparencia real.
- Respetar sellos, pilares, marcos y reflejos.
- Evitar halos blancos.
- Mantener bordes suaves.

### 13.4. Estructura de archivos

```text
/assets/simulator/
  /sedan/
    /front-exterior/
      base.webp
      tint-front-windows.webp
      tint-rear-windows.webp
      tint-windshield.webp
      tint-roof.webp
      ppf-hood.webp
      ppf-bumper.webp
      ppf-fenders.webp
      ppf-mirrors.webp
    /rear-exterior/
      base.webp
      tint-front-windows.webp
      tint-rear-windows.webp
      tint-rear-windshield.webp
      ppf-trunk.webp
    /side-interior/
      base.webp
      tint-front-windows.webp
      tint-rear-windows.webp
    /windshield-interior/
      base.webp
      tint-windshield.webp
      tint-visor-strip.webp
```

### 13.5. Composición CSS básica

```jsx
<div className="vehicle-preview">
  <img src={baseImage} className="layer base-layer" alt="Vehículo" />

  {visibleLayers.map(layer => (
    <img
      key={layer.id}
      src={layer.src}
      className="layer effect-layer"
      style={{
        opacity: layer.opacity,
        mixBlendMode: layer.blendMode
      }}
      alt=""
    />
  ))}
</div>
```

```css
.vehicle-preview {
  position: relative;
  width: 100%;
  aspect-ratio: 8 / 5;
}

.layer {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: contain;
}
```

### 13.6. Canvas recomendado

Para más control:

1. Dibujar base.
2. Dibujar máscara alfa.
3. Aplicar color y opacidad.
4. Aplicar modo de mezcla.
5. Dibujar reflejos superiores.
6. Exportar a PNG o WebP.

Canvas permitirá:

- Descargar resultado.
- Compartir imagen.
- Añadir logo.
- Añadir resumen.
- Generar una miniatura para WhatsApp.

---

## 14. Sistema de precios

```json
{
  "productId": "3m-ceramic-ir",
  "vehiclePrices": {
    "sedan": 1600000,
    "suv": 0,
    "truck": 0
  },
  "extras": {
    "windshield": 0,
    "panoramicRoof": 0,
    "removeOldFilm": 0
  },
  "display": {
    "showExact": false,
    "showFrom": true
  }
}
```

Regla recomendada:

```ts
estimatedPrice =
  baseVehiclePrice +
  windshieldExtra +
  roofExtra +
  removalExtra +
  selectedPpfZonesTotal;
```

Si un valor no está disponible:

```text
Precio sujeto a confirmación según vehículo.
```

---

## 15. Estructura completa del sitio

### 15.1. Inicio

1. Hero premium.
2. Propuesta de valor.
3. CTA al simulador.
4. CTA a WhatsApp.
5. Marcas.
6. Servicios.
7. Comparación de tecnologías.
8. Proyectos reales.
9. Proceso de instalación.
10. Garantías.
11. Testimonios.
12. Ubicación.
13. Preguntas frecuentes.
14. CTA final.

### 15.2. Polarizados

- Qué es VLT.
- Privacidad vs. rechazo de calor.
- UV, IR y TSER.
- Película tradicional.
- Carbono.
- Cerámica.
- Tecnología premium.
- Productos 4K.
- Precios.
- Garantías.
- Comparador.
- Preguntas frecuentes.

### 15.3. PPF

- Qué protege.
- Riesgos cotidianos.
- Zonas.
- PPF vs. cerámico.
- Acabados.
- Cuidados.
- Garantías.
- Proyectos.
- Cotización.

### 15.4. Otros servicios

- Insonorización.
- Accesorios.
- Switches.
- Tapetes.
- Iluminación.
- Servicios activos confirmados.

### 15.5. Proyectos

Cada caso debe contener:

- Vehículo.
- Necesidad.
- Producto instalado.
- Motivo de recomendación.
- Resultado.
- Fotos.
- Video.
- CTA.

Casos de contenido ya trabajados que pueden inspirar esta sección:

- Tesla Model Y con Ceramic IR, incluyendo techo.
- Mazda CX-5 con Ceramic IR y certificado.
- Renault Clio 2008 con Ceramic IR como ejemplo de que el valor del vehículo no define la necesidad de confort.
- Audi SQ5.
- Renault Koleos.
- Mazda 3.

### 15.6. Marcas y garantías

- Marca.
- Producto.
- Tecnología.
- Garantía.
- Certificación.
- Qué cubre.
- Qué no cubre.
- Recomendaciones de cuidado.

### 15.7. Contacto

- Dirección.
- Mapa.
- WhatsApp.
- Teléfono.
- Horarios.
- Instagram.
- Formulario breve.
- Cómo llegar.
- Botón de agendamiento.

---

## 16. Diseño visual

### 16.1. Estética

- Automotriz premium.
- Moderna.
- Oscura.
- Minimalista.
- Tecnológica sin parecer videojuego.
- Fotografías grandes.
- Alto contraste.
- Espaciado amplio.
- Microanimaciones.
- Reflejos suaves.
- Bordes sobrios.

### 16.2. Evitar

- Plantilla genérica.
- Exceso de neón.
- Títulos en cursiva.
- Animaciones invasivas.
- Fondos saturados.
- Párrafos extensos sin jerarquía.
- Carruseles automáticos rápidos.
- Botones poco claros.

### 16.3. Tipografía

- Space Grotesk.
- Manrope.
- Inter.
- Sora.

Combinación sugerida:

- Títulos: Space Grotesk.
- Texto: Inter o Manrope.

### 16.4. Paleta base provisional

```css
:root {
  --black: #070809;
  --graphite: #111317;
  --graphite-soft: #1A1D22;
  --white: #F5F7FA;
  --gray: #9BA1AA;
  --border: rgba(255, 255, 255, 0.10);
  --accent: var(--brand-color-confirmed);
}
```

El acento debe tomarse del logo oficial.

---

## 17. SEO local

### Palabras clave iniciales

- Polarizados en Barranquilla.
- Polarizados para carros Barranquilla.
- Polarizados 3M Barranquilla.
- 3M Ceramic IR Barranquilla.
- Polarizado cerámico Barranquilla.
- PPF Barranquilla.
- Protección de pintura Barranquilla.
- Polarizado para techo panorámico.
- Polarizados con garantía Barranquilla.
- Instalación de polarizados cerca de mí.

### Implementación

- Títulos únicos.
- Metadescripciones.
- Encabezados jerárquicos.
- URLs limpias.
- Sitemap.
- `robots.txt`.
- Canonical.
- Open Graph.
- Datos estructurados.
- Texto alternativo.
- Dirección consistente.
- Mapa.
- Reseñas.
- Preguntas frecuentes.
- Google Search Console.
- Google Business Profile.

### Ejemplos de URLs

```text
/
/polarizados/
/polarizados/3m-ceramic-ir/
/polarizados/3m-crystalline-75/
/ppf/
/simulador/
/proyectos/
/garantias/
/contacto/
```

---

## 18. Analítica y publicidad

Integraciones:

- Google Analytics 4.
- Google Search Console.
- Meta Pixel.
- Google Business Profile.
- UTMs.
- Consentimiento de cookies cuando corresponda.

Eventos:

```text
vehicle_selected
need_selected
product_selected
tint_zone_selected
tint_vlt_selected
ppf_zone_selected
recommendation_started
recommendation_completed
simulator_completed
price_viewed
whatsapp_clicked
call_clicked
map_clicked
appointment_started
form_submitted
project_viewed
```

Eventos Meta sugeridos:

- `ViewContent`.
- `Lead`.
- `Contact`.
- `Schedule`.

Audiencias futuras:

- Usuarios del simulador.
- Interesados en Ceramic IR.
- Interesados en PPF.
- Visitantes de precios.
- Usuarios que llegaron al resumen pero no escribieron.
- Visitantes recurrentes.

---

## 19. Rendimiento y accesibilidad

### Rendimiento

- LCP inferior a 2,5 segundos.
- Imágenes WebP/AVIF.
- Lazy loading.
- Precargar únicamente vehículo y vista activos.
- Caché de capas.
- Skeleton de carga.
- Evitar descargar todas las máscaras al inicio.
- Comprimir fuentes.
- Minimizar JavaScript.

### Accesibilidad

- Botones de mínimo 44 × 44 px.
- Navegación por teclado.
- Estados de foco visibles.
- Etiquetas claras.
- No depender solo del color.
- Texto alternativo útil.
- `aria-live` para cambios de precio y recomendación.
- No duplicar controles del carrusel.
- Evitar botones dentro de botones.

### Móvil

- Panel de opciones tipo pasos.
- Preview visible o fijado cuando sea posible.
- CTA inferior permanente.
- No depender exclusivamente de drag and drop.
- Prioridades seleccionables con números o botones.

---

## 20. Seguridad y privacidad

- SSL y HTTPS.
- Validación de formularios.
- Protección anti-spam.
- Límites de solicitudes.
- Variables de entorno.
- Claves fuera del repositorio público.
- Política de privacidad.
- Autorización de tratamiento de datos.
- Copias de seguridad.
- Actualizaciones.
- Formularios enviados por HTTPS.
- No exponer credenciales en JavaScript.

---

## 21. Avisos legales del simulador

Texto sugerido:

> Las imágenes son representaciones digitales con fines ilustrativos. El color, la privacidad y la apariencia real pueden variar según la iluminación, el vidrio original, el vehículo y la referencia instalada.

Texto sobre VLT:

> La disponibilidad y aplicación de determinados niveles de transmisión de luz puede depender de la referencia, el vehículo y la normativa vigente. Consulta con nuestro equipo antes de realizar la instalación.

Texto sobre precios:

> Los valores mostrados son estimados o precios desde. La cotización final puede variar según el tipo de vehículo, las áreas seleccionadas, el estado de los vidrios y los servicios adicionales.

---

## 22. Fases de desarrollo

### Fase 1 — Web comercial

- Inicio.
- Servicios.
- Productos.
- Proyectos.
- Marcas.
- Garantías.
- Testimonios.
- Contacto.
- WhatsApp.
- SEO.
- Analytics.
- Meta Pixel.

### Fase 2 — Simulador MVP

- Sedan, SUV y camioneta.
- Cuatro vistas.
- Polarizado.
- VLT.
- Productos.
- Antes/después.
- Precio desde.
- Resumen.
- WhatsApp.

### Fase 3 — PPF

- Zonas PPF.
- Acabados.
- Recomendador.
- Cotización por zona.
- Combinación con polarizado.

### Fase 4 — Plataforma avanzada

- Modelos específicos.
- Panel administrativo.
- CRM.
- Agendamiento.
- Configuraciones compartibles.
- Carga de fotografía.
- Visualización asistida por IA.
- Precios dinámicos.

---

## 23. Criterios de aceptación

La primera versión se considera lista cuando:

- Funciona correctamente en móvil y escritorio.
- Permite seleccionar al menos tres tipos de vehículo.
- Permite escoger un producto.
- Permite aplicar tonos por zona.
- Permite cambiar entre vistas.
- Tiene antes/después.
- Genera resumen.
- Genera mensaje de WhatsApp.
- Muestra precios configurables.
- Los productos se alimentan desde datos editables.
- Carga sin errores visibles.
- Las máscaras están alineadas.
- Tiene avisos legales.
- Registra eventos principales.
- Tiene metadatos SEO.
- Tiene SSL.
- La información de contacto está verificada.

---

## 24. Pruebas requeridas

### Funcionales

- Selección de cada vehículo.
- Selección de cada producto.
- Selección y eliminación de zonas.
- Cambio de VLT global e individual.
- Combinación de polarizado y PPF.
- Reinicio.
- Interior/exterior.
- Antes/después.
- Descarga.
- WhatsApp.
- Formulario.
- Precios.

### Visuales

- Alineación de máscaras.
- Bordes de vidrios.
- Reflejos.
- Escalado responsive.
- Carga sin saltos.
- Contraste.

### Técnicas

- Chrome.
- Safari.
- Edge.
- Android.
- iPhone.
- Conexión móvil lenta.
- Lighthouse.
- Accesibilidad por teclado.

---

## 25. Información pendiente de Polarizados 4K

Antes de publicación:

- Dirección exacta.
- Número principal.
- WhatsApp.
- Horarios.
- Email.
- Instagram.
- Facebook.
- TikTok.
- Logo vectorial.
- Colores oficiales.
- Fotografías del local.
- Certificaciones.
- Marcas vigentes.
- Referencias activas.
- Fichas técnicas.
- VLT por producto.
- Garantía por producto.
- Precio por tipo de vehículo.
- Precio de parabrisas.
- Precio de techos.
- Precio de retiro de película.
- Precio PPF por zona.
- Tiempo de instalación.
- Métodos de pago.
- Política de garantía.
- Condiciones de reserva.
- Reseñas autorizadas.

Nada pendiente debe completarse con información inventada.

---

## 26. Contexto maestro listo para una IA desarrolladora

```text
Actúa como un equipo senior compuesto por estratega digital, diseñador UI/UX,
desarrollador front-end, especialista en rendimiento, SEO local y conversión.

Debes diseñar y desarrollar una página web premium para Polarizados 4K,
negocio automotriz ubicado en Barranquilla y especializado en polarizados,
películas cerámicas, control solar, PPF, insonorización y accesorios.

El objetivo principal no es un ecommerce tradicional. La web debe educar,
generar confianza, mostrar proyectos, ayudar a escoger un producto y convertir
visitantes en conversaciones calificadas de WhatsApp y citas.

El principal diferenciador será un simulador visual de polarizados y PPF.
La referencia funcional es el simulador de SunTek, pero no debes copiar su
código, imágenes, textos, marcas ni diseño. Debes utilizar un sistema propio
de imágenes 2D y máscaras alineadas.

El simulador debe permitir:

1. Elegir sedan, SUV, camioneta, hatchback, deportivo o crossover.
2. Elegir una necesidad: calor, privacidad, UV, visibilidad, apariencia,
   trabajo, carretera, finca o presupuesto.
3. Elegir un producto o recibir una recomendación.
4. Escoger laterales delanteros, laterales traseros, vidrio trasero,
   parabrisas, franja y techo panorámico.
5. Aplicar VLT por zona.
6. Cambiar entre exterior delantero, exterior trasero, interior lateral e
   interior por parabrisas.
7. Comparar antes y después.
8. Agregar zonas PPF.
9. Ver un precio desde o estimado.
10. Generar un resumen y enviarlo a WhatsApp.

La interfaz debe ser completamente en español, premium, automotriz, oscura,
minimalista, rápida y optimizada para móvil. Utiliza tipografías sans serif
rectas y evita cursivas, plantillas genéricas, neón excesivo y animaciones
invasivas.

Productos conocidos que deben modelarse, pendientes de validación final:

- 3M Color Stable.
- 3M Ceramic IR.
- 3M Crystalline 75.
- Spectra HD IR Plus.
- HD Spectra.
- BlackFlint.
- Dimension UV.
- 7H.

Precios internos conocidos, pendientes de aprobación:

- 3M Ceramic IR desde $1.600.000 COP.
- Dimension UV alrededor de $1.100.000 COP.
- 7H alrededor de $800.000 COP.

No inventes especificaciones, porcentajes, garantías, dirección, teléfono,
horarios ni precios faltantes. Utiliza campos pendientes claramente marcados.

La web debe incluir:

- Inicio.
- Polarizados.
- PPF.
- Otros servicios.
- Simulador.
- Proyectos.
- Marcas y garantías.
- Preguntas frecuentes.
- Contacto.

Debe integrar Google Analytics 4, Search Console, Meta Pixel, SEO local,
Google Business Profile, WhatsApp, mapa, formularios seguros, HTTPS y eventos
personalizados.

Prioriza rendimiento, accesibilidad, claridad comercial y facilidad de
mantenimiento. Los productos, precios, proyectos, garantías y preguntas deben
estar separados del código de interfaz mediante archivos JSON o un CMS.

El resultado debe sentirse como una herramienta comercial premium, no como
una demostración tecnológica. Cada paso debe acercar al usuario a entender,
escoger, cotizar y agendar.
```

---

## 27. Conclusión

El valor principal del proyecto estará en combinar cuatro elementos:

1. **Información comercial clara:** explicar diferencias, beneficios, garantías y precios.
2. **Prueba visual:** mostrar cómo podría verse el vehículo.
3. **Confianza:** evidenciar procesos, proyectos, certificaciones y resultados.
4. **Conversión:** enviar una solicitud estructurada a WhatsApp.

La referencia de SunTek confirma que una composición 2D por capas es suficiente para crear un simulador útil. Polarizados 4K puede superar esa experiencia si utiliza mejores imágenes, una interfaz móvil más sencilla, productos y precios reales, un recomendador explicativo y una conexión inmediata con el equipo comercial.

La prioridad no debe ser construir el sistema más complejo, sino el sistema que ayude a más clientes a tomar una decisión y contactar a Polarizados 4K con una necesidad clara.
