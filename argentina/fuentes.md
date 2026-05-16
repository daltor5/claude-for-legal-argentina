# Fuentes normativas argentinas · Conectores MCP

Repositorios de la comunidad que conectan claude-for-legal directamente con las fuentes oficiales argentinas. Reemplazan los conectores originales del repositorio (Westlaw, CourtListener, Everlaw) para práctica local.

No son necesarios para empezar. Los plugins funcionan con el perfil de práctica (`CLAUDE.md`) como única configuración. Los conectores son la segunda capa: permiten que el sistema consulte fuentes primarias automáticamente sin que el abogado tenga que pegar el texto de la norma en la sesión.

---

## Conectores disponibles

### 1. Ansvar-Systems/argentine-law-mcp

**Repositorio:** https://github.com/Ansvar-Systems/argentine-law-mcp  
**Fuentes:** InfoLEG · SAIJ  
**Función:** Devuelve el texto literal de normas nacionales argentinas sin pasar por ningún modelo de lenguaje. Ideal para verificación de vigencia y texto oficial de artículos específicos.

Casos de uso:
- Verificar texto actual de un artículo del CCCN o la LCT
- Confirmar si una norma fue modificada o derogada
- Obtener el texto de una ley especial sin buscarlo manualmente

### 2. Psflores/Legal-MCP-Server-

**Repositorio:** https://github.com/Psflores/Legal-MCP-Server-  
**Fuentes:** Poder Judicial de la Nación · Justicia CABA  
**Función:** Búsqueda de jurisprudencia de CABA y fueros nacionales.

Casos de uso:
- Buscar fallos por doctrina antes de citar en un escrito
- Verificar criterio de la sala en una materia específica
- Rastrear evolución jurisprudencial sobre un instituto

### 3. guidobonomini/argentina-law-mcp-server

**Repositorio:** https://github.com/guidobonomini/argentina-law-mcp-server  
**Función:** Análisis semántico de documentos legales, glosario judicial argentino, módulos de detección de riesgos según praxis local.

Casos de uso:
- Análisis de contratos con terminología jurídica argentina nativa
- Detección de riesgos calibrada para jurisprudencia local
- Consulta de glosario cuando el sistema genera términos de common law

### 4. datos-justicia-argentina/Tesauro-Saij-de-Derecho-Argentino

**Repositorio:** https://github.com/datos-justicia-argentina/Tesauro-Saij-de-Derecho-Argentino  
**Fuente:** SAIJ  
**Función:** Vocabulario controlado para búsqueda jurídica. Mapea sinónimos, términos preferidos y jerarquías conceptuales del derecho argentino.

Casos de uso:
- Mejorar la precisión de búsquedas jurisprudenciales
- Evitar que el sistema use términos de common law cuando existe equivalente argentino
- Consistencia terminológica en documentos largos

---

## Fuentes primarias oficiales (sin conector MCP)

Estas fuentes no tienen conector MCP disponible actualmente. Se acceden directamente por el abogado para verificación manual.

| Fuente | URL | Uso |
|---|---|---|
| InfoLEG | infoleg.gob.ar | Texto oficial de normas nacionales |
| SAIJ | saij.gob.ar | Jurisprudencia, doctrina, legislación provincial |
| PJN | pjn.gov.ar | Acordadas, jurisprudencia federal |
| SCBA | scba.gov.ar | Jurisprudencia PBA |
| AAIP | argentina.gob.ar/aaip | Disposiciones de datos personales |
| IGJ | igj.gob.ar | Resoluciones societarias CABA |
| CNV | cnv.gov.ar | Normas y resoluciones mercado de capitales |

---

## Instalación de conectores MCP

Los conectores se instalan en Claude Cowork (aplicación de escritorio). El proceso general:

1. Abrir Claude Cowork
2. Ir a Configuración > MCP Servers
3. Agregar el repositorio del conector
4. Verificar que el conector aparezca activo antes de usarlo

Para instrucciones específicas de cada conector, consultar el README del repositorio correspondiente.

---

*Última actualización: mayo 2026*
