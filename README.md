<div align="center">

# 📚 Tutoria

### *Your Smart Learning Companion*

[![Android](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Language-Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![Firebase](https://img.shields.io/badge/Backend-Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Min SDK](https://img.shields.io/badge/Min%20SDK-28%20(Pie)-orange?style=for-the-badge)](https://developer.android.com/about/versions/pie)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

**Tutoria** is a modern Android application designed to connect learners with the knowledge they need — anytime, anywhere.

</div>

---

## 🌟 Overview

Tutoria is built from the ground up using **Jetpack Compose**, Android's modern declarative UI toolkit. At its core, the app aims to deliver a seamless learning experience — starting with a polished authentication flow featuring Google Sign-In and traditional credentials — with more features being actively developed.

---

## ✨ Features

| Feature | Status |
|---|---|
| 🔑 Login with Username & Password | ✅ Available |
| 🔒 Password Visibility Toggle | ✅ Available |
| 💾 Remember Me | ✅ Available |
| 🔗 Forgot Password | ✅ Available |
| 🌐 Continue with Google | ✅ Available |
| 📋 Sign-Up / Registration | 🚧 In Progress |
| 🌙 Dark / Light Theme Support | ✅ Available |
| 📱 Edge-to-Edge UI | ✅ Available |

---

## 🛠️ Tech Stack

### Language & UI
| Tool | Version | Purpose |
|---|---|---|
| [Kotlin](https://kotlinlang.org) | 2.0.0 | Primary programming language |
| [Jetpack Compose](https://developer.android.com/jetpack/compose) | BOM 2024.04.01 | Declarative, reactive UI framework |
| [Material Design 3](https://m3.material.io) | Latest | Design system & UI components |

### Android Jetpack
| Library | Purpose |
|---|---|
| `androidx.core:core-ktx` | Kotlin extensions for core Android APIs |
| `androidx.activity:activity-compose` | Compose integration with `ComponentActivity` |
| `androidx.lifecycle:lifecycle-runtime-ktx` | Lifecycle-aware coroutines & state management |

### Backend & Services
| Tool | Purpose |
|---|---|
| [Firebase](https://firebase.google.com) (BOM 33.10.0) | Backend platform — Authentication, Database, and more |

### Build & Tooling
| Tool | Version | Purpose |
|---|---|---|
| Android Gradle Plugin (AGP) | 8.8.0 | Build system for Android |
| Gradle Version Catalog (`libs.versions.toml`) | — | Centralized dependency management |
| ProGuard | — | Code shrinking & obfuscation for release builds |

---

## 🏗️ Project Architecture

Tutoria follows a clean, layered **Presentation-first** architecture, preparing the codebase to scale toward a full **MVVM (Model-View-ViewModel)** pattern.

```
app/
└── src/
    └── main/
        └── java/com/example/raionapp/
            ├── common/
            │   └── Resource.kt          # Sealed class for async state (Loading / Success / Error)
            └── presentation/
                ├── MainActivity.kt      # App entry point, hosts Compose content
                ├── register/
                │   └── LoginPage.kt     # Login & Sign-Up UI screen
                └── ui/
                    └── theme/
                        ├── Color.kt     # App-wide color palette
                        ├── Theme.kt     # MaterialTheme setup (dark/light/dynamic)
                        └── Type.kt      # Typography scale
```

### Key Design Decisions

- **`Resource<T>` Sealed Class** — A generic wrapper in `common/Resource.kt` that elegantly represents the three states of any async operation: `Loading`, `Success`, and `Error`. This is the foundation for handling network or database calls in a predictable, type-safe manner.

- **Declarative UI with Jetpack Compose** — Every screen is a `@Composable` function, making UI logic easy to read, preview, and test in isolation.

- **Dynamic Theming** — On Android 12+ (API 31+), the app automatically adapts to the user's system wallpaper colors via Material You dynamic theming. On older devices, a curated purple/pink palette is applied.

- **Edge-to-Edge Layout** — `enableEdgeToEdge()` is called in `MainActivity` so the app content extends under system bars for a truly immersive experience.

---

## 📱 Screens

### 🔐 Login Screen (`LoginPage.kt`)

The Login screen is built entirely with composable functions and handles user state via `remember { mutableStateOf(...) }`.

**Components used:**
- `Box` + `Column` — Layered layout with a floating card at the bottom
- `TextField` — Material3 styled inputs for Username and Password with custom colors
- `RoundedCornerShape` — Soft, card-like UI corners
- `Image` (vector drawables) — Branded visuals for labels, buttons, and dividers
- `Icon` — Checkbox for "Remember Me"
- `Button` — Transparent back navigation button with an icon
- Clickable `Text` — "Forgot Password?" action link in brand blue (`#1A5294`)

---

## 🚀 Getting Started

### Prerequisites

- **Android Studio** Hedgehog (2023.1.1) or newer
- **JDK 11** or higher
- **Android device or emulator** running Android 9 (API 28) or higher
- A **Firebase project** with a `google-services.json` file

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/alHerys/Tutoria.git
   cd Tutoria
   ```

2. **Add your Firebase configuration**

   Place your `google-services.json` file in the `app/` directory:
   ```
   app/google-services.json
   ```
   You can generate this file from the [Firebase Console](https://console.firebase.google.com).

3. **Open in Android Studio**

   Open the project root directory in Android Studio and let Gradle sync complete.

4. **Run the app**

   Select a device/emulator and click ▶ **Run**, or use:
   ```bash
   ./gradlew assembleDebug
   ```

---

## 📦 Build Variants

| Variant | Description |
|---|---|
| `debug` | Development build with full debugging tools |
| `release` | Optimized build with ProGuard rules applied |

---

## 🧪 Testing

The project includes scaffolded tests ready to be expanded:

| Test Type | Location | Tool |
|---|---|---|
| Unit Tests | `src/test/` | JUnit 4 |
| Instrumented Tests | `src/androidTest/` | Espresso + Compose UI Test |

Run all tests with:
```bash
./gradlew test                  # Unit tests
./gradlew connectedAndroidTest  # Instrumented tests
```

---

## 📂 Resources Overview

The `res/drawable/` folder contains a rich set of **vector assets** that form the visual identity of the app:

| Asset | Description |
|---|---|
| `logo_app` | Main application logo |
| `welcome_back` | Illustrated welcome graphic on the Login screen |
| `login_and_signup` | Tab/toggle graphic for Login and Sign-Up navigation |
| `log_in_button` | Branded primary login action button |
| `sign_up_button` | Branded sign-up action button |
| `continue_with_google` | Google OAuth sign-in button |
| `username_text` / `password_text` | Decorative field labels |
| `check_box_outline` | "Remember Me" checkbox icon |
| `arrow_back_button` | Back navigation icon |
| `or_line` | Visual divider between login methods |
| `no_look` | Password visibility toggle icon |
| `sign_up_screen_background` | Background image for the sign-up screen |

---

## 🎨 Theme & Design Language

Tutoria uses **Material Design 3** with a custom color palette:

| Token | Light | Dark |
|---|---|---|
| Primary | `Purple40` (`#6650A4`) | `Purple80` (`#D0BCFF`) |
| Secondary | `PurpleGrey40` (`#625B71`) | `PurpleGrey80` (`#CCC2DC`) |
| Tertiary | `Pink40` (`#7D5260`) | `Pink80` (`#EFB8C8`) |

**Dynamic Color** (Material You) is enabled by default on Android 12+, automatically pulling colors from the user's wallpaper for a personalized experience.

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/my-new-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

Made with ❤️ using **Jetpack Compose** & **Firebase**

</div>
