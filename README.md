# Cafh Oficina Digital

Plataforma interna de gestión de Cafh. Reúne en una sola aplicación los módulos de
coordinación de la institución —sedes, comunidades, seminarios, finanzas, actividades
de extensión— junto al módulo de **Gestión de Redes Sociales**.

**Archivo vigente:** `index.html`

Es un único archivo HTML. No requiere instalación, servidor ni base de datos: se abre
con doble clic en cualquier navegador moderno.

---

## Cómo abrirla

**En su propia computadora:** doble clic sobre el archivo.

**Publicada en GitHub Pages:** en **Settings → Pages**, elija la rama `main` y la
carpeta raíz `/`. En aproximadamente un minuto queda disponible en
`https://USUARIO.github.io/REPOSITORIO/`. Ese enlace se abre en cualquier celular o
computadora, sin cuenta y sin instalar nada, y puede enviarse por WhatsApp o correo.

> **Atención:** una página publicada en GitHub Pages es **pública** y la indexan los
> buscadores. No lleva contraseña. En el plan gratuito, además, Pages sólo publica desde
> repositorios públicos: el código queda a la vista de cualquiera. Por eso este archivo
> no contiene ningún correo personal (ver *Destinatarios del reporte*).

### Qué subir al repositorio

Sólo `index.html` y `README.md`. Las versiones anteriores no hacen falta: el historial
pasa a ser el de Git, y cada versión puede marcarse con una etiqueta (`git tag v7`).

> **Antes del primer commit:** el historial de Git es permanente. Un dato personal que se
> suba y se borre después sigue accesible en el historial para siempre, y limpiarlo exige
> reescribirlo. Conviene revisar el archivo antes de publicar, no después.

---

## Regla de datos del módulo de Redes Sociales

Este módulo se construyó bajo una regla explícita: **no se inventa ningún dato.** Cada
cifra visible fue verificada en fuentes públicas y lleva su fecha de verificación a la
vista. Lo que no se puede obtener sin credenciales aparece marcado como
**🔒 Requiere API**, en lugar de rellenarse con estimaciones.

Esto hace que el tablero se vea menos completo de lo que se vería con datos de ejemplo.
Es deliberado: un hueco marcado es información útil; un número inventado es una decisión
tomada sobre algo que no existe.

### Lo que sí está verificado

Cuentas con conteo público confirmado el **3 de agosto de 2026**:

| Cuenta | Red | País | Seguidores | Publicaciones |
|---|---|---|---:|---:|
| @cafhglobal | Instagram | Global | 1.805 | 392 |
| @cafhembalse | Instagram | Argentina | 1.540 | 348 |
| @cafhargentina | Instagram | Argentina | 766 | 227 |
| @cafhportugal | Instagram | Portugal | 369 | 74 |
| @cafh_bolivia | Instagram | Bolivia | 89 | 12 |
| facebrasil.cafh | Facebook | Brasil | 2.026 | — |

Cuentas **confirmadas pero sin métricas accesibles**: `@cafh_org`, `@cafhbrasil`,
`@cafh_chile`, `@cafh.sgo`, `facebook.com/www.cafh.org`, `youtube.com/c/cafhbrasil`.

También están verificados: los **15 países** con presencia oficial según el directorio
de `cafh.org/sedes`, ocho sedes con dirección y contacto, la agenda de actividades
capturada de `cafh.app`, el ecosistema de dominios y los datos institucionales de Cafh
Foundation Inc.

### Lo que NO contiene, y por qué

El tablero **no muestra** alcance, impresiones, tasa de engagement, mejores y peores
publicaciones, comentarios de usuarios, análisis de sentimiento, tasa de
aceptación/rechazo ni origen geográfico de la audiencia.

Ninguno de esos datos es público. Sólo se obtienen con **acceso de administrador** a
cada cuenta, vía Meta Business Suite (Instagram y Facebook) y YouTube Analytics. No es
una limitación de esta herramienta: no están disponibles para nadie que no administre
las cuentas. La pestaña **🔒 Pendientes** los lista uno por uno con la fuente exacta que
los destrabaría.

