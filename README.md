# Rock-paper-scissors-game


---

## 📌 **Project Title: Rock-Paper-Scissors Using Hand Gesture Detection**

### 🧠 **Project Description:**

This is a computer vision–based interactive game that allows users to play **Rock-Paper-Scissors** using **hand gestures** in real-time. The system uses **OpenCV** for video processing and **MediaPipe** for hand landmark detection to recognize the user's gesture and compare it with a randomly selected move by the computer.

### 🎯 **Objectives:**

* Recognize hand gestures for Rock, Paper, and Scissors.
* Allow users to play the game through webcam input.
* Provide a countdown timer before gesture recognition.
* Display the result (Win/Lose/Draw) on the screen.

---

### 🛠️ **Technologies Used:**

| Component   | Description                                         |
| ----------- | --------------------------------------------------- |
| `Python`    | Main programming language                           |
| `OpenCV`    | For webcam access and real-time video frame display |
| `MediaPipe` | For real-time hand tracking and landmark detection  |
| `Time`      | For countdown and game flow timing                  |
| `Random`    | To generate computer's random move                  |

---

### ✋ **How It Works:**

1. **Start Game:**

   * User presses the **Spacebar** to begin.
   * A **3-second countdown** is shown to prepare the hand gesture.

2. **Hand Detection:**

   * MediaPipe detects and tracks **21 hand landmarks**.
   * Finger positions (up/down) are analyzed using the y-coordinates of each finger's joints.

3. **Gesture Classification:**

   * **Rock** → All fingers folded → `"00000"`
   * **Paper** → All fingers extended → `"11111"`
   * **Scissors** → Index & middle up, others down → `"01100"`

4. **Computer Move:**

   * Computer randomly picks Rock, Paper, or Scissors.

5. **Game Result:**

   * Compares player's move with the computer's.
   * Displays the outcome (`You Win!`, `You Lose!`, or `It's a Draw!`) with both moves.

---

### 🖼️ **User Interface:**

* Webcam feed with hand tracking annotations
* Game instructions:

  * "PRESS SPACE TO START!"
  * Countdown: "PLAY STARTS IN 3"
  * Prompt: "PLAY NOW!"
* Result display: `"You: Rock | Computer: Paper – You've Lost!"`

---

### ✅ **Key Features:**

* Real-time gesture recognition using webcam.
* Smooth and responsive countdown timer.
* Interactive feedback and game result.
* Fully keyboard-controlled (Space to start, Esc to quit).

---

### 📈 **Applications & Learning Outcomes:**

* Understanding of computer vision and hand tracking.
* Practical use of landmark-based gesture recognition.
* Real-time game logic and UI overlay with OpenCV.
* Combination of multiple Python libraries for real-world interactivity.

---

### 🔄 **Future Enhancements:**

* Add scoring system (user vs computer)
* Improve gesture recognition with custom calibration
* Add sound effects and visual animations
* Support for left-hand detection and multiple players
* GUI interface using Tkinter or PyQt

---


