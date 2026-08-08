# HardwareMonitor Dashboard

A modern, customizable hardware monitoring dashboard for displaying real-time PC sensor data in a clean and highly configurable interface.

HardwareMonitor Dashboard can combine data from **HWiNFO**, **Libre Hardware Monitor**, or **OpenHardwareMonitor** and display it through customizable cards, charts, sensors, alerts, and themes.

---

## ✨ Features

- 📊 **Real-time hardware monitoring**
- 🖥️ Customizable dashboard layout
- 🎨 Multiple built-in themes
- 🌈 Fully customizable colors
- 📈 Live sensor charts
- 🚨 Sensor thresholds and visual alerts
- 📉 Trend sparklines
- 🔄 Global and per-card refresh rates
- 🧩 Drag-and-drop card ordering
- 📐 Custom card sizes and sensor columns
- 👀 Live configuration previews
- 🌡️ Unit conversion support
- 💾 JSON configuration export/import
- 🖥️ Custom resolution scaling
- 🌐 Remote monitoring over your local network

---

## 📡 Supported Hardware Sources

The dashboard can receive sensor data from one or both of the following sources:

### HWiNFO

[HWiNFO](https://www.hwinfo.com/download/) is supported through the [RemoteHWInfo](https://github.com/Demion/remotehwinfo) server.

Enable the RemoteHWInfo server and configure its address and port in the dashboard settings.

### Libre Hardware Monitor

[Libre Hardware Monitor](https://github.com/LibreHardwareMonitor/LibreHardwareMonitor) can be used with its built-in Remote Web Server.

### OpenHardwareMonitor

[OpenHardwareMonitor](https://github.com/openhardwaremonitor/openhardwaremonitor) is also supported through its built-in Remote Web Server.

---

## 🚀 Getting Started

### 1. Start a Hardware Monitoring Source

Run at least one supported hardware monitoring application:

- HWiNFO + RemoteHWInfo
- Libre Hardware Monitor
- OpenHardwareMonitor

Make sure its web server is enabled.

### 2. Start the Dashboard

Launch the dashboard and open **Settings**.

### 3. Configure the Connection

Enter the IP address and port of your hardware monitoring source.

Example configuration:

```text
HWiNFO: 127.0.0.1:60000
LHM:    127.0.0.1:8085
```

Configure the polling interval according to your needs.

For example:

```text
4000 ms = 4 seconds
```

Click **Save & Test** to verify the connection.

---

## ⚙️ Configuration

The dashboard provides extensive customization through the **Settings** panel.

### 🎨 Themes

Several built-in presets are available:

- Midnight Obsidian
- Cyberpunk Neon
- Nordic Frost
- Clean Light
- Retro Console
- Matrix Grid
- and many more (total 30 options)

You can also customize individual colors, including:

- Background
- Card background
- Chart containers
- Accent color
- Text
- Borders

---

## 🧩 Dashboard Cards

Cards are the main building blocks of the dashboard.

Each card can be customized independently.

### Layout

- Reorder cards using the controls in Settings
- Drag and drop cards directly on the dashboard
- Adjust card width
- Adjust card height
- Configure the number of sensor columns

### Collapsible Sections

Cards and their internal groups can be collapsed to keep complex dashboards organized.

### Live Preview

While editing a card, the configuration interface provides a live preview with animated mock values.

This allows you to configure the dashboard without constantly switching between the settings and dashboard views.

---

## 📈 Charts

Cards can contain live line charts for monitoring sensor values over time.

Charts support:

- Custom metrics
- Custom colors
- Font size
- Decimal precision
- Unit conversion
- Area fill
- Line width
- Side-by-side or stacked layouts

Multiple charts can be customized individually, or the **Paint All Charts** control can be used to apply a color across all charts in a card.

---

## 📊 Text Sensors

Text sensors provide a compact way of displaying individual hardware metrics.

They support:

- Custom sensor values
- Alert thresholds
- Trend sparklines
- Dynamic color thresholds
- Multiple value-based colors

For example, a sensor can change color when a value reaches a specified threshold:

```text
Value ≥ X → Custom color
```

When an alert threshold is exceeded, the sensor value turns red and the associated card can display an alert border.

---

## 🔄 Refresh Rates

The dashboard supports both global and per-card refresh rates.

### Global Polling Rate

Controls how frequently hardware data is retrieved.

Example:

```text
4000 ms → refresh every 4 seconds
```

### Per-Card Refresh Rate

Individual cards can override the global polling interval.

This allows frequently changing sensors to update faster while keeping less important cards at a lower refresh rate.

---

## 🖥️ Resolution & Dedicated Displays

The dashboard can be configured for dedicated sensor displays.

You can select a predefined resolution or enter a custom:

```text
Width × Height
```

This is useful for setups such as:

- Secondary monitors
- Small sensor displays
- Tablets
- Dedicated monitoring screens

If the dashboard is accessed from another device on the same network, the included firewall port-opening script may be required.

---

## 💾 Import & Export

Dashboard configurations can be backed up and transferred using JSON files.

### Export

Export your current:

- Layout
- Cards
- Sensor configuration
- Theme settings

to a JSON file.

### Import

Import a previously exported JSON configuration to restore or share a dashboard layout.

This also makes it easy to create and distribute custom dashboard presets.

---

## 🌐 Remote Monitoring

The dashboard can be accessed from another device on the same local network.

This makes it possible to turn an old tablet or secondary display into a dedicated hardware monitoring screen.

Script to open required default ports for local network usage is included in the release archive.

---

## 🤝 Contributing

Contributions, suggestions, bug reports, and feature requests are welcome.

If you find a problem or have an idea for improving the dashboard, feel free to open an **Issue** or submit a **Pull Request**.

---

## ⭐ Support

If you find HardwareMonitor Dashboard useful, consider giving the repository a ⭐ on GitHub.

Enjoy building your own monitoring dashboard!