> Si encuentra alguna versión anterior de este tablero que muestre comentarios de
> usuarios o porcentajes de sentimiento, descártela: esos datos no existen y no fueron
> verificados.

### Datos pendientes de confirmación manual

- **@CafhGlobal (X/Twitter)** — apareció en un rastreo anterior como cuenta sin
  publicaciones desde 2022, pero no se pudo reconfirmar. Verificar antes de decidir si
  se mantiene.
- **Cafh USA and Canada (YouTube)** — canal citado en un rastreo anterior, no
  reconfirmado.
- **TikTok** — ninguna búsqueda devolvió una cuenta oficial de Cafh.

### Sobre las fechas

Los conteos son del **3 de agosto de 2026**. En la varredura del **23 de octubre de
2026** los buscadores no devolvieron los perfiles, de modo que las cifras conservan su
fecha original en lugar de presentarse como actuales. Esa varredura sí aportó datos
institucionales nuevos, visibles en la pestaña **🌐 Ecosistema**.

---

## El histórico: por qué hay que empezar hoy

**La evolución de seguidores no existe retroactivamente.** Nadie puede recuperar hacia
atrás la serie de una cuenta que no administra. Aunque mañana se conecten todas las
APIs, el histórico empezará ese día.

Por eso el módulo incluye el botón **🔄 Registrar medición de hoy**: abre un formulario
con todas las cuentas, muestra el valor anterior de cada una, y permite anotar a mano
las cifras mirando cada perfil. Con dos mediciones ya se dibuja la curva en la pestaña
**📈 Histórico**.

Es trabajo manual, y es lo máximo que puede hacer una página sin credenciales. Una
medición semanal ya permite ver tendencia en un mes. Cada semana sin medir es
información perdida de forma definitiva.

---

## Dónde se guardan los datos

Todo lo que se registra en la aplicación —mediciones, lecciones aprendidas, problemas,
metas, proyectos, registros editados— se guarda en el **localStorage del navegador**
donde se está usando.

Esto tiene tres consecuencias que conviene tener claras:

1. **No se sincroniza.** Si abre el tablero en otro dispositivo o en otro navegador, no
   encontrará lo que registró antes.
2. **No se comparte.** Si varias personas usan el mismo enlace, cada una verá sus
   propios registros.
3. **Se pierde** si se borran los datos del navegador o se usa una ventana privada.

Para consolidar información del equipo, use los botones **⬇ CSV** de las pestañas
Cuentas e Histórico y guarde el resultado en una planilla compartida.

Claves utilizadas: `cafh_*` para los módulos generales y `cafhrs_*` para redes sociales.
El enlace **"Borrar los datos guardados en este navegador"**, en la pantalla de salida,
elimina todas ellas de forma irreversible.

---

## Los módulos

| Módulo | Contenido |
|---|---|
| 📊 Dashboard Global | Visión consolidada |
| 🌐 Oficina Digital | Proyectos de la plataforma |
| 📱 **Redes Sociales** | Gestión y monitoreo — 13 pestañas |
| 🤝 AAEE | Actividades de Extensión |
| 🏛️ Instituciones | Sedes y contratos |
| 🎓 Seminarios | Seminarios de Ordenación |
| 👥 Comunidades | Comunidades Cafh |
| 🗺️ Regional 1 / 2 | América / Resto del mundo |
| 💰 Finanzas | Consolidación |
| ⚙️ Admin | Planeación estratégica |

> **Importante:** los diez módulos distintos de Redes Sociales conservan los **datos de
> ejemplo** del archivo original. No fueron verificados ni modificados. Antes de usarlos
> para decidir algo, confirme qué registros son reales.

### Pestañas del módulo de Redes Sociales

`📊 Panel` · `📱 Cuentas` · `📈 Histórico` · `🌍 Países y sedes` · `📅 Agenda` ·
`🌐 Ecosistema` · `🎯 Metas` · `📌 Proyectos` · `🤖 IA` · `🔒 Pendientes` ·
`✉️ Reportes` · `📚 Lecciones` · `🔎 Problemas`

