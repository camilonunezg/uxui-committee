# Karma - Guía de UX/UI, HTML Semántico y Accesibilidad

## Introducción

El propósito de este documento es contextualizar a nuevos integrantes y establecer guías y lineamientos en cuanto a conceptos y prácticas referentes a UX/UI, HTML Semántico y Accesibilidad. Además ofrecer recursos a los actuales desarrolladores front  y  demás intersados, a traves de ejemplos y documentación que resulten en un desarrollo de alto nivel.

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

1. **Entender la Estructura del Diseño:**

   Analiza y comprende la estructura general del diseño en Figma. Identifica los componentes, secciones y la jerarquía de elementos.

2. **Organización de Componentes:**

   Divide el diseño en componentes lógicos y reutilizables. Cada sección o elemento significativo debería ser un componente independiente

3. **Estilos y CSS:**

   Utiliza estilos modulares, estilos en línea o estilos en un archivo separado. Mantén la coherencia en la nomenclatura de clases.

4. **Flexibilidad Responsiva:**

   Utiliza clases y estilos que se adapten a diferentes tamaños de pantalla.

5. **Variables y Configuraciones:**

   Identifica variables clave en Figma (colores, tamaños de fuente, márgenes) y configúralas como variables en tu código

6. **Imágenes y Recursos:**

   Descarga y almacena imágenes y otros recursos necesarios localmente en tu proyecto Vue. Utiliza las rutas relativas adecuadas.Implementa la lógica de manejo de datos en tus componentes.

7. **Manejo de Datos Dinámicos:**
   Si el diseño implica datos dinámicos, asegúrate de entender cómo se deben cargar y mostrar esos datos.

8. **Pruebas y Verificación:**
   Verifica que la funcionalidad y la apariencia en Vue coincidan con el diseño en Figma. Ajusta cualquier discrepancia y realiza pruebas en diferentes navegadores.

9. **Colaboración con Diseñadores:**

   Mantén una comunicación abierta con los diseñadores. Si hay elementos que no están claros o que podrían requerir ajustes para la implementación, coordina con el equipo de diseño.

10. **Versionamiento y Control de Código:**

    Utiliza un sistema de control de versiones (como Git) para rastrear los cambios en tu código. Esto es especialmente útil cuando trabajas en colaboración con otros desarrolladores o cuando necesitas retroceder a versiones anteriores.

11. **Documentación:**

    Documenta tu código. Incluye comentarios explicativos, especialmente para lógica compleja o soluciones no convencionales.

La traducción de un diseño a código es un proceso iterativo, y es posible que necesites hacer ajustes a medida que avanzas. La colaboración continua entre diseñadores y desarrolladores es clave para lograr un producto final que se alinee tanto con el diseño como con las expectativas de la funcionalidad.

### Buenas de prácticas de diseño

Las mejores prácticas de diseño web son un conjunto de pautas y enfoques que se consideran efectivos y beneficiosos para crear sitios web atractivos, funcionales y accesibles.

1.  **Usabilidad:**

    Las mejores prácticas se centran en la facilidad de uso y la experiencia del usuario. Los sitios web deben ser intuitivos y permitir a los usuarios navegar y encontrar información de manera eficiente.

2.  **Accesibilidad:**

    Un diseño web accesible garantiza que todas las personas, independientemente de sus habilidades o discapacidades, puedan acceder y utilizar el sitio. Esto incluye la atención a detalles como la navegación por teclado, el contraste de colores y el uso de etiquetas descriptivas.

3.  **Velocidad de Carga:**

    La optimización del rendimiento es fundamental. Los sitios web deben cargar rápidamente para retener la atención del usuario y mejorar el posicionamiento en los motores de búsqueda.

4.  **Diseño Intuitivo:**

    La disposición de elementos y la navegación deben seguir patrones intuitivos. Los usuarios deben comprender fácilmente cómo interactuar con el sitio y encontrar lo que buscan.

