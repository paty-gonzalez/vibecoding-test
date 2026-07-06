Pájaros Furiosos 🐦 - JS Nativo & Canvas HTML5

Un clon ligero y responsivo del clásico juego de físicas "Angry Birds", construido completamente desde cero utilizando JavaScript Vanilla y la API de HTML5 Canvas. Este proyecto demuestra cómo implementar un motor de físicas personalizado sin depender de librerías externas pesadas (como Matter.js o Box2D).

🚀 Características Principales

Motor de Físicas Personalizado: Implementación propia de gravedad, fricción, vectores de fuerza, rebotes y detección de colisiones (AABB híbrido y circular).

Zero Assets (Sin imágenes externas): Todo el renderizado de personajes (pájaros, cerdos, cajas) se realiza utilizando emojis nativos del sistema dibujados en el Canvas, garantizando carga instantánea y cero dependencias de red.

100% Responsivo y Mobile First: * Escalado adaptativo (Letterboxing/Contain) que mantiene la relación de aspecto del nivel sin importar la resolución del dispositivo.

Soporte completo para eventos táctiles (touchstart, touchmove, touchend) con prevención de gestos nativos del navegador (como el pull-to-refresh).

Hitboxes táctiles ampliadas para mayor precisión en pantallas pequeñas.

UX (Experiencia de Usuario) Avanzada:

Predicción de Trayectoria: Línea punteada dinámica que ayuda al jugador a visualizar la parábola del disparo antes de soltar el pájaro.

Interfaz de Usuario limpia: Construida con Tailwind CSS, superpuesta al canvas usando HTML/CSS tradicional para facilitar su modificación sin alterar la lógica de renderizado del juego.

Generación Procedural: A partir del nivel 3, el juego genera estructuras aleatorias para una rejugabilidad infinita.

🛠️ Tecnologías Utilizadas

HTML5 Canvas: Para el renderizado del juego (60 FPS).

JavaScript (ES6+): Lógica del juego, físicas y clases orientadas a objetos.

Tailwind CSS (vía CDN): Para el estilizado rápido de la interfaz de usuario (menús, puntajes).

🎮 Cómo Jugar

Abre el archivo index.html en cualquier navegador web moderno. No se requiere servidor local para jugar.

En PC: Haz clic y mantén presionado el ratón sobre el pájaro en la resortera. Arrastra hacia atrás para apuntar y suelta para disparar.

En Móvil: Toca el pájaro, desliza el dedo hacia atrás y suelta la pantalla para lanzarlo.

Objetivo: Derriba todos los cerditos 🐷 usando la menor cantidad de tiros posibles.

🧠 Estructura del Código (Highlights)

El código está contenido en un solo archivo index.html para máxima portabilidad, organizado en las siguientes secciones lógicas:

Configuración del Canvas: Manejo del escalado dinámico (resizeCanvas).

Clases Principales:

Bird: Maneja el estado (volando, en reposo), vectores de velocidad y el rastro.

Entity: Clase genérica para Cerditos y Bloques, maneja puntos de vida (HP) e interacciones físicas.

Particle: Pequeño sistema de partículas para las explosiones.

Físicas (checkCollisions): Sistema optimizado que calcula colisiones circulares para el pájaro e interacciones de rebote entre entidades.

Game Loop: Bucle principal gestionado por requestAnimationFrame.

🤝 Contribuir

¡Las contribuciones son bienvenidas! Si deseas mejorar las físicas, añadir nuevos tipos de pájaros con habilidades especiales o crear niveles predefinidos más complejos:

Haz un Fork del repositorio.

Crea tu rama de características (git checkout -b feature/NuevaCaracteristica).

Haz Commit de tus cambios (git commit -m 'Añadir Nueva Caracteristica').

Haz Push a la rama (git push origin feature/NuevaCaracteristica).

Abre un Pull Request.

📄 Licencia

Este proyecto es de código abierto y está disponible bajo la Licencia MIT.
