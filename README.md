# glazewm-config

Mi entorno de escritorio en Windows 11: [GlazeWM](https://github.com/glzr-io/glazewm) como gestor de ventanas en mosaico y [YASB](https://github.com/amnweb/yasb) como barra superior.

## Estructura

| Ruta | Va en | Qué es |
| --- | --- | --- |
| `config.yaml` | `~\.glzr\glazewm\` | Configuración de GlazeWM |
| `yasb/config.yaml` | `~\.config\yasb\` | Barra y widgets de YASB |
| `yasb/styles.css` | `~\.config\yasb\` | Estilos de la barra |
| `yasb/yasb_colors.css` | `~\.config\yasb\` | Colores del sistema (lo genera YASB, no editar) |

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

Barra superior de 35 px en el monitor principal, con colores tomados del tema de Windows.

- **Izquierda:** menú de inicio (`家`) con accesos a carpetas y la ventana activa.
- **Centro:** reloj con calendario, visualizador de audio y el medio en reproducción.
- **Derecha:** bandeja del sistema, volumen, notificaciones, idioma del teclado y centro de control.
