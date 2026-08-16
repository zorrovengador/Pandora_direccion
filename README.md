# Pandora_direccion

Paquete de configuración, skills y onboarding para una instancia de Hermes orientada a Dirección General.

## Objetivo

Entregar un Pandora ejecutivo que convierta correo, calendario, documentos, reuniones y contexto autorizado en **briefings, decisiones y seguimiento verificable**.

Este repositorio contiene materiales portables y seguros. No contiene sesiones Hermes, credenciales, tokens, QR, datos personales del Director General ni archivos `.env` reales.

## Skills incluidas

| Skill | Función |
|---|---|
| `dg-jefe-de-gabinete` | Prioridades, asuntos abiertos, riesgos y siguientes acciones |
| `dg-briefing-y-decisiones` | Briefings ejecutivos y análisis de alternativas |
| `dg-agenda-y-reuniones` | Preparación de juntas, minuta, acuerdos y seguimiento |
| `dg-correo-y-comunicacion` | Resúmenes de correo y borradores sin envío implícito |
| `dg-documentos-ejecutivos` | Síntesis y producción de documentos para Dirección |
| `dg-memoria-y-contexto` | Memoria mínima, portable y con procedencia |
| `dg-seguridad-y-aprobaciones` | Mínimo privilegio, aislamiento, aprobación y control de acciones |

## Dependencias externas

Las skills operativas requieren que la instancia tenga, según el alcance autorizado: Google Calendar, Gmail y Drive; herramientas de reuniones/transcripciones; proveedor de modelo; memoria local aislada; y canal definido.

La primera configuración debe iniciar en **solo lectura**. Envíos, cambios, publicaciones, permisos y eliminaciones requieren autorización explícita.

## Instalación conceptual

1. Crear un perfil Hermes independiente para el Director General.
2. Copiar `skills/` al directorio de skills del perfil.
3. Adaptar `config/permissions.example.yaml` sin agregar secretos al repositorio.
4. Completar `onboarding/`.
5. Conectar únicamente las fuentes autorizadas.
6. Ejecutar las pruebas del guion inicial.

El paquete es agnóstico de hosting: VPS dedicado/aislado o Hermes Cloud. La decisión debe registrarse con privacidad, exportación, soporte y responsabilidades operativas.