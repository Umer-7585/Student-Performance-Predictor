# 🎓 Student Performance Predictor

> An AI-powered Android application that predicts student academic performance, provides personalized insights, and enforces a smart focus-lock system to improve study habits.

---

## About the App

**Student Performance Predictor** is an intelligent Android mobile application designed to help students understand and improve their academic performance. By analyzing key study-related parameters — including daily study hours, attendance rate, assignment completion, class participation, sleep habits, previous grades, and stress levels — the app predicts a student's expected score and grade using a weighted algorithm.

The app also features a unique **App Lock** mechanism: if a student's predicted performance falls below 50%, the app activates a 1-hour focus lock, encouraging the student to step away and dedicate time to their studies. A detailed **Skill Radar chart** visualizes individual strengths and weaknesses, while an **AI Advisor Insights** panel provides personalized academic recommendations.

This app is ideal for students, academic advisors, and educators who want a data-driven approach to monitoring and improving student outcomes.

---

## App Screenshots

| Login Screen | Main Dashboard | Analysis Result |
|:---:|:---:|:---:|
| ![Login](screenshots/login_screen.png) | ![Dashboard](screenshots/dashboard.png) | ![Analysis](screenshots/analysis_result.png) |

| Skill Radar & AI Insights | App Locked Screen |
|:---:|:---:|
| ![Skill Radar](screenshots/skill_radar.png) | ![App Locked](screenshots/app_locked.png) |

---

## Features

- 🔐 **User Authentication** — Secure email/password login and sign-up with session management
- 📊 **Performance Prediction** — Weighted algorithm predicts student score and assigns a grade (A–F)
- 🎯 **Interactive Sliders** — Adjust 7 key academic parameters with intuitive real-time sliders
- 📡 **Skill Radar Chart** — Spider/radar visualization of academic strengths across all dimensions
- ⚠️ **Weakness Analysis** — Automatically identifies and highlights areas needing improvement
- 🤖 **AI Advisor Insights** — Personalized academic recommendations powered by AI
- 🔒 **Smart App Lock** — Automatically locks the app for 1 hour if predicted performance is below 50%
- 🌙 **Dark Theme UI** — Sleek, modern dark-mode interface for comfortable use
- 📱 **Offline Support** — Core prediction features work without internet connectivity
- 💾 **Session Persistence** — User data and preferences saved across sessions

---

## Technologies Used

| Category | Technology |
|---|---|
| Language | Java / Kotlin |
| IDE | Android Studio |
| UI | XML Layouts + Material Design |
| Charts | MPAndroidChart (Radar Chart) |
| Authentication | Firebase Authentication |
| Database | Firebase Firestore / SharedPreferences |
| AI Integration | OpenAI API (AI Advisor Insights) |
| Build System | Gradle |
| Minimum SDK | Android 8.0 (API 26) |
| Target SDK | Android 14 (API 34) |

---

## APK Download

📥 [**Download APK**](apk/StudentPerformancePredictor.apk)

> **File:** `StudentPerformancePredictor.apk`
> **Size:** ~8 MB
> **Requires:** Android 8.0 or above

---

## How to Install the APK

1. Download the APK file from the link above.
2. Transfer the APK to your Android device (if downloaded on a PC).
3. On your Android device, go to **Settings → Security** (or **Settings → Apps → Special Access**).
4. Enable **"Install from Unknown Sources"** or **"Allow from this source"**.
5. Open the APK file using a file manager.
6. Tap **Install** and wait for installation to complete.
7. Open **Student Performance Predictor** from your app drawer.

---

## How to Run the Project in Android Studio

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/StudentPerformancePredictor.git
   ```

2. **Open in Android Studio:**
   - Launch Android Studio
   - Select **File → Open**
   - Navigate to the cloned `StudentPerformancePredictor/` folder and click **OK**

3. **Sync Gradle:**
   - Wait for Android Studio to sync all Gradle dependencies automatically
   - If prompted, click **"Sync Now"**

4. **Configure Firebase:**
   - Go to [Firebase Console](https://console.firebase.google.com)
   - Create a new project or use an existing one
   - Download `google-services.json` and place it in the `app/` directory
   - Enable **Authentication** (Email/Password) and **Firestore Database**

5. **Configure AI API Key (optional):**
   - Add your OpenAI API key to `local.properties`:
     ```
     OPENAI_API_KEY=your_api_key_here
     ```

6. **Run the app:**
   - Connect an Android device via USB (with USB Debugging enabled), or start an emulator
   - Click the green **Run ▶** button in Android Studio

---

## How to Use the App

1. **Sign Up / Login** — Create an account or log in with your email and password.
2. **Set Parameters** — On the main dashboard, adjust the 7 sliders to match your current academic profile:
   - 📚 Daily Study Hours
   - 🏫 Attendance Rate
   - 📝 Assignment Completion
   - 🙋 Class Participation
   - 😴 Sleep Hours/Night
   - 📋 Previous Grade
   - 😰 Stress Level
3. **Analyze** — Tap the **"Analyze Performance"** button.
4. **Review Results** — View your predicted score, grade, skill radar chart, weakness analysis, and AI advisor insights.
5. **Focus Lock** — If your score is below 50%, the app will lock for 1 hour with a motivational message to encourage studying.

---

## Demo Video

📹 [Watch Demo Video](demo-video-link)

> *(Update this link with your actual demo video URL — YouTube, Google Drive, etc.)*

---

## Privacy Policy

This app may collect and process the following user data:
- Email address (for authentication)
- Academic performance inputs (processed locally or via AI)

📄 [**View Full Privacy Policy**](docs/privacy_policy.pdf)

All data is handled in accordance with applicable privacy laws. See the full policy for details.

---

## Future Enhancements

- 📈 **Historical Tracking** — Save and compare performance predictions over time
- 👨‍🏫 **Instructor Dashboard** — Allow teachers to monitor class-wide performance trends
- 🔔 **Smart Notifications** — Daily study reminders and motivational alerts
- 🌐 **Multi-language Support** — Localization for non-English-speaking students
- 📊 **Detailed Reports** — Export performance reports as PDF
- 🎮 **Gamification** — Reward badges and streaks for consistent study habits
- ☁️ **Cloud Sync** — Sync performance history across multiple devices
- 🧠 **Improved AI Model** — Train a custom ML model on real student data for higher prediction accuracy

---

## Project Structure

```
StudentPerformancePredictor/
│
├── app/                          # Complete Android project source code
│   ├── src/main/java/            # Java/Kotlin source files
│   ├── src/main/res/             # XML layouts, drawables, strings
│   └── build.gradle              # App-level Gradle config
│
├── screenshots/                  # App screen captures
│   ├── login_screen.png
│   ├── dashboard.png
│   ├── analysis_result.png
│   ├── skill_radar.png
│   └── app_locked.png
│
├── apk/                          # Installable APK file
│   └── StudentPerformancePredictor.apk
│
├── docs/                         # Documentation
│   ├── privacy_policy.pdf
│   └── user_manual.pdf
│
├── README.md                     # This file
├── LICENSE                       # MIT License
├── .gitignore                    # Git ignore rules
├── build.gradle                  # Root Gradle config
└── settings.gradle               # Gradle settings
```

---

## Developed By

**[ Your Full Name ]**
**Class / Semester:** [ e.g., BS-SE 6th Semester ]
**Department:** [ e.g., Department of Computer Science ]
**University:** [ e.g., University of Lahore ]

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/your-profile)

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  Made with ❤️ for academic excellence
</p>
