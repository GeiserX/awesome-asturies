# AGENTS.md — awesome-asturies

## Propósito

Selección de software open source que da **soporte específico al Principado de Asturias** — su gobierno autonómico, ayuntamientos, universidad, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es el Principado de Asturias: el software debe dirigirse específicamente a esta comunidad autónoma o a sus concejos.

## Ámbito

- **78 concejos** del Principado de Asturias están dentro del ámbito (1 provincia, sin subsecciones).
- Principales ciudades: Oviedo/Uviéu (capital), Gijón/Xixón, Avilés, Siero, Langreo, Mieres, Castrillón, San Martín del Rey Aurelio.
- **Universidades**: UniOvi (Universidad de Oviedo).
- **Instituciones**: Principado de Asturias (gobierno autonómico), SADEI (Sociedad Asturiana de Estudios Económicos e Industriales), CTIC (Centro Tecnológico de la Información y la Comunicación).

## Criterios de inclusión

### Incluir

- Software que interactúa con el **Principado de Asturias** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos).
- Herramientas para **ayuntamientos** del Principado de Asturias.
- Software de la **Universidad de Oviedo** (UniOvi) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** del Principado de Asturias (opendata.asturias.es, SADEI).
- Software relacionado con el **medio ambiente asturiano** (Picos de Europa, costa cantábrica, espacios naturales).
- Software de **transporte** asturiano (TUA, ALSA, FEVE/Renfe Cercanías Asturias).
- Herramientas de **cartografía y SIG** específicas del Principado de Asturias.
- Software sobre **cultura y patrimonio** asturiano (prerrománico, llingua asturiana, Camino de Santiago).
- Herramientas de **turismo** de la región.
- Software sobre **deportes** asturianos (Real Sporting, Real Oviedo).
- Proyectos del **sistema sanitario asturiano** (SESPA).
- Software **educativo** específico de la región.
- Herramientas de **industria, energía y minería** asturiana.
- Software de **smart cities** para ciudades asturianas (Gijón smart city).
- Proyectos de la **llingua asturiana** (asturianu/bable) — NLP, diccionarios, herramientas lingüísticas.

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Asturias — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por asturianos que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de la Universidad de Oviedo que podrían ser genéricos — incluir si tienen datos o configuración específica de Asturias.
- Software que cubre Asturias junto con otras regiones — incluir si Asturias es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución asturiana** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-asturies» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades asturianas (AsturiasHacking, Cloud Native Asturias, asturias.js, Elixir Asturias) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- Las búsquedas en GitHub con «asturias» devuelven muchos resultados genéricos (bootcamps, ejercicios de clase). Filtrar con criterio.
- SADEI tiene usuario GitHub `sadeiasturias` con repos de indicadores ODS y datos abiertos — pocos stars pero contenido institucional real.
- La Universidad de Oviedo no tiene organización oficial en GitHub. `medialab-uniovi` tiene repos de IoT/LoRaWAN.
- `Cloud-Native-Asturias` es una comunidad tech activa con directorio de empresas.
- `AsturiasHacking` es la comunidad hacker/maker principal de Asturias, con web activa en 2026.
- `comunidad-tecnologica/Asturias` es un directorio de comunidades tech asturianas.
- `alexcorvis84/LoRa_MakersAsturias` es el repo más popular (18 stars) — red LoRa/TTN de Makers Asturias.
- No se encontraron repos significativos de transporte asturiano (TUA, ALSA).
- No se encontró presencia significativa del CTIC en GitHub.
- Gijón tiene iniciativas de smart city pero sin repos públicos significativos en GitHub.
- La llingua asturiana (asturianu/bable) no tiene herramientas NLP significativas en GitHub — oportunidad de nicho.
- `Naroh091/contratos-menores-principado-de-asturias` es un scraper de transparencia muy relevante (activo 2026).

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*
