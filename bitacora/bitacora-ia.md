# Bitácora de IA

## Trabajo Práctico N.º 1 – Proceso de Diseño de Interfaz de Usuario

**Materia:** Diseño de Interfaces de Usuario

**Proyecto:** Plataforma de Juegos Online – Temática Batman

**Herramienta de IA utilizada:** ChatGPT (GPT-5.5)

---

# Objetivo del uso de IA

La inteligencia artificial fue utilizada como herramienta de validación durante el proceso de diseño de la interfaz. Su función fue analizar los componentes desarrollados, verificar el cumplimiento de principios de UX/UI, evaluar la organización del Design System y proponer mejoras fundamentadas.

La IA no fue utilizada para generar automáticamente el Design System ni las interfaces, respetando la consigna del trabajo práctico.

---

# Iteración 1 – Desarrollo inicial del Design System

## Estado inicial

Se desarrolló una primera versión del Design System incluyendo los elementos solicitados por la consigna:

* Paleta de colores.
* Tipografía.
* Cards de juegos.
* Carruseles.
* Botones.
* Navbar.
* Iconografía.
* Modal para compartir contenido.
* Logo.

El objetivo fue construir un sistema reutilizable para el desarrollo posterior de las pantallas.

---

## Validación realizada por IA

Durante la primera revisión se detectaron oportunidades de mejora.

### Organización del Design System

Los componentes estaban distribuidos sobre el lienzo sin seguir una estructura clara.

Esto dificultaba comprender rápidamente la función de cada elemento y su reutilización.

**Motivo del cambio**

Un Design System correctamente organizado facilita el mantenimiento del proyecto y la reutilización de componentes.

---

### Sistema tipográfico

Inicialmente únicamente se indicaban las familias tipográficas:

* Chakra Petch
* Roboto

No existía documentación sobre tamaños, pesos ni jerarquías.

**Motivo del cambio**

Una escala tipográfica documentada mantiene consistencia visual entre todas las pantallas y facilita el uso correcto de los estilos de texto.

---

### Atomic Design

Los componentes estaban desarrollados, pero todavía no estaban clasificados según Atomic Design.

**Motivo del cambio**

La metodología Atomic Design permite organizar los componentes según su nivel de complejidad, favoreciendo su reutilización.

---

## Cambios implementados

### Mejora de la tipografía

Se creó una tabla tipográfica donde se documentaron:

* Familia tipográfica.
* Peso.
* Tamaño.
* Altura de línea.
* Espaciado.

También se definieron los distintos estilos para títulos, botones, carruseles y cards.

---

### Reorganización del Design System

Se reorganizaron visualmente todos los componentes para que el archivo fuera más claro y sencillo de navegar.

---

### Implementación de Atomic Design

Los componentes fueron clasificados según la metodología Atomic Design.

**Átomos**

* Paleta de colores.
* Tipografía.
* Logo.
* Iconografía.
* Botones.

**Moléculas**

* Search Bar.
* Card Game.

**Organismos**

* Navbar.
* Carrusel.
* Fat Footer.
* Modal para compartir.
* Ficha del Peg Solitaire.

---

## Resultado

El Design System obtuvo una estructura mucho más organizada, facilitando la reutilización de componentes durante el desarrollo del resto del proyecto.

---

# Iteración 2 – Desarrollo de las pantallas

Con el Design System finalizado se comenzó el desarrollo de las interfaces solicitadas por la consigna.

---

## Pantalla Login

Se desarrolló la pantalla de registro e inicio de sesión.

Incluye:

* Logo.
* Formulario destacado.
* Registro.
* Inicio de sesión.
* Google.
* Facebook.
* Recaptcha no funcional.

Toda la interfaz reutiliza la identidad visual definida previamente.

---

## Pantalla Home

Se desarrolló la página principal de la plataforma.

Se implementaron:

* Header.
* Logo.
* Barra de búsqueda.
* Menú hamburguesa.
* Carruseles de juegos.
* Recomendaciones personalizadas.
* Fat Footer.

Todos los carruseles reutilizan el componente Card Game definido en el Design System.

---

## Página del juego

Se desarrolló la pantalla correspondiente al juego **Peg Solitaire** con temática Batman.

Incluye:

* Área de ejecución del juego.
* Breadcrumbs.
* Panel de ayuda.
* Información del juego.
* Galería.
* Enlaces útiles.
* Comunidad.
* Formulario de comentarios.
* Compartir por redes sociales.
* Botón para regresar al Home.

