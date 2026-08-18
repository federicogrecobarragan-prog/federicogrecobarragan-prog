# Federico Greco Barragán

Buenos Aires, Argentina.

Construyo **sistemas multiagente autónomos**, automatización con IA y herramientas para Claude Code y agentes de codificación.

---

## En qué trabajo

**Arneses agénticos de grado productivo.** No prompts sueltos: sistemas con memoria durable, verificación por capas, separación entre quien produce y quien audita, y criterios de cierre que un detector puede comprobar.

Las cuatro piezas que sostienen todo lo que construyo:

| Pieza | Qué resuelve |
|---|---|
| **Memoria persistente** | Que un agente sepa lo que ya sabe. LLM Wiki en markdown interlinkado, con procedencia y decisiones humanas trazables. Grafo de código para relaciones e impacto. |
| **Verificación real** | Que "listo" signifique algo. Verificación en capas —sintaxis, unitaria, integración, E2E, semántica— y la regla que las gobierna: *un criterio sin detector no se cumple, se supone.* |
| **Orquestación** | Equipos de agentes con roles, no un agente haciendo de todo. Maker ≠ checker. Subagentes efímeros para producción y auditoría separadas. |
| **Seguridad y gates** | Reglas vinculantes, secretos fuera del código, confirmación humana previa a toda acción externa o irreversible. |

---

## Público

Repositorios abiertos que salieron de ese trabajo:

| Repo | Qué es |
|---|---|
| [`claude-code-safety-hooks`](https://github.com/federicogrecobarragan-prog/claude-code-safety-hooks) | Hooks de seguridad configurables para Claude Code: backup de archivos críticos, bloqueo de ediciones malformadas, alerta en archivos de alto impacto. Cero dependencias. |
| [`notify-admin-telegram`](https://github.com/federicogrecobarragan-prog/notify-admin-telegram) | Notificador de alertas de infraestructura por Telegram. Sin dependencias, configurable por entorno, con severidad. |
| [`claude-creative-work`](https://github.com/federicogrecobarragan-prog/claude-creative-work) | Guía de Claude for Creative Work: conectores, workflows y batch processing. |

El resto del ecosistema es privado.

---

## Cómo trabajo

- **Especificación antes que código.** Specs verificables, no descripciones.
- **La IA sintetiza datos reales, nunca los inventa.** Si no hay dato, se escribe `«sin dato»` y se registra la fuente faltante.
- **Nada se da por cerrado sin evidencia de ejecución.** Un merge no es un despliegue; un README no prueba producción; git prueba historia, no vigencia.
- **Lo que falla se documenta.** Cada patrón de error recurrente se convierte en una regla compacta y en un detector.

---

## Contacto

[LinkedIn](https://www.linkedin.com/in/federicogrecobarragan) · [CV](https://federicogrecobarragan-prog.github.io/CV_FedericoGrecoBarragan.github.io/)
