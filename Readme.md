# 🎙️ Voice Controlled Music Band Simulator 🎶

A revolutionary, voice-driven music creation application built in Python! Record instrument loops, synthesize custom songs, and control the entire studio experience using **just your voice**.

download link -> https://drive.google.com/file/d/1dextX63qjBfSrsDD-KpluB99EZ9ZcOhp/view?usp=drive_link

---

## ✨ Features

- **🗣️ Voice Command Driven**: Fully hands-free operation! Navigate menus, select instruments, and mix tracks entirely through voice commands.
- **🎸 Multiple Instruments**: Synthesize loops for Piano, Guitar, Drums, and Flute by speaking the sequence of notes!
- **🎤 Live Vocal Recording**: Record your own 30-second vocal tracks directly into the mix.
- **🎛️ Automated Song Mixing**: Seamlessly mixes all your recorded instrument loops and vocals into one cohesive final song.
- **🎧 Real-Time Playback**: Preview and loop individual instruments before mixing.
- **🎨 Sleek GUI**: An intuitive and visually pleasing interface powered by Pygame.
- **✅ Offline Capable**: Bundled with a portable FFmpeg distribution for local audio processing.

---

## 🛠️ Tech Stack

- **[Python 3](https://www.python.org/)**: Core application logic.
- **[Pygame](https://www.pygame.org/)**: Rendering the interactive graphical interface and audio playback.
- **[SpeechRecognition](https://pypi.org/project/SpeechRecognition/)**: Listening and interpreting voice commands.
- **[Pydub](https://pypi.org/project/pydub/)**: Powerful audio manipulation, looping, fading, and mixing.
- **[SoundDevice](https://python-sounddevice.readthedocs.io/)**: Capturing high-quality raw audio from your microphone.

---

## 🚀 Voice Commands Guide

The app constantly listens for commands while in the menu or instrument screens.

### 🏠 Main Menu Commands
- `select piano`
- `select guitar`
- `select drum`
- `select flute`
- `select vocals`
- `make song`
- `play song`
- `pause song`

### 🎵 Instrument/Recording Screen Commands
- `record` (Starts recording notes for instruments or live audio for vocals)
- `play` (Plays the recorded loop for the current instrument)
- `pause` (Stops playback)
- `back` (Returns to the main menu)

**Recording Instrument Notes:**
When recording an instrument (like piano or drums), simply speak the notes you want to hear!
For example:
- `zero one two three four`
- `0 1 2 3 4 5`

---

## 💻 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/siddhantsaxena45/music-band-simulator.git
cd voice-band-simulator/code
```

### 2. Create a Virtual Environment (Recommended)
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. FFmpeg Requirement
Since Pydub relies heavily on FFmpeg for audio processing, ensure FFmpeg is available.
- **Windows**: Download a static build from [gyan.dev](https://www.gyan.dev/ffmpeg/builds/ffmpeg-release-essentials.zip), extract it, and place `ffmpeg.exe` inside a `ffmpeg/bin/` folder in the project directory, or add it to your system PATH.
- **macOS/Linux**: `brew install ffmpeg` or `sudo apt install ffmpeg`.

---

## 🎮 How to Run

Launch the application using:
```bash
python main.py
```
*(Make sure your microphone is connected and set as the default input device!)*

---

## 📦 Building an Executable (Windows)

Want to package the app into a standalone `.exe`? Use PyInstaller!

1. Install PyInstaller:
   ```bash
   pip install pyinstaller
   ```
2. Build the executable:
   ```bash
   pyinstaller --onefile --add-data "assets;assets" --add-data "sounds;sounds" main.py
   ```
3. For the `.exe` to work properly, ensure it sits alongside the following directories:
   - `assets/`
   - `sounds/`
   - `ffmpeg/bin/` (containing `ffmpeg.exe`)

---

## 📸 Screenshots

![Screenshot 1](screenshots/s%20(1).png)
![Screenshot 2](screenshots/s%20(2).png)
![Screenshot 3](screenshots/s%20(3).png)
![Screenshot 4](screenshots/s%20(4).png)
![Screenshot 5](screenshots/s%20(5).png)
![Screenshot 6](screenshots/s%20(6).png)

---

## 📜 License & Credits

MIT License © 2025 Siddhant

**Special Thanks to:**
- [Python](https://python.org)
- [PyGame](https://www.pygame.org)
- [FFmpeg](https://ffmpeg.org)
- Inspired by the vibrant community of voice-controlled audio interfaces!

---

⭐ **Star this repository if you find it interesting or helpful!**
