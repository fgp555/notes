## Implementación: Módulo de Subida de Documentos para Pacientes

## 1. Descripción General

Se propone desarrollar un nuevo módulo que permita la **subida de imágenes de documentos (frontal y lateral)** por parte de pacientes y administradores. Este módulo se integrará al sistema actual y estará relacionado con las órdenes asociadas a los pacientes.

## 2. Pagina Pública del Paciente

- Formulario de busqueda de pacientes por cedula y tipo de documento.
- Formulario para pueda subir imágenes de sus documentos frontal y lateral.
- Compresión de imágenes para optimizar peso, velocidad y espacio en hosting.
- Permitir capturar imagen con la cámara directa desde celular.
- Permitir seleccionar archivos desde la galería del ordenador.

## 3. Requisitos Funcionales Dashboard

- Funcionalidad en el dashboard para que operadores o administradores suban documentos.
- Visualización de imágenes cargadas en el dashboard de pacientes.
- Reemplazo o eliminación de imágenes desde el dashboard.
- Asociación de documentos de pacientes a órdenes específicas.
- Exportación a pdf de ordenes con las imagenes de los documentos del paciente.
- Consulta de orden con el (los) documentos asociados.
- Listados por rangos de fechas.

## 6. Extras opcionales (sujetos a disponibilidad de tiempo)

- Seguridad mediante token temporal en el flujo público.
- Opción de CAPTCHA para proteger el formulario público.
- Carga de documentos mediante la app de whatsapp

## 7. Plan de Desarrollo

| Fase                    | Duración estimada     |
| ----------------------- | --------------------- |
| Análisis técnico        | 1-2 día               |
| Diseño sistema/interfaz | 1-2 días              |
| Desarrollo              | 8-10 días             |
| Pruebas internas        | Durante todo el ciclo |
| Fase de estabilización  | 5 días hábiles        |

---

## Fase de estabilización / Pruebas en producción

**Nota:** La etapa de **pruebas en producción** será realizada por el **Product Owner de Transpaservic** y tendrá una duración máxima de **5 días hábiles**. Durante este periodo se podrán:

- Validar el comportamiento real del sistema con usuarios y datos reales.
- Pruebas de usabilidad y experiencia de usuario: Se evalúa si los usuarios (pacientes o admins) entienden el flujo y si algo puede mejorarse.
- Detectar y corregir errores menores no identificados durante el desarrollo.
- Ajustes visuales, de validación o de comportamiento inesperado no detectado en desarrollo.
- Ajustar textos, validaciones o flujos según retroalimentación directa del uso real.

Esta etapa tiene como objetivo estabilizar el módulo en entorno real antes de considerarlo cerrado.

En caso de que este periodo de pruebas sea superado, el tiempo adicional será considerado como **servicio adicional** y podrá implicar **costos extra**, los cuales serán informados y aprobados previamente.

## 8. Consideraciones

- El presente desarrollo contempla exclusivamente las funcionalidades descritas en este documento.
- Cualquier funcionalidad nueva solicitada fuera de alcance será presupuestada y facturada adicionalmente.

## 9. Despliegue y Entorno

- Despliegue continuo diario en entorno de desarrollo.
- Coordinación con QA (David) y PO (Transpaservic) para validación continua.
- Despliegue a producción bajo calendario coordinado.

---
