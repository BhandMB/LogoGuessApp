# LogoGuessApp

A fun and interactive Logo Guessing Game Android App built using **Java + Android SDK**, where users test their knowledge of popular brand logos. The project is designed as a practical Android application for learning activities, intents, UI design, state management, and local score persistence.

## 🚀 Features

- 🎯 Guess logos from popular brands
- 🧩 Multiple difficulty levels (Easy, Medium, Hard)
- 🏆 Score tracking
- 💾 Local score persistence with SharedPreferences
- 📱 Clean and responsive Android UI

## 🛠️ Tech Stack

- **Language:** Java
- **Framework:** Android SDK
- **IDE:** Android Studio
- **Concepts:** Activities & Intents, RecyclerView / GridView, OOP, JSON parsing, SharedPreferences, file handling, and basic animations

## 📂 Project Structure

```text
LogoGuessApp/
│── app/
│   ├── java/com/example/logoguessapp/
│   │   ├── MainActivity.java
│   │   ├── GameActivity.java
│   │   ├── ResultActivity.java
│   │   ├── adapter/
│   │   ├── model/
│   │   │   └── Logo.java
│   │   ├── utils/
│   │   │   └── ScoreManager.java
│   │
│   ├── res/
│   │   ├── layout/
│   │   │   ├── activity_main.xml
│   │   │   ├── activity_game.xml
│   │   │   ├── activity_result.xml
│   │   ├── drawable/
│   │   │   └── logos/
│   │   ├── values/
│   │   │   ├── strings.xml
│   │   │   ├── colors.xml
│   │
│   ├── assets/
│   │   └── questions.json
│   │
│── build.gradle
│── README.md
```

## ▶️ Getting Started

1. Clone the repository:

```bash
git clone https://github.com/BhandMB/LogoGuessApp.git
```

2. Open the project in **Android Studio**.
3. Allow Gradle to synchronize dependencies.
4. Select an Android emulator or connected device.
5. Build and run the `app` module.

> The exact Android SDK/Gradle versions should be taken from the project's Gradle configuration when setting up a development environment.

## 🧪 Development Checklist

Before publishing a new version, verify:

- [ ] The app builds successfully
- [ ] Logo questions load correctly
- [ ] Easy, Medium, and Hard modes work
- [ ] Correct and incorrect answers update the score
- [ ] Result screen displays the final score
- [ ] Saved scores persist after restarting the app
- [ ] UI works on different screen sizes

## 📚 Learning Outcomes

This project provides hands-on practice with:

- Android app lifecycle
- UI design using XML
- Activity navigation and intents
- State management
- Local persistence with SharedPreferences
- JSON-based application data
- Debugging real-world application behavior

## 🔧 Future Improvements

- Add a larger question bank
- Add timed quiz mode
- Add sound and haptic feedback
- Add a persistent leaderboard
- Migrate question data to a remote API