5.  **Consistencia:**

    La consistencia en el diseño, la tipografía, los colores y la navegación crea una experiencia coherente y profesional. Los elementos clave deben mantenerse uniformes en todas las páginas.

6.  **Contenido Relevante y de Calidad:**

    La información presentada en el sitio debe ser relevante, fácil de entender y valiosa para los usuarios. Un buen equilibrio entre texto, imágenes y otros medios contribuye a la efectividad del contenido.

7.  **Seguridad:**

    La seguridad es esencial para la confianza del usuario. La implementación de protocolos de seguridad, especialmente en sitios que manejan información confidencial, es una mejor práctica.

8.  **SEO (Optimización para Motores de Búsqueda):**
    La optimización del contenido y la estructura del sitio para los motores de búsqueda ayuda a mejorar la visibilidad en los resultados de búsqueda, aumentando la probabilidad de que los usuarios encuentren el sitio.

9.  **Pruebas y Mejora Continua:**
    La implementación de análisis y pruebas de usabilidad permite identificar áreas de mejora.

10. **Diseño Responsivo:**
    Un diseño web responsivo garantiza que el contenido se vea bien y sea funcional en diferentes dispositivos.

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

Como desarrolladores frontend, es importante tener los siguientes aspectos en cuenta para la correcta implementación de un sistema de diseño

1. Comprende y familiarizate con el sistema de diseño. revisa si cuenta con componentes disponibles
2. Colaboración con el equipo de diseño: establece una comunicación estrecha para resolver cualquier duda respecto al sistema de diseño con el equipo generador
3. Adaptabilidad: Asegúrate que los componentes y directrices del sistema de diseño sean implementables (viables técnicamente) y adaptables en los dispositivos objetivo de la aplicación o servicio.
4. Accesibiliad: Garantiza que los componentes sean accesibles y utilizables para todos los posibles usuarios. Sigue las pautas definidas posteriormente en este documento.
5. Feedback, feedback, feedback: los comentarios constructivos y tu perspectiva técnica y de negocio pueden beneficiar a todos los involucrados en el proyecto

---

#### Atomic design

Contexto, implementación e impacto

**Contexto**: El diseño atómico es una metodología para diseñar sistemas de interfaz de usuario de manera modular y jerárquica. Propuesto como una forma de abordar los desafíos de diseño en la creación de interfaces de usuario coherentes y escalables.

La idea principal detrás del diseño atómico es conceptualizar una interfaz de usuario como un sistema compuesto por componentes más pequeños y más simples, que se organizan en niveles jerárquicos.

![atomic design](/assets/images/atomic_design.png "Atomic Design")

---

**Implementación**:

A continuación, se presenta un ejemplo de cómo implementar el diseño atómico en una aplicación hecha con VueJs, sin embargo, los principios per se son agnósticos al framework de preferencia.

Comencemos a construir nuestro átomo, un botón:

Definiremos qué propiedades tiene un botón y el grado de extensibilidad y modificación que éste tendrá:

| Nombre 	| Predeterminado 	| Descripción 	|
|---	|---	|---	|
| label 	|  	| Texto principal 	|
| type 	|  	| 'default'\|'primary'\|'secondary'\|'danger' Define el estilo visual del botón 	|
| size 	| 'md' 	| 'sm' \| 'md' \| 'lg' Tamaño del botón 	|
| isInactive 	| false 	| **boolean** Si el botón se encuentra deshabilitado 	|

Observamos entonces que a través de props es posible modificar su texto principal, estilos como su estado de habilitado, el tipo y tamaño.

```Javascript
/** Definitions * */
type ButtonType = 'default' | 'primary' | 'secondary' | 'danger'
type ButtonSize = 'sm' | 'md' | 'lg'
```

Trasladamos lo definido en la tabla como requisitos,  al script del componente:

