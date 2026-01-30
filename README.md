# Configuración Personal de VS Code

Una configuración sencilla para Visual Studio Code que deshabilita las funciones de IA/Copilot y establece un entorno de desarrollo personalizado y automatizado.

[![Release VSCode Config](https://github.com/baa4ts/vscode-config/actions/workflows/release-vscode.yml/badge.svg)](https://github.com/baa4ts/vscode-config/actions/workflows/release-vscode.yml)
## 📋 Qué hace esta configuración

Esta configuración realiza automáticamente lo siguiente:
*   **Deshabilita por completo** GitHub Copilot, Copilot Chat y todas las sugerencias de IA.
*   **Configura la apariencia** con el tema Tokyo Night Storm y los iconos Material Icons.
*   **Instala un conjunto de extensiones útiles** para el desarrollo.
*   **Aplica reglas de formato** básicas (como formatear al guardar).
*   **Reduce la telemetría** del editor.

## 🧩 Lista de extensiones

| Extensión | Descripción |
| :--- | :--- |
| **Tokyo Night** | Tema de color oscuro elegante. |
| **Material Icon Theme** | Iconos detallados para el explorador de archivos. |
| **Error Lens** | Muestra errores y advertencias directamente en la línea de código. |
| **Thunder Client** | Cliente HTTP para probar APIs (similar a Postman). |
| **Better Comments** | Colorea los comentarios para categorizarlos. |

## 🚀 Cómo se usa

1.  En la carpeta raíz de tu proyecto, crea una carpeta llamada **`.vscode`**.
2.  Dentro de ella, crea y guarda los siguientes tres archivos de configuración:
    *   `settings.json` (configuración del editor)
    *   `extensions.json` (lista de extensiones)
    *   `tasks.json` (tarea de instalación automática para Windows)
3.  **Asegúrate de que el comando `code` esté disponible** en tu sistema. Para ello, en VS Code, abre la Paleta de Comandos (`Ctrl+Shift+P`), busca y ejecuta **"Shell Command: Install 'code' command in PATH"**.
4.  Cierra y vuelve a abrir la carpeta de tu proyecto en VS Code. La primera vez, debes **permitir la ejecución automática de tareas** cuando te lo pregunte.

> [!CAUTION]
> **Nota:** El archivo `tasks.json` proporcionado está configurado para **Windows**. Si usas Linux o macOS, necesitarás un comando diferente (normalmente basado en `bash` y `jq`).
