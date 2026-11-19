# Guitar Hero 5 Recomp

**[🇦🇷 Español](#-español)** · **[🇬🇧 English](#-english)**

---

## 🇦🇷 Español

🚧 **Estado del proyecto: Alpha.** Proyecto experimental y no oficial. Vulkan sigue en desarrollo y la compilación inicial de shaders puede provocar tirones.

### 🤖 Aclaración sobre el desarrollo asistido por IA

Sí, este proyecto se desarrolla con ayuda de inteligencia artificial, principalmente ChatGPT. Prefiero dejarlo claro desde el principio.

No pretendo ser un desarrollador profesional de emuladores, ingeniero de gráficos ni experto en ingeniería inversa. Mi parte es decidir qué hay que mejorar, probar el juego, investigar los errores, comparar resultados y seguir ajustando hasta acercarnos a la experiencia original de Xbox 360.

Generalmente pasa algo así:

> **Yo:** «¿Podemos hacer que Guitar Hero 5 funcione bien en PC?»
> **IA:** «Podemos intentarlo».
> **Yo, varias compilaciones después:** «Bueno, ¿y ahora por qué las notas se atrasan respecto de la música?» 😅

Todo esto acompañado de pruebas reales jugando y bastante depuración. Las críticas, los reportes de fallos y la ayuda de la comunidad son bienvenidos.

### 🎵 Sobre el proyecto

**Guitar Hero 5 Recomp** es un proyecto independiente de compatibilidad cuyo objetivo es ejecutar la versión de Xbox 360 de Guitar Hero 5 en Windows mediante un entorno basado en ReXGlue.

La idea no es rehacer ni reemplazar el juego, sino preservar su experiencia original mientras mejoramos la compatibilidad con PC, la sincronización musical, los gráficos, los controles y la estabilidad.

### ⚙️ Objetivos actuales de desarrollo

- **Audio y sincronización de notas:** investigar desfases progresivos, estabilidad en canciones largas y relojes de juego consistentes.
- **Gráficos:** desarrollar y probar renderizadores para PC, incluido Direct3D 12. Vulkan sigue en desarrollo y puede ser inestable.
- **Rendimiento:** trabajar sobre el ritmo de fotogramas, V-Sync, tirones relacionados con shaders y estabilidad.
- **Controles:** mejorar la asignación de teclado y joystick para guitarra, bajo y batería.
- **Launcher y configuración:** simplificar la selección de la carpeta del juego y los ajustes del runtime.

Son áreas en desarrollo: no significa que todos estos problemas estén resueltos.

### 🛠️ Instalación y pruebas

1. Descargá la compilación disponible más reciente desde la sección **Releases** del repositorio.
2. Extraé el archivo en la carpeta que prefieras.
3. Abrí el launcher y entrá en la pestaña **Carpetas**. Buscá y seleccioná el archivo `default.xex` de tu propia copia de Guitar Hero 5 para Xbox 360.
4. Desde esa misma pestaña **Carpetas**, elegí dónde se guardarán las partidas y los perfiles. Asegurate de que la carpeta seleccionada permita guardar archivos.
5. Configurá los gráficos y controles disponibles y luego iniciá el juego.
6. Si encontrás un cierre inesperado, desincronización o problemas de controles, informá la versión, el renderizador elegido y cómo reproducir el problema.

### ⚠️ Vulkan y compilación de shaders por primera vez

- Vulkan todavía está en desarrollo. Es experimental y puede presentar tirones adicionales o problemas de estabilidad.
- La primera vez que entrás a una canción, un escenario (*venue*) o un menú, puede haber pequeños congelamientos o tirones. Esto ocurre porque algunos shaders se compilan en caliente, justo cuando el juego los necesita por primera vez.
- Al volver a visitar ese contenido, el rendimiento puede mejorar gracias a los shaders ya compilados o guardados en caché, pero no significa que todos los tirones estén solucionados.

No se incluyen archivos originales del juego, canciones ni recursos protegidos por derechos de autor. Las funciones disponibles pueden cambiar entre versiones Alpha.

### 🙏 Créditos y comunidad

Un agradecimiento especial a **Tom (crack)**, creador y responsable principal de ReXGlue, y a todos sus colaboradores. Su conjunto de herramientas para recompilar juegos de Xbox 360 es la base tecnológica de este proyecto.

- ReXGlue SDK (proyecto oficial): https://github.com/rexglue/rexglue-sdk
- Creador de ReXGlue, Tom (`tomcl7`): https://github.com/tomcl7

Gracias también a quienes prueban las versiones Alpha, reportan problemas y ayudan a investigar errores. Todos los autores y colaboradores originales conservan el crédito por su trabajo.

💬 [Sumate a nuestro Discord de Guitar Hero Modding Hub](https://discord.gg/TcZYbD7q4)

### ⚖️ Aviso legal

Este es un proyecto no oficial creado por fans con fines de compatibilidad, experimentación y preservación. No está afiliado, patrocinado ni respaldado por Activision, Neversoft, Microsoft, Xbox ni otros titulares de derechos.

Guitar Hero, Guitar Hero 5 y sus marcas y recursos asociados pertenecen a sus respectivos propietarios. No se distribuye el juego original ni contenido protegido por derechos de autor. Cada usuario debe disponer de su propia copia obtenida legalmente.

### 🤘 Nota final

Guitar Hero 5 es uno de mis juegos favoritos. Lo único que quería era disfrutarlo en PC como lo recordaba en Xbox 360.

Y de alguna manera terminé investigando relojes de audio, renderizadores, controles, registros de errores y carpetas llamadas `Alpha`, `FIX`, `R2` y `FINAL_AHORA_SI`. Si algo falla, seguro aparece otra compilación para investigarlo. 😎

¡Saludos desde Rosario, Santa Fe, Argentina! 🇦🇷

---

## 🇬🇧 English

🚧 **Project status: Alpha.** Experimental, unofficial project. Vulkan is still under development, and the initial shader compilation can cause stutter.

### 🤖 A note on AI-assisted development

Yes, this project is developed with the help of artificial intelligence, mainly ChatGPT. I'd rather make that clear from the start.

I don't claim to be a professional emulator developer, graphics engineer or reverse-engineering expert. My part is deciding what needs improving, testing the game, investigating bugs, comparing results and keeping on tweaking until we get closer to the original Xbox 360 experience.

It usually goes something like this:

> **Me:** "Can we make Guitar Hero 5 run well on PC?"
> **AI:** "We can try."
> **Me, several builds later:** "So, why are the notes now falling behind the music?" 😅

All of it comes with real playtesting and a fair amount of debugging. Criticism, bug reports and help from the community are welcome.

### 🎵 About the project

**Guitar Hero 5 Recomp** is an independent compatibility project that aims to run the Xbox 360 version of Guitar Hero 5 on Windows through a ReXGlue-based environment.

The idea is not to remake or replace the game, but to preserve its original experience while improving PC compatibility, music synchronization, graphics, controls and stability.

### ⚙️ Current development goals

- **Audio and note synchronization:** investigate progressive drift, stability in long songs and consistent game clocks.
- **Graphics:** develop and test PC renderers, including Direct3D 12. Vulkan is still under development and may be unstable.
- **Performance:** work on frame rate, V-Sync, shader-related stutter and stability.
- **Controls:** improve keyboard and joystick mapping for guitar, bass and drums.
- **Launcher and settings:** simplify choosing the game folder and the runtime settings.

These are areas under development: it doesn't mean all of these problems are solved.

### 🛠️ Installation and testing

1. Download the latest available build from the repository's **Releases** section.
2. Extract the archive to any folder you like.
3. Open the launcher and go to the **Folders** tab. Browse for and select the `default.xex` file from your own copy of Guitar Hero 5 for Xbox 360.
4. In that same **Folders** tab, choose where saves and profiles will be stored. Make sure the selected folder allows writing files.
5. Configure the available graphics and controls, then start the game.
6. If you run into an unexpected crash, desync or controller problems, please report the version, the renderer you chose and how to reproduce the problem.

### ⚠️ Vulkan and first-time shader compilation

- Vulkan is still under development. It is experimental and may show extra stutter or stability problems.
- The first time you enter a song, a venue or a menu, you may notice small freezes or stutter. This happens because some shaders are compiled on the fly, right when the game needs them for the first time.
- When you revisit that content, performance may improve thanks to shaders that are already compiled or cached, but that doesn't mean all stutter is fixed.

No original game files, songs or copyrighted assets are included. Available features may change between Alpha versions.

### 🙏 Credits and community

Special thanks to **Tom (crack)**, creator and lead maintainer of ReXGlue, and to all of its contributors. Their toolset for recompiling Xbox 360 games is the technological foundation of this project.

- ReXGlue SDK (official project): https://github.com/rexglue/rexglue-sdk
- ReXGlue creator, Tom (`tomcl7`): https://github.com/tomcl7

Thanks as well to everyone who tests the Alpha builds, reports problems and helps investigate bugs. All original authors and contributors keep the credit for their work.

💬 [Join our Guitar Hero Modding Hub Discord](https://discord.gg/TcZYbD7q4)

### ⚖️ Legal notice

This is an unofficial, fan-made project created for compatibility, experimentation and preservation purposes. It is not affiliated with, sponsored by or endorsed by Activision, Neversoft, Microsoft, Xbox or any other rights holders.

Guitar Hero, Guitar Hero 5 and their associated trademarks and assets belong to their respective owners. The original game and copyrighted content are not distributed. Each user must have their own legally obtained copy.

### 🤘 Final note

Guitar Hero 5 is one of my favorite games. All I wanted was to enjoy it on PC the way I remembered it on Xbox 360.

And somehow I ended up investigating audio clocks, renderers, controls, error logs and folders named `Alpha`, `FIX`, `R2` and `FINAL_AHORA_SI`. If something breaks, there will surely be another build to investigate. 😎

Greetings from Rosario, Santa Fe, Argentina! 🇦🇷
