# 💬 How We Feel+ (Realtime) — Scratch Extension

**How We Feel+ (Realtime)** is a Scratch/PenguinMod extension that detects user emotions in real-time using a webcam. It infers emotional states by analyzing brightness levels and changes from the video feed, allowing Scratch projects to dynamically respond to how the user feels.

> 🔒 Requires **unsandboxed mode** and **camera access**.  
> 🧪 Built using [ExtForge](https://jwklong.github.io/extforge).

---

## 🎯 Features

- 📷 Real-time emotion detection via facecam
- 😃 21+ emotional states supported, including:
  - `happy`, `sad`, `angry`, `excited`, `calm`, `fearful`, `proud`, `bored`, `anxious`, and more
- 🧠 Burst detection for repeated emotional states
- 📈 Tracks emotion counts, logs, and detection stats
- 📡 Sends broadcasts like `I feel happy!` when emotions change
- ⚙️ Configurable detection interval and smart detection toggle

---

## 🧱 Scratch Extension Blocks

| Type     | Block                                                              |
|----------|--------------------------------------------------------------------|
| `hat`    | *(Broadcast-based emotion detection trigger)*                      |
| `command`| `start emotion detection`                                          |
| `command`| `stop emotion detection`                                           |
| `command`| `I feel [emotion]` *(manual override)*                             |
| `command`| `set smart detect to [on/off]`                                     |
| `command`| `set detection interval to [x] seconds`                            |
| `command`| `reset emotion log`                                                |
| `reporter`| `emotion log`                                                    |
| `reporter`| `latest emotion`                                                 |
| `reporter`| `count of [emotion] felt`                                        |
| `reporter`| `detected emotion`                                               |
| `reporter`| `detected emoji`                                                 |
| `reporter`| `emotion % for [emotion]`                                        |
| `reporter`| `emotion percent number for [emotion]`                           |
| `reporter`| `total detections`                                               |
| `reporter`| `most frequent emotion`                                          |
| `boolean` | `detect burst (same emotion 3+ times)`                            |

---

## 🧪 How It Works

1. Accesses the webcam using `getUserMedia()`
2. Analyzes each video frame’s brightness data
3. Determines the most likely emotion based on heuristic thresholds
4. Updates emotion state, triggers broadcasts, and logs detection stats

---

## 🚀 Usage Instructions

1. Use in **PenguinMod** or another Scratch fork with **unsandboxed extension support**
2. Load the extension file (via ExtForge or direct embed)
3. Grant camera access when prompted
4. Start detection and use reporter blocks to react in your project

---

## 🛠 Use Cases

- Emotion-aware games and characters
- Mood-adaptive music or story projects
- Learning tools for emotional awareness
- Personal well-being dashboards in Scratch

---

## 📜 Notes

- This extension does **not use AI or ML**, only light-based heuristics
- No video or audio data is stored or transmitted
- Accuracy depends on lighting and camera quality

---

## 🧠 Credits

Created by **Nedas15930**  
Built using [ExtForge](https://jwklong.github.io/extforge)

---

> 🎉 Contributions, forks, and feedback are welcome!  
> You are free to customize the emotion set, visuals, and detection logic for your needs.

