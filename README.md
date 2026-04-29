# z_health_appointment

## Descripción General

Este módulo extiende las vistas de citas de **GNU Health** con personalizaciones locales, sin modificar el módulo original `health_calendar` del proyecto upstream. Sigue el patrón recomendado de crear un módulo separado para sobrescribir vistas, lo que permite actualizar GNU Health sin perder las personalizaciones.

## Funcionalidades

La vista de árbol (lista) de citas muestra las columnas en el siguiente orden personalizado:

| # | Columna | Descripción |
|---|---------|-------------|
| 1 | **Profesional de Salud** | Médico o especialista asignado a la cita |
| 2 | **Paciente** | Nombre del paciente |
| 3 | **Fecha** | Fecha de la cita |
| 4 | **Hora** | Hora de inicio de la cita |
| 5 | **Especialidad** | Especialidad médica correspondiente |
| 6 | **Institución** | Centro o establecimiento de salud |
| 7 | **Estado** | Estado actual de la cita (ej: confirmada, cancelada, atendida) |

## Instalación

Requisitos del entorno:
- **GNU Health** 4.2.0
- **Tryton** 6.0
- **Python** 3.10

Desde el directorio del módulo, instalar con:

```console
pip install .
```

O en **modo editable** (recomendado durante desarrollo, los cambios en el código fuente se reflejan sin reinstalar):

```console
pip install -e .
```

## Uso

1. Instalar el módulo con cualquiera de los comandos anteriores.
2. Ingresar a Tryton como administrador.
3. Ir a **Módulos** y buscar `z_health_appointment`.
4. Activar/actualizar el módulo como cualquier módulo estándar de Tryton.
5. El orden de columnas personalizado se aplicará automáticamente en la vista de lista de citas.

## Licencia

**GPL-3.0-or-later** — Software libre bajo la Licencia Pública General de GNU versión 3 o posterior.
