Markdown

## Licencia

Este proyecto es de uso académico para el programa de formación Análisis y Desarrollo de Software (ADSO) - SENA. 
 
 Bitácora de Registro y Seguimiento Técnico - ADSO

Este repositorio contiene el sistema de documentación web en HTML5 estructurado para el registro de actividades, control de trazabilidad y normativa técnica del proyecto de desarrollo de software (SENA ADSO).

El objetivo principal es mantener un historial técnico, inmutable y verificable del avance del equipo de desarrollo, aplicando buenas prácticas de maquetación semántica, accesibilidad web y estándares de control de versiones.

---

## Estructura del Proyecto y Vistas Desarrolladas

El proyecto está organizado de forma modular por años, meses y semanas dentro del repositorio. En cada iteración o semana de trabajo se estructuran tres vistas principales:

### 1. Vista Principal de Bitácora 
**Propósito:** Registrar de forma tabular y cronológica los eventos, tareas y avances técnicos ejecutados por el equipo durante las jornadas de desarrollo.
**Componentes:** Tabla técnica estructurada con ID único, marcas de tiempo (*timestamp*), responsabilidad/autoría, objeto técnico con alcance, enlaces a evidencias (commits/PRs), matriz de impedimentos y plan de mitigación.

### 2. Vista de Normas y Guía de Llenado (`reglaprueba.html` / `reglas.html`)
**Propósito:** Definir los lineamientos estándar y el marco normativo para el diligenciamiento correcto de la bitácora.
**Componentes:**
Normas de redacción técnica (Principio de Responsabilidad Única - SRP, neutralidad de lenguaje sin adjetivos subjetivos, inmutabilidad de registros e informes explícitos de impedimentos).
Guía explicativa tipo glosario/tabla sobre la especificación y formato esperado para cada columna de la bitácora.

### 3. Vista de Trazabilidad e Historial (`trazabilidad.html`)
**Propósito:** Documentar los ajustes, correcciones y eventos de soporte o cambios en el repositorio para garantizar auditoría técnica.
**Componentes:** Tabla cronológica de control de versiones interna que enlaza las correcciones a los IDs específicos de la bitácora principal.

---

## Prácticas de Semántica y Accesibilidad Implementadas

En el desarrollo de todas las vistas HTML5 se aplican las siguientes prácticas de accesibilidad (WCAG) y estándares web:

**Maquetación Semántica Estricta:** Uso correcto de etiquetas de estructura global (`<header>`, `<main>`, `<section>`, `<footer>`) para delimitar las zonas de la página y facilitar la lectura por tecnologías de asistencia.
**Jerarquía de Encabezados:** Control ordenado de títulos (`<h1>`, `<h2>`, `<h3>`) sin saltos de nivel para mantener una tabla de contenidos lógica en lectores de pantalla.
**Estructura Accesible de Tablas:**
Uso de etiquetas semánticas `<thead>`, `<tbody>` y `<tfoot>`.
Encabezados de columna definidos con `<th>` y alcance asociativo.
Atributos de formato explícitos para asegurar la correcta renderización visual sin romper el flujo de lectura.
**Diseño Responsivo y Configuración Viewport:** Implementación de la etiqueta `<meta name="viewport" content="width=device-width, initial-scale=1.0">` en el `<head>` de cada documento para garantizar la adaptabilidad en dispositivos móviles y escritorios.
**Navegación e Hipervínculos Descriptivos:** Enlaces de retorno e interacción con textos ancla claros (e.g., `← Volver al Inicio`), evitando frases ambiguas.

