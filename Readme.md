# 🌌 Gesture Controlled Space Shooter

A unique, interactive Space Shooter game built in Python that uses **computer vision** and **hand gestures** to control the player's ship! Powered by Pygame, OpenCV, and MediaPipe, this game offers an immersive experience where you use your hands to steer your ship and blast enemies out of the sky.

download link -> https://drive.google.com/file/d/1dextX63qjBfSrsDD-KpluB99EZ9ZcOhp/view?usp=drive_link
---

## ✨ Features

- **✋ Hand Gesture Controls**: Steer your ship and shoot using real-time hand tracking.
- **🎮 Classic Keyboard Controls**: Traditional arrow keys and spacebar support as a fallback or for precision movement (including vertical movement).
- **🚀 4 Unique Levels & Boss Fights**: Face off against increasingly difficult waves of enemies and challenge unique bosses in levels 2, 3, and 4!
- **⚡ Power-Ups**: Collect dynamic power-ups that drop during gameplay:
  - 💚 **Health**: Restores 30 HP to keep you in the fight.
  - 🛡️ **Shield**: Grants 5 seconds of invulnerability (indicated by a cyan aura).
  - 🚀 **Rapid Fire**: Massively boosts your firing rate for 5 seconds.
- **📷 Real-Time Feedback**: A secondary window displays your camera feed with live hand-tracking landmarks and recognized action text (LEFT, RIGHT, FIRE).

---

## 🛠️ Tech Stack

- **[Python 3](https://www.python.org/)**: Core programming language.
- **[Pygame](https://www.pygame.org/)**: Rendering, game loop, collision detection, and audio.
- **[OpenCV](https://opencv.org/)**: Webcam feed capture and image processing.
- **[MediaPipe](https://developers.google.com/mediapipe)**: Advanced hand landmark detection.

---

## 🚀 Installation & Setup

1. **Clone this repository:**
   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ```

2. **Create and activate a virtual environment (Recommended):**
   ```bash
   # On Windows
   python -m venv venv
   venv\Scripts\activate

   # On macOS/Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

---

## 🕹️ How to Play

Start the game by running:
```bash
python main.py
```
*(Ensure your webcam is connected and unblocked before starting the game!)*

### Controls

The game translates your hand movements in real-time into game inputs using your webcam.

| Control Type | Action | Input Mechanism |
| :--- | :--- | :--- |
| **🖐️ Gesture** | **Move Left** | Move your **Index Finger** towards the **left** side of the camera view (x < 0.4). |
| **🖐️ Gesture** | **Move Right** | Move your **Index Finger** towards the **right** side of the camera view (x > 0.6). |
| **🖐️ Gesture** | **Fire Laser** | **Pinch** your **Thumb and Index Finger** together. |
| **⌨️ Keyboard** | **Movement** | Use the `Up`, `Down`, `Left`, and `Right` arrow keys. |
| **⌨️ Keyboard** | **Fire Laser** | Press the `Spacebar`. |

**💡 Pro Tip:** The "Hand Detection" camera window displays text (e.g., "LEFT!", "FIRE!") to help you understand what the game is recognizing. Keep your hand visible and well-lit for the best tracking performance!

---

## 👾 Gameplay Mechanics

### Enemies
- **Standard Enemies**: Red, Green, and Blue ships that fly downward and shoot lasers.
- **Bosses**: 
  - Encountered at the climax of levels 2, 3, and 4.
  - Features high health and unique spread-shot or multi-laser attacks.
  - Must be defeated to clear the level!

### Player Stats
- **Health**: You start with 100 HP. Taking hits from lasers or crashing into enemies reduces it.
- **Lives**: You have 5 lives. Letting an enemy ship pass you costs a life. 
- You lose if your health reaches 0 or if you run out of lives.

---

## 📸 Screenshots


![Screenshot 1](screenshots/s%20(1).png)
![Screenshot 2](screenshots/s%20(2).png)
![Screenshot 3](screenshots/s%20(3).png)
![Screenshot 4](screenshots/s%20(4).png)
![Screenshot 5](screenshots/s%20(5).png)
![Screenshot 6](screenshots/s%20(6).png)

---

## 🛑 Important Notes

- When you start the game, **two windows** will open: the main Pygame window and the "Hand Detection" webcam feed.
- If tracking is poor, ensure you are in a well-lit room and that your hand is clearly visible to the camera.
- To exit the game, simply click the "Quit" button on the main menu or close the Pygame window.