```Javascript
/** AtomButton.vue script section * */
<script setup lang="ts">
import { ButtonType, ButtonSize } from './utils';

interface Props {
  label: string,
  type: ButtonType,
  size?: ButtonSize,
  isInactive?: boolean,
}

withDefaults(defineProps<Props>(), {
  size: 'md',
  isInactive: false,
})
</script>
```
En cuanto al template, adicional a la implementación de las props  antes vistas, existen dos slots (análogo hasta cierto punto a `children` en ReactJs ) para añadir opcionalmente los íconos leading y trailing

```Javascript
/** AtomButton.vue template section * */
<template>
  <button
    :disabled="isInactive"
    :class="[type, size]"
  >
  <slot name="leadingIcon"/>
  {{ label }}
  <slot name="trailingIcon"/>
  </button>
</template>
```

Definimos los estilos de acuerdo con props y estados:

```Javascript

<style scoped>
  /* AtomButton.vue style section */
button {
  all: unset;
  padding: 0.5rem 1rem;
  border-radius: 8px;
  color: #fafafa;
  transition: opacity 200ms;
}
button:hover {
opacity: 0.75;
}
button.default {
  background-color: #64748b;
}
button.primary {
  background-color: #0ea5e9;
}
button.secondary {
  background-color: #34d399;
}
button.danger {
  background-color: #f43f5e;
}
button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}
button.sm {
  font-size: 0.9rem;
  padding: 0.25rem 0.5rem;
}
button.md {
  font-size: 1rem;
  padding: 0.5rem 1rem;
}
button.lg {
  font-size: 1.1rem;
  padding: 0.5rem 1rem;
}
</style>
```

![atomic button](/assets/images/atom_button.png "Atomic Button")
*Atomic Button con variaciones y múltiples configuraciones.*

A continuación, podrás encontrar el ejemplo completo de éste desarrollo en el playground de Vue