**Metas** y **Proyectos** arrancan vacíos a propósito: las define el equipo, no la
herramienta.

**IA** reúne los seis hallazgos de la varredura. Cada uno separa explícitamente tres
capas: *Hecho verificado* (lo que la búsqueda encontró), *Lectura* (interpretación) y
*Meta sugerida*. La separación es intencional: el dato y la opinión sobre el dato no
deben confundirse.

### Filtros

Canal, país y período. El selector de período sigue el estándar de mercado: los presets
(30 días, 90 días, 12 meses, este año) **rellenan** los campos Desde y Hasta, que son la
única fuente de verdad. Editar una fecha a mano cambia el selector a "Personalizado"
automáticamente.

---

## Identidad visual

Alineada al **Manual de Identidad Visual de Cafh**.

**Colores primarios**

| Color | Hex | Pantone |
|---|---|---|
| Azul Índigo | `#1A428A` | 7687 C |
| Azul Celeste | `#6FCFEB` | Blue 0821 C |

**Secundarios** — Celestes: Verde Turquesa `#58A3AE`, Gainsboro `#D6DAE2`, Azul Reina
`#5B708D`. Terrosos: Durazno `#FABDA0`, Lavanda `#BE8FA0`, Rojo Arcilla `#D45467`.
Nunca se aplican al logo (manual, pág. 19).

La barra de menú usa `#123063`, un Azul Índigo oscurecido, para que el ítem activo en
Índigo puro resalte sobre el fondo.

**Tipografía:** Nunito Sans (oficial) y Sansita Swashed (apoyo), ambas de Google Fonts.

**Logo:** las tres versiones —blanca, azul marino y celeste— van **embebidas en base64**
dentro del archivo. No se enlazan a `cafh.org`, de modo que se ven sin conexión y
seguirán viéndose aunque el sitio cambie de dirección. Si la imagen fallara, la
aplicación vuelve sola a un respaldo tipográfico en Nunito Sans, que no imita el
logotipo (el manual prohíbe rediseñarlo, pág. 16).

**Desvío conocido:** el manual fija un mínimo de 10 pt para el texto (pág. 22). La
aplicación usa rótulos y leyendas de 10 y 11 px, por debajo de ese mínimo. Fue una
decisión consciente para mantener la densidad de las tablas y el comportamiento
responsivo en celular.

---

## Limitaciones conocidas

**El botón "✨ Nuevo insight" no funciona.** Viene del archivo original y llama a la API
de Anthropic directamente desde el navegador, sin clave de autenticación. Falla en todos
los módulos y muestra un mensaje de error. Para activarlo haría falta un backend que
guarde la clave: nunca puede ir en un HTML público, porque quedaría a la vista de
cualquiera.

**No hay inicio de sesión.** La aplicación corre entera en el navegador, sin servidor ni
usuarios. El botón **🚪 Salir** no cierra ninguna sesión —no existe una que cerrar—:
intenta cerrar la pestaña y muestra una pantalla de salida. Como los navegadores sólo
permiten cerrar pestañas abiertas por script, lo habitual es que aparezca esa pantalla.

**Requiere internet para dos cosas:** las fuentes de Google y la biblioteca de gráficos
Chart.js 4.4.0, ambas desde CDN. Sin conexión la aplicación funciona, pero los gráficos
no se dibujan y la tipografía cae a la del sistema. El logo sí se ve, porque está
embebido.

**La agenda está congelada.** Las actividades fueron leídas de `cafh.app` el 3 de agosto
de 2026 y sus fechas ya pasaron. Se conservan como registro de actividad por país, no
como próximos eventos.

---

## Automatizar el monitoreo diario

El tablero es una interfaz: no ejecuta tareas en segundo plano ni envía correos por sí
solo. Para el monitoreo automático hace falta un orquestador externo. La ruta
recomendada, detallada en la pestaña **✉️ Reportes**:

