# HardwareMonitor Dashboard

Lightweight hardware monitoring for your computer hardware in real time.

## 1. System Requirements & Setup

To stream metrics into the dashboard, you must have one or both of the following software running in the background with a web server enabled:

-   **HWiNFO:** Download HWiNFO [here](https://www.hwinfo.com/download/) and requires the [RemoteHWInfo](https://github.com/Demion/remotehwinfo) server enabled.
-   **Libre Hardware Monitor (LHM) or OpenHardwareMonitor (OHM):** Download Libre Hardware Monitor [here](https://github.scom/LibreHardwareMonitor/LibreHardwareMonitor) or OpenHardwareMonitor [here](https://github.com/HardwareMonitor/openhardwaremonitor) (requires the built-in Remote Web Server enabled in the settings).

## 2. Opening and Managing Settings

To customize the layout, cards, and metrics, click the Settings button in the top right corner.

### A. Theme Customization, Presets & Language

Choose a built-in theme or manually adjust all colors using the color pickers:

-   **Preset Themes:** Midnight Obsidian, Cyberpunk Neon, Nordic Frost, Clean Light, Retro Console, Matrix Grid.
-   **Color Fields:** Background (--bg), card background (--card), chart sub-containers (--card-sub), accent colors (--accent), as well as text and border colors.

Language Selection

You can change dashboard language. Supported languages include:

-   English
-   Finnish
-   Svenska
-   Deutsch

### B. Connection Settings & Resolution

-   Run included firewall port-opening script if running dashboard on another device on the same network (e.g. tablet).
-   **HWiNFO/LHM IP:Port:** Define the IP addresses and ports for your hardware sources (e.g., HWiNFO 127.0.0.1:60000 and LHM 127.0.0.1:8085).
-   **Polling Rate (ms):** Define how often data is refreshed in milliseconds (e.g., 4000 = 4 seconds). Click Save & Test when finished.
-   **Resolution Settings:** Choose a preset resolution base or enter a custom width and height to scale the dashboard perfectly for a dedicated sensor display.

### C. Export and Import Settings

-   **Export Settings (JSON):** Back up your current layout, cards, and theme to a file.
-   **Import Settings (JSON):** Restore or load a layout template from a file.

## 4. Managing Cards and Metrics

At the bottom of the settings panel, you will find a list of current Cards that you can modify as follows:

-   **Card Order:** Move cards up or down using the control buttons.
-   **Card Dimensions:** Use sliders to adjust card width (colSpan 1-12), height, and the number of sensor columns.
-   **Charts:** Add live line charts to cards for real-time tracking. Choose the desired metric, color, decimal places, and unit conversion (e.g., MHz to GHz or °C to °F).
-   **Text Sensors & Alerts:** Add individual text-based metrics to a card. You can set an alert value threshold; if exceeded, the value turns red and the respective card activates an alert border (alert-active).