---

## Resultado

Las tres pantallas mantienen una identidad visual consistente gracias a la reutilización de los componentes desarrollados previamente.

---

# Iteración 3 – Organización del archivo de Figma

Durante el desarrollo surgió una limitación del plan gratuito de Figma, que únicamente permitía trabajar con tres páginas dentro del archivo.

Para cumplir con la consigna se reorganizó el proyecto de la siguiente manera:

**Página 1**

Design System.

**Página 2**

Login.

**Página 3**

Home y Game Page.

Dentro de la tercera página se utilizaron **Frames independientes** para representar ambas interfaces.

Esta solución permitió mantener correctamente organizado el proyecto sin modificar el contenido solicitado por el trabajo práctico.

---

# Iteración 4 – Implementación del flujo del prototipo

Una vez finalizadas las interfaces se comenzó el desarrollo del prototipo interactivo.

---

## Estado inicial

Las pantallas eran completamente estáticas.

No existía navegación entre ellas.

---

## Validación realizada por IA

Se verificó el flujo solicitado por la consigna.

También se recomendó configurar correctamente el punto inicial del prototipo y conectar todas las pantallas mediante interacciones.

---

## Cambios implementados

Se agregaron las interacciones necesarias para permitir la navegación entre los distintos frames.

Se configuró el siguiente recorrido:

* Login → Home.
* Home → Game Page.
* Game Page → Home.

Además se configuró la pantalla de Login como punto de inicio del prototipo.

---

## Resultado

El proyecto dejó de ser una colección de pantallas estáticas y pasó a comportarse como un prototipo navegable.

---

# Iteración 5 – Organización de Templates y componentes

Durante una nueva revisión del archivo se detectó que una de las pantallas completas ("Desktop") había sido incorporada dentro del Design System como si fuera un componente.

La IA indicó que una pantalla completa no corresponde a un componente reutilizable, por lo que se reorganizó la estructura del proyecto.

---

## Validación realizada por IA

Se verificó la correcta aplicación de Atomic Design.

Se recomendó separar claramente los componentes reutilizables de las pantallas finales.

---

## Cambios implementados

Se reorganizaron los elementos del proyecto utilizando la siguiente estructura:

### Átomos

* Paleta de Colores.
* Tipografía.
* Logo.
* Iconos.
* Botones.

### Moléculas

* Search Bar.
* Card Game.

### Organismos

* Navbar.
* Carrusel.
* Fat Footer.
* Menú Hamburguesa.
* Ficha Peg Solitaire.

### Templates

Se crearon los layouts principales del sitio:

* **Home Desktop**.
* **Home Open Menu Desktop** (estado del menú hamburguesa desplegado).
* **Game Page Desktop**.

Estos templates representan la estructura general de las páginas reutilizando los organismos desarrollados previamente.

### Pages

Las páginas finales del proyecto quedaron organizadas como:

* Login.
* Home.
* Game Page.

---

## Resultado

La organización del archivo pasó a seguir correctamente la metodología Atomic Design, diferenciando entre componentes reutilizables, templates y páginas finales.

---

# Validaciones realizadas por IA

Durante todo el proceso de desarrollo la IA permitió validar los siguientes aspectos:

* Organización del Design System.
* Correcta aplicación de Atomic Design.
* Escala tipográfica.
* Consistencia de la paleta de colores.
* Reutilización de componentes.
* Organización visual del archivo de Figma.
* Implementación del patrón Fat Footer.
* Uso del menú hamburguesa.
* Implementación del flujo del prototipo.
* Separación entre componentes reutilizables, templates y páginas finales.

Todas las observaciones fueron incorporadas progresivamente durante el desarrollo del proyecto.

---

# Conclusión

La utilización de inteligencia artificial permitió validar continuamente el desarrollo del proyecto, detectando oportunidades de mejora antes de finalizar el prototipo.

Las principales mejoras implementadas fueron:

* Organización del Design System.
* Documentación de la tipografía.
* Aplicación correcta de Atomic Design.
* Reutilización de componentes.
* Desarrollo de un flujo de navegación interactivo.
* Organización del archivo de Figma mediante Templates y Pages.

Como resultado, el proyecto evolucionó desde un conjunto inicial de componentes hacia un sistema de diseño estructurado, reutilizable y consistente, cumpliendo los requisitos establecidos en la consigna y facilitando tanto la presentación como la defensa del trabajo práctico.

