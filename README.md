# Live Interpreter
## Real-time Speech Translation: Arabic ↔ English

**Designed & Developed by Nashat Shamsady**

A professional-grade live interpreter application that converts spoken language in real-time between Arabic and English with ultra-low latency.

---

## Features

- 🎤 **Real-time Speech-to-Text** - Live transcription as you speak
- 🌐 **AI-Powered Translation** - Context-aware Azure Speech Translation
- ⚡ **Ultra-Low Latency** - Target 1-2 second end-to-end delay
- 🖥️ **Modern UI** - Professional interpreter-style dual-panel interface
- 🌙 **Dark/Light Themes** - Easy on the eyes for long sessions
- ⌨️ **Global Hotkeys** - Control from any application
- 🔒 **Privacy-First** - No permanent audio storage

---

## Quick Start

### 1. Install Dependencies

```bash
cd "D:\Speech to text"
pip install -r requirements.txt
```

### 2. Configure Azure Speech Services

1. Create an Azure Speech Services resource at [portal.azure.com](https://portal.azure.com)
2. Copy your API key and region
3. Launch the app and go to Settings (⚙️) to enter your credentials

### 3. Run the Application

**Dictation Mode (NEW - Types into any app!):**
```bash
python dictate.py
```

**Full Interpreter Mode:**
```bash
python run.py
```

---

## Two Modes

### 🎤 Dictation Mode (`dictate.py`)
- **Lightweight** - Fast startup, minimal UI
- **Auto-types** - Recognized speech is typed directly into any active window
- **Auto language detection** - Arabic, English, Kurdish
- **Floating overlay** - Small draggable status window

### 🌐 Interpreter Mode (`run.py`)
- **Full UI** - Dual-panel translation interface
- **Real-time translation** - Arabic ↔ English
- **Professional** - Suitable for meetings and lectures

---

## Global Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Shift + 1` | Start Listening |
| `Ctrl + Shift + 2` | Stop Listening |
| `Ctrl + Shift + 3` | Toggle Always-on-Top |
| `Ctrl + Shift + 4` | Mute/Unmute Microphone |

These shortcuts work globally when the application is running.

---

## Project Structure

```
D:\Speech to text\
├── live_interpreter/
│   ├── __init__.py
│   ├── main.py              # Application entry point
│   ├── config.py            # Configuration management
│   ├── core/
│   │   ├── audio_capture.py # Microphone audio handling
│   │   ├── speech_recognizer.py # Azure STT
│   │   └── translator.py    # Azure Speech Translation
│   ├── ui/
│   │   ├── main_window.py   # Main interpreter window
│   │   ├── splash_screen.py # Startup splash
│   │   ├── about_dialog.py  # About page
│   │   ├── settings_dialog.py # Settings
│   │   ├── widgets/
│   │   │   ├── live_panel.py # Live text display
│   │   │   └── status_bar.py # Status indicators
│   │   └── styles/
│   │       ├── dark_theme.qss
│   │       └── light_theme.qss
│   ├── hotkeys/
│   │   └── global_shortcuts.py
│   └── utils/
│       └── logger.py
├── requirements.txt
├── run.py
└── README.md
```

---

## Requirements

- **OS**: Windows 10/11
- **Python**: 3.11+
- **Azure**: Speech Services subscription

---

## Credits

**Live Interpreter** is designed and developed by **Nashat Shamsady**.

© 2025 Nashat Shamsady. All Rights Reserved.
