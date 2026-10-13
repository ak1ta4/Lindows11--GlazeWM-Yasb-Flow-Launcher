<h1 align="center">🐧 Windows 11, a lo Linux</h1>

<p align="center"><b>GlazeWM</b> · <b>YASB</b> · <b>Flow Launcher</b></p>

Mi entorno para "linuxificar" Windows 11 y que se parezca a un escritorio tipo i3/Hyprland:

- [GlazeWM](https://github.com/glzr-io/glazewm) como gestor de ventanas en mosaico.
- [YASB](https://github.com/amnweb/yasb) como barra superior.
- [Flow Launcher](https://github.com/Flow-Launcher/Flow.Launcher) como lanzador de aplicaciones al estilo rofi/wofi (`Ctrl + Q`).

## Estructura

| Ruta | Va en | Qué es |
| --- | --- | --- |
| `config.yaml` | `~\.glzr\glazewm\` | Configuración de GlazeWM |
| `yasb/config.yaml` | `~\.config\yasb\` | Barra y widgets de YASB |
| `yasb/styles.css` | `~\.config\yasb\` | Estilos de la barra |
| `yasb/yasb_colors.css` | `~\.config\yasb\` | Colores del sistema (lo genera YASB, no editar) |
| `flowlauncher/` | `%APPDATA%\FlowLauncher\Settings\` | Ajustes de Flow Launcher y de sus plugins |

## GlazeWM

- 9 workspaces, ventanas nuevas en mosaico y huecos de 20 px entre ventanas y 10 px con el borde.
- Borde naranja (`#DD9958`) en la ventana activa y gris en el resto.
- El cursor salta al cambiar de monitor.
- Mientras **Moonlight** tiene el foco, los atajos pasan a la sesión remota (modo `passthrough`). Se sale con `Ctrl+Alt+Shift+F12` o cambiando de ventana.

### Atajos principales

| Atajo | Acción |
| --- | --- |
| `Alt + H/J/K/L` o flechas | Cambiar el foco |
| `Alt + Shift + H/J/K/L` o flechas | Mover la ventana |
| `Alt + Shift + 1/2/3/4` | Mover la ventana al monitor izquierdo / central / pequeño / derecho |
| `Alt + U/I/O/P` | Redimensionar |
| `Alt + R` | Modo redimensionar (HJKL/flechas, `Esc` para salir) |
| `Alt + V` | Cambiar la dirección del mosaico |
| `Alt + Space` | Alternar foco entre mosaico, flotante y pantalla completa |
| `Alt + Shift + Space` | Ventana flotante |
| `Alt + T` / `Alt + F` / `Alt + M` | Mosaico / pantalla completa / minimizar |
| `Alt + Shift + Q` | Cerrar la ventana |
| `Alt + Shift + P` | Pausar GlazeWM |
| `Alt + Shift + R` | Recargar la configuración |
| `Alt + Shift + E` | Salir de GlazeWM |
| `Alt + Enter` | Abrir una terminal |

## YASB

Barra superior de 35 px en el monitor principal, con colores tomados del tema de Windows. Parte del tema [Okinami](https://github.com/MrDLingters/Okinami_YASB) de MrDLingters (ver [Créditos](#créditos)).

- **Izquierda:** menú de inicio (`秋田`) con accesos a carpetas y la ventana activa.
- **Centro:** reloj con calendario, visualizador de audio a ambos lados (simétrico, para que el calendario quede centrado bajo el notch) y el medio en reproducción.
- **Derecha:** bandeja del sistema, volumen, notificaciones, idioma del teclado y centro de control.

## Flow Launcher

Sustituye al menú de inicio: con `Ctrl + Q` se abre una barra de búsqueda para lanzar aplicaciones, buscar archivos o hacer cálculos rápidos sin tocar el ratón.

Prefijos para los plugins:

| Prefijo | Qué hace |
| --- | --- |
| `>` | Ejecutar un comando en la shell |
| `kill` | Cerrar un proceso |
| `b` | Buscar en los marcadores del navegador |
| `s` | Abrir un ajuste de Windows |
| `st` | Buscar juegos de Steam |
| `vo` | Cambiar el volumen |
| `t` | Añadir una tarea (MarkdownTodo) |
| `doc:` | Buscar dentro del contenido de los archivos |
| `pm` | Instalar o gestionar plugins |

Sin prefijo busca aplicaciones, archivos, ajustes del sistema y hace cálculos.

## Créditos

- **Tema de YASB:** [Okinami](https://github.com/MrDLingters/Okinami_YASB), de [MrDLingters](https://github.com/MrDLingters). Mi `yasb/config.yaml` y mi `yasb/styles.css` se basan en su código, publicado en [yasb-themes](https://github.com/amnweb/yasb-themes/tree/main/themes/b51c153d-397c-4be0-b7ed-4f619c6de87f).