1. **Acceso a las cuentas.** Un administrador de cada cuenta autoriza el acceso vía Meta
   Business Suite y Google Cloud (YouTube Data + Analytics API).
2. **Snapshot diario.** Un escenario en Make o Zapier con disparador diario consulta
   cada cuenta y escribe una fila por día en Google Sheets o Airtable.
3. **Clasificación de comentarios.** Los comentarios extraídos vía API se pasan por un
   modelo de lenguaje que los clasifica. Recién ahí la tasa de aceptación y rechazo
   tiene base real.
4. **Reporte y envío.** El mismo escenario arma un resumen en HTML y lo envía a la lista
   de destinatarios por Gmail o SMTP.
5. **Alimentar el tablero.** Pasa a leer esa base en lugar de datos fijos, y los campos
   marcados como *Requiere API* se llenan solos.

Las alertas automáticas dependen de tener el histórico en marcha: aparecerán cuando
existan al menos dos mediciones reales para comparar. No se muestran alertas simuladas.

### Destinatarios del reporte

La lista de la pestaña **✉️ Reportes** arranca **vacía**. No hay ningún correo escrito en
el código fuente: cada persona agrega los suyos y quedan guardados en **su** navegador
(clave `cafhrs_emails`), nunca en el repositorio.

Es una decisión de privacidad, no un olvido. Un correo personal dentro de un repositorio
público queda indexado por los buscadores y expuesto a los rastreadores de spam. Los
contactos institucionales que sí aparecen en la aplicación —sedes, teléfonos— provienen
del directorio público de `cafh.org` y ya eran públicos antes.

---

## Para modificar la aplicación

Todo está en un solo archivo. Los puntos de edición más probables:

| Qué cambiar | Dónde |
|---|---|
| Agregar o editar cuentas | `const RS_CUENTAS` |
| Fechas de verificación | `RS_VERIF` y `RS_VARREDURA` |
| Hallazgos de la pestaña IA | `MOCK_INSIGHTS['redes']` |
| Logo | `CAFH_LOGO_BLANCO`, `CAFH_LOGO_MARINO`, `CAFH_LOGO_AZUL` |
| Cuál logo se usa | `const CAFH_LOGO = ...` |
| Paleta de colores | bloque `:root` del CSS |
| Color de la barra de menú | `--sidebar-bg` |
| Lista de destinatarios | `rsEmails()` — arranca vacía a propósito |

Al sustituir el logo por otro archivo, conviértalo a base64
(`base64 -w0 logo.png`) y pegue el resultado precedido de
`data:image/png;base64,`.

---

## Próximos pasos sugeridos

1. **Confirmar el censo de cuentas** con las 15 sedes. La varredura encontró cuentas en
   6 países; las otras 9 pueden tener cuentas no detectadas.
2. **Obtener los accesos de administrador** en Meta y YouTube. Sin eso, ninguna métrica
   de desempeño es obtenible.
3. **Empezar el registro semanal de mediciones**, aunque el resto siga en definición.
4. **Completar el directorio de sedes**: la aplicación tiene la página 1 de 8 de
   `cafh.org/sedes`.
5. **Decidir explícitamente sobre TikTok** y dejarlo asentado.

---

## Historial de versiones

| Versión | Cambio |
|---|---|
| v8 | Lista de destinatarios configurable, sin correos en el código; preparada para GitHub Pages |
| v7 | Metas, Proyectos e IA en Redes Sociales; "Inteligencia" renombrada a "IA" en todos los módulos |
| v6 | Barra de menú en Azul Índigo oscurecido |
| v5 | Paleta alineada al Manual de Identidad Visual |
| v4 | Logos embebidos en base64; favicon |
| v3 | Logo de Cafh (enlazado a cafh.org) |
| v2 | Botón Salir y pantalla de salida |
| v1 | Fusión del módulo de Redes con los 10 módulos de Oficina Digital; corrección del `</div>` que rompía la navegación |

---

*Documentación al 23 de octubre de 2026.*
