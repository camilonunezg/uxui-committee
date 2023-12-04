# Karma - Guía de UX/UI, HTML Semántico y Accesibilidad

## Introducción

El propósito de este documento es contextualizar a nuevos integrantes y establecer guías y lineamientos en cuanto a conceptos y prácticas, además ofrecer recursos a los actuales desarrolladores front que pertenecen a la empresa, a traves de ejemplos y documentación que resulten en un desarrollo de alto nivel.

## Índice

- [UX/UI](#uxui)

  - [Fundamentos](#fundamentos)
  - [Traducción de diseño a código](#traducción-de-diseño-a-código)
  - [Buenas de prácticas de diseño](#buenas-de-prácticas-de-diseño)
  - [Design Systems](#design-systems)
  - [Herramientas de análisis](#herramientas-de-análisis)

- [HTML Semántico](#html-semántico)

  - [Fundamentos](#fundamentos-1)
  - [¿Por qué usar HTML semántico?](#¿por-qué-usar-html-semántico)
  - [Ejemplos + Buenas prácticas](#ejemplos--buenas-prácticas)

- [Accesibilidad y Roles](#accesibilidad-y-roles)
  - [Fundamentos](#fundamentos-2)
  - [Aria](#aria)
  - [Directrices](#directrices)
  - [Errores comunes](#errores-comunes)
  - [Herramientas de medición](#herramientas-de-medición)

## UX/UI

### Fundamentos

### Traducción de diseño a código

Entender la Estructura del Diseño

- Identifica los componentes, secciones y la jerarquía de elementos.

Organización de Componentes

- Cada sección o elemento significativo debería ser un componente ndependiente

Estilos y CSS

- Estilos en línea, estilos en un archivo separado o incluso mediante el uso de preprocesadores
  Mantén la coherencia en la nomenclatura de clases

Flexibilidad Responsiva

- Utiliza clases y estilos que se adapten a diferentes tamaños de pantalla.

Variables y Configuraciones

- Identifica variables clave en Figma (colores, tamaños de fuente, márgenes) y configúralas como variables en tu código

Imágenes y Recursos

- Descarga y almacena imágenes y otros recursos necesarios localmente

Colaboración con Diseñadores

- Mantén una comunicación abierta con los diseñadores

### Buenas de prácticas de diseño

Estándares de marca:
colores, tipografía y elementos que son específicos de la empresa

- Balance(distribucion eficaz de elementos):

  - simetrico: especular. imagenes grandes con bloques de texto
  - asimetrico: Grande en el centro, pequeños en el periferico, se puede dar enfoque
  - fuera de balance: sugiere accion y movimiento, carrusel de informacion

- Composicion:
  regla de los tercios : https://www.photographymad.com/pages/view/rule-of-thirds

- Espaciamiento:
  Diferenciar claramente secciones o bloques

- Punto focal:
  un solo punto focal, zona mas importante que se quiere mostrar

- Color:
  limitar el uso del color
  identificar color primario y secundario (tonos cercanos a esos para hacer enfasis)
  https://color.adobe.com/es/create/color-wheel
  considerar el daltonismo (4.5% de la poblacion)

- Contraste:
  altos contraste permiten resaltar ideas puntuales

### Design Systems

¿Qué son? Los sistemas de diseño son conjuntos de reglas, principios, componentes y directrices para diseñar y desarrollar productos o servicios con consistencia visual, de interacción y experiencia únificada en todos los aspectos de una marca. Incluye elementos como colores, tipografías, iconografías, componentes y pautas de diseño.

> 💡Algunos ejemplos de sistemas de diseño:
>
> - [Primer - Github](https://primer.style/)
> - [Andes UI - Mercado Libre](https://www.behance.net/gallery/72037475/Andes-UI)
> - [Fluent 2 - Microsoft](https://fluent2.microsoft.design/get-started/whatisnew)
> - [Material Design - Google](https://m3.material.io/)

Como desarrolladores fronted, es importante tener los siguientes aspectos en cuenta para la correcta implementación de un sistema de diseño

1. Comprende y familiarizate con el sistema de diseño. revisa si cuenta con componentes disponibles
2. Colaboración con el equipo de diseño: establece una comunicación estrecha para resolver cualquier duda respecto al sistema de diseño con el equipo generador
3. Adaptabilidad: Asegúrate que los componentes y directrices del sistema de diseño sean implementables (viables técnicamente) y adaptables en los dispositivos objetivo de la aplicación o servicio.
4. Accesibiliad: Garantiza que los componentes sean accesibles y utilizables para todos los posibles usuarios. Sigue las pautas definidas posteriormente en este documento.
5. Feedback, feedback, feedback: los comentarios constructivos y tu perspectiva técnica y de negocio pueden beneficiar a todos los involucrados en el proyecto

#### Atomic design

Contexto, implementación e impacto

### Herramientas de análisis

**[CSS Stats](https://cssstats.com/)**: A través de la url esta heramienta te va a permitir hacer un análisis de los colores, tipografías, bordes, sombras y demás elementos de la interfaz de usuario y el sistema de diseño, así podrás revisar aspectos como la correcta implementación del sistema de diseño e inferir c uantitativamente la optimización del css.

## HTML Semántico

### Fundamentos

### ¿Por qué usar HTML semántico?

### Ejemplos + Buenas prácticas

## Accesibilidad y Roles

### Fundamentos

### Aria

### Directrices

### Errores comunes

### Herramientas de medición

## Feedback recibido

- Me falta diseño atómico y como impacta los desarrollos
- Falta los productos o recursos que ustedes aportarían a la comunidad de alternova, ejemplo: charlas, live código, **artículos, o repositorios con ejemplos**

## Fuentes y artículos relacionados

- [Primer - Github design system](https://primer.style/guides)
- [Ejemplo Guía de estilo fronted](https://doc.clickup.com/3063428/d/h/2xfm4-23364/42c77c7d0894c02/2xfm4-40722)

## Recursos adicionales

# Preguntas </Eliminar al finalizar el entregable/>

Documentación proporcionada debe ser agnóstica al framework

Ser agnósticos, luego tener consideraciones relacionadas a cada framework

Profundidad de accesibilidad que daba ser tenida en cuenta (Discapacidades visuales, condiciones mentales.)

¿Como medir la accesibilidad en la web, se regula? ¿Quien? ¿Como afectan estándares? Herramientas que miden accesibilidad, estándares, áreas, etc.

Alcance de UX/UI

Extrapolar de diseño a código y sugerencias de diseño en cuanto a color de botones, etc.

Semántica adecuada para herramientas externas (Lector de pantalla, traducción y corrección de texto, cambio de tema a daltónicos, etc.)

Herramientas que hacen scraping para identificar mejoras en diseños

# Notas </Eliminar al finalizar el entregable/>

- Definir estándares de codificación: Establecer reglas claras para la escritura de código HTML, CSS y JavaScript, incluyendo convenciones de nomenclatura, indentación, comentarios y organización de archivos
  Gestionar la arquitectura del proyecto: Definir la estructura de directorios, la gestión de dependencias, la configuración de herramientas de construcción (build tools) y la integración de sistemas de control de versiones
  Establecer directrices de rendimiento: Incluir prácticas recomendadas para optimizar el rendimiento del frontend, como la compresión de recursos, el uso eficiente de imágenes y la minimización de solicitudes HTTP
  Documentar componentes reutilizables: Describir la implementación y el uso de componentes de interfaz de usuario reutilizables, como botones, formularios, barras de navegación, entre otros
  Considerar la usabilidad y la accesibilidad: Incluir pautas para garantizar la usabilidad y la accesibilidad del frontend, como el uso de etiquetas semánticas, el contraste de colores y la navegación coherente

**Entregables de un comité**

- Informe de investigación: El comité puede producir un informe detallado sobre una tecnología, herramienta, problema o solución específicos que haya investigado. El informe puede incluir recomendaciones, conclusiones y evidencia para respaldar sus hallazgos.
- Mejoras en el proceso de desarrollo: El comité puede proponer mejoras en el proceso de desarrollo de software del equipo, como la implementación de nuevas prácticas o herramientas. Estas mejoras pueden ser documentadas y presentadas al equipo para su implementación.
- Recomendaciones de estándares y regulaciones: El comité puede investigar los estándares y regulaciones relevantes para el desarrollo de software y producir recomendaciones para asegurarse de que el equipo los cumpla. Estas recomendaciones pueden ser documentadas y presentadas al equipo para su implementación.
- Prototipos o pruebas de concepto: El comité puede producir prototipos o pruebas de concepto de nuevas tecnologías o soluciones que haya investigado. Estos prototipos o pruebas de concepto pueden ser presentados al equipo para su evaluación y posible implementación.
- Informes de progreso: El comité puede producir informes de progreso sobre las investigaciones que esté llevando a cabo. Estos informes pueden incluir detalles sobre los hallazgos, los próximos pasos y cualquier problema o desafío que el comité haya encontrado.