>[Ejemplo completo - Vue Playground - Atomic Button](https://play.vuejs.org/#eNq1WO9u2zYQfxVCAea08H87/1Q3Q9N0QIaiK5pgX6Z9oCVKYSORAkklzjJ/3MdtGPYAfZABe6Y+wo6kJEtZHCu2g6KJdLw7/u53xxMvd86bNO1eZ8RxnYn0BU0VkkRlKYoxi157jpKec+wxmqRcKPRG8eQkU4ozFAqeoFa3txBpNy2PeSwgIWXko+CpnNx5DIGvKYm/dZFUgrLIY/Pj3Rcem/TshuAeXhRJ0hgrAm8ITSTxFYVd/BhLCTBuBE5TIgwWrQAqAb02uublcnh8cZuSSQ8eSiEGaJ2phWsggKNTEuIsVp6DFOiDAMDmgt7xZCrM/0c9fBQ0weJ24SEtBQ09nBOfs6DmA+ItRQ29nEKCNCNlIMX7fftJz1K1hLdTKvE03ow6l8oOZRhydq0XlMjIVgjdyO8KmjfyvZT8Zl5XpOSc/kKQTDZKiQQfOuJkK4lYw9sK+tfwuJT0x3w1oTqOtkF1HG2T6qd4a0b1UzyuovpBXyuofk9wAO0f/UhlhmPZhHKfJFMi0ODgAaJKW7AuPh5oJ7abnEH0FQVQMU6Pv375+7dJzz5X7Hu1r48VVRA14+wDVyjkAiX6xN/jbU2wf/3x9cuf/zwX4Pf0qgK1UjHrov0d0P67MdoVZXQhMI2fVEff4WsuqKrEuqKIVL7FslC/2Tk6GI1ePVdePpGEXzcuotVgB/1+f//Z0L7lTFFmPnNNK6kJ5MG4vznkFaV0wtVl8zIaDEfjwbYaEYS4v9cswDUpPBwOD9ZhsM5cAQAu6/ZKDrKaC3iV6jbWj938lo7MpT+gEnRuXRQJGrzSEv3QKUw7Po+zhEkXCZISrHbHbTQIxYuFZoRTFw366WwhwpniHcFvwCqhLMGzXajtdNZGekGbzs1YkeNx2jC+AD8hjbqfJWcw4xhknuPzJKUxET+kOiQYcVyLWa/hOOY33xuZvr21C7l/SfyrB+Sf5UzL9DedSCL0wS3XFBYRgSuCXn53/oHM4LlcTHiQxaD9yOInIoEljdGqnWQsANgVPYP2zExnUA0X8t1MESaLoMz1EzTnRt9zYEJ7+0joC7ij7sjYAaPAYn3GazYq3iFroceydv5sLlvzcnSEwGLZgqyBEVNEhNgnyIyNFpIp3WJqNBHoo+dWHWuhvpLAcLnYwkipPMuv4bA25RzOI4MFiMhjN1Rd5vc5uVudVs1PGE7bFoD27KJWErTuuXRRCC1DbzRfMcjaQ2UJduFI6FErALIWvjwnXy1m3Z90lG2z+c92MZ+JY7hgMJyY+9eiu3hOz6zf3VnC0BxivKde7RaF/qRXHvgHDzSCo5OSACS9l5XBX1cApMQo5EP6y57H8l5paIOadFHGoDjMyU1xoLG6qN/dEyRBA/hhFqZcBER0BISSwYk+zE86NAYuXLQTYv3PiAA/FLXezEU8xT5Vt2jY7yfSHnm7uXsJX03TfHIVvePBXlWlm1/aLc4p9q8iweFM6WZk9twfH4wPpzWTvM8vNekTvEeOaiblB3Cp0WgcjI7qRvYrv9QiHI/CPVKLtygna1MJWscMPGZCalPGVce0CaLbcAVlYg1D+IB3bKn3u0dFcipZG5q02ezVPCT51hUPZXKXZH1hHEf/N+42MK/1d9NCukpCT9KnptIa0GvUyrPdQr+iVp5G81zmx7xZ4uEvVxUPplOBB5kYFegA+lccmb9vkZntcBrnvV5Ua0IA1pn/BzA4UvM=)

Éste es sólo él desarrollo de un átomo sencillo que puede ser utilizado por ejemplo con otro átomo input, para formar una molécula.

---

**Impacto**:

El imparto del diseño átomico se presenta en diferentes niveles: a nivdel de desarrollo, de proyeto y de organización

- A nivel de desarrollador:
    - Reutilización de componentes: Puede aprovechar esto incluso de proyectos preexistentes, acelerando la velocidad a la que se le entrega valor al proyecto
    - Desarrollo incremental: Facilita la resolución progresiva de problemas y reduce el riesgo de errores
    - Facilidad de mantenimiento: ya que obliga la modularidad de componentes y esto a su vez facilita la implementación de pruebas unitarias efectivas.
    - Consistencia en la UI: al crear interfaces basadas en átomos, habrá siempre una coherencia visual, relacionada también a los sistemas de diseño estudiados previamente.
-  A nivel de proyecto:
    - Adaptabilidad al cambio: los requisitos y el diseño se modifican constantemente, estos cambios de pueden aplicar de manera fácil y granular en el diseño atómico.
    - Escalabilidad: facilitando la gestión de errores y el mantenimiento de proyectos grandes
- A nivel organizacional:
   - Colaboracíon efectiva: al existir un lenguaje común entre el equipo de desarrollo y el equipo de diseño, mejorando la compresión mutua
   - Gestión de recursos: La reutilización de componentes y la gestión de un sistema de diseño optimiza el tiempo necesario para diseñar y desarrollar

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

## Feedback recibido </Eliminar al finalizar el entregable/>

1ra entrega
- Me falta diseño atómico y como impacta los desarrollos
- Falta los productos o recursos que ustedes aportarían a la comunidad de alternova, ejemplo: charlas, live código, **artículos, o repositorios con ejemplos**

## ¿Cómo contribuir a esta guía?
Tanto el desarrollo de software como el diseño, son campos en constante evolución, es por esto que todos los lectores de esta guía son bienvenidos a aportar con comentarios, críticas constructivas, artículos y demás elementos que ayuden a esta guía a conservar su valor a los demás colaboradores. 

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
