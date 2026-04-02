# Instrucciones para el Agente (Agent Instructions)

Este documento define las reglas de desarrollo y arquitectura base para la web app `trueke`, la cual será construida usando **Vite + React**.

## Stack Tecnológico
1. **Core:** React (con JSX/JS o TS).
2. **Construcción:** Vite.
3. **Estilos:** Vanilla CSS / CSS Modules (A menos que se incorpore TailwindCSS más adelante, priorizar Vanilla CSS semántico).

## Diseño e Interfaz
- **Estética:** Se requiere un diseño moderno de alta calidad ("Premium"). Uso de colores vibrantes, paletas cohesivas (HSL preferible) y tipografía moderna (ej. de Google Fonts).
- **Animaciones:** Incluir micro-interacciones (fades, hovers suaves, expansiones orgánicas) para hacer la UI dinámica.
- **Responsividad:** Al ser el target un entorno principalmente "móvil web", todo diseño debe planearse de "Mobile First" en adelante (priorizar usabilidad táctil, botones con buen padding, etc.).
- **Imágenes:** No usar placeholders aburridos. Utiliza herramientas de IA para generar imágenes demostrativas si un componente necesita mostrar contenido multimedia.

## Flujo de Trabajo
1. **Entender los requerimientos del usuario:** Nunca empezar a escribir a ciegas.
2. **Definir tokens de CSS:** Empezar por el `index.css` definiendo variables globales.
3. **Desarrollo de componentes:** Componentes modulares, pequeños y reutilizables.
4. **Ensamblado:** Organizar las vistas principales.

## Reglas Clave:
- **No añadir librerías enormes** sin consultar (e.g., Redux, Styled Components) a menos que la complejidad del estado lo justifique.
- Todas las etiquetas interactivas HTML deben ser semánticas y accesibles (uso de `button`, `a`, descripciones interactivas, etc.).
- Prohibida la lógica espagueti: Separar componentes visuales de la lógica de negocio cuando un archivo empiece a superar las 200 líneas.
