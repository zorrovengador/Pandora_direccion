# SkillSpector de NVIDIA

SkillSpector se incluye como **control de calidad y seguridad del paquete**, no como una skill de conversación para Dirección General.

## Uso

Desde la raíz del repositorio:

```bash
uvx --from git+https://github.com/NVIDIA/skillspector.git skillspector scan skills \
  --recursive --no-llm --format json \
  --output /tmp/pandora-direccion-skillspector.json
```

`--no-llm` mantiene el análisis estático y determinista, sin enviar el contenido de las skills a un modelo.

## Gate de admisión

Revisar `max_risk_score`, `risk_assessment`, `issues`, `execution_successful` y cobertura. No instalar una skill con hallazgos críticos, acceso indebido a credenciales, exfiltración, persistencia, acciones destructivas, prompt injection o cobertura incompleta sin revisión humana.

## Resultado de esta versión

- SkillSpector: `v2.9.5`.
- Skills escaneadas: `7`.
- Ejecución: exitosa.
- Riesgo máximo: `0`.
- Hallazgos: `0`.
- Cada skill contiene únicamente `SKILL.md`; no hay scripts ejecutables.

El reporte detallado se conserva fuera del repositorio durante el desarrollo; este resumen evita convertir el repositorio de producto en un depósito de artefactos temporales del entorno local.