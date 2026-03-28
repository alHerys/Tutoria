<div align="center">

# 📚 Tutoria

### *Your Smart Learning Companion*

[![Android](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Language-Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![Firebase](https://img.shields.io/badge/Backend-Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Supabase](https://img.shields.io/badge/Storage-Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)](https://supabase.com)
[![Min SDK](https://img.shields.io/badge/Min%20SDK-28%20(Pie)-orange?style=for-the-badge)](https://developer.android.com/about/versions/pie)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

**Tutoria** is a modern Android application designed to connect learners with the knowledge they need — anytime, anywhere. It features a full learning platform with courses, video lessons, a question bank, a community discussion forum, and a mentorship system.

</div>

---

## 🌟 Overview

Tutoria is built from the ground up using **Jetpack Compose**, Android's modern declarative UI toolkit. The app delivers a complete learning experience — from authentication with Google Sign-In and email/password, through browsing and enrolling in courses organized by subject and semester, to a mentorship system where educators can create and publish their own classes.

---

## ✨ Features

| Feature | Status |
|---|---|
| 🔑 Login with Email & Password | ✅ Available |
| 📋 Sign-Up / Registration | ✅ Available |
| 🌐 Continue with Google | ✅ Available |
| 🔗 Forgot Password & Email Verification | ✅ Available |
| 🏠 Home Page with Community Forum (Threads) | ✅ Available |
| 💬 Thread Comments & Replies | ✅ Available |
| 📚 Learning Page (Browse Lessons by Subject & Semester) | ✅ Available |
| 🎬 Video Lessons (ExoPlayer / Media3) | ✅ Available |
| 📄 File & PDF Viewer | ✅ Available |
| 🗂️ Question Bank (Bank Soal) | ✅ Available |
| 👤 User Profile & About Page | ✅ Available |
| 🧑‍🏫 Become a Mentor / Mentor Registration | ✅ Available |
| 🏫 My Course (Mentor Course Management) | ✅ Available |
| ➕ Create New Class & Sub-Lessons | ✅ Available |
| 💳 Payment Overview | ✅ Available |
| 💾 Saved Answers | ✅ Available |
| 🌙 Dark / Light Theme Support | ✅ Available |
| 📱 Edge-to-Edge UI | ✅ Available |
| ✨ Splash Screen | ✅ Available |

---

## 🛠️ Tech Stack

### Language & UI
| Tool | Version | Purpose |
|---|---|---|
| [Kotlin](https://kotlinlang.org) | 2.0.0 | Primary programming language |
| [Jetpack Compose](https://developer.android.com/jetpack/compose) | BOM 2024.04.01 | Declarative, reactive UI framework |
| [Material Design 3](https://m3.material.io) | Latest | Design system & UI components |
| [Material Icons Extended](https://developer.android.com/reference/kotlin/androidx/compose/material/icons/package-summary) | 1.7.8 | Extended icon set for Compose |
| [Coil](https://coil-kt.github.io/coil/) | 2.2.2 | Async image loading for Compose |
| [Google Fonts (Compose)](https://developer.android.com/jetpack/compose/text/fonts) | 1.0.0 | Downloadable fonts (Montserrat) |

### Android Jetpack
| Library | Version | Purpose |
|---|---|---|
| `androidx.core:core-ktx` | 1.15.0 | Kotlin extensions for core Android APIs |
| `androidx.activity:activity-compose` | 1.10.0 | Compose integration with `ComponentActivity` |
| `androidx.lifecycle:lifecycle-runtime-ktx` | 2.8.7 | Lifecycle-aware coroutines & state management |
| `androidx.navigation:navigation-compose` | 2.8.8 | Type-safe in-app navigation |
| `androidx.compose.runtime:runtime-livedata` | 1.7.8 | `observeAsState()` for LiveData in Compose |
| `androidx.core:core-splashscreen` | 1.2.0-beta01 | Splash screen API |

### Dependency Injection
| Library | Version | Purpose |
|---|---|---|
| [Dagger-Hilt](https://dagger.dev/hilt/) | 2.51.1 | Compile-time dependency injection |
| `androidx.hilt:hilt-navigation-compose` | 1.2.0 | Hilt integration with Navigation Compose |

### Media
| Library | Version | Purpose |
|---|---|---|
| [Media3 ExoPlayer](https://developer.android.com/media/media3/exoplayer) | 1.5.1 | Video playback |
| `media3-exoplayer-dash` | 1.5.1 | DASH adaptive streaming support |
| `media3-ui` | 1.5.1 | Pre-built player UI components |

### Backend & Services
| Tool | Version | Purpose |
|---|---|---|
| [Firebase](https://firebase.google.com) | BOM 33.10.0 | Authentication & Firestore database |
| [Firebase Firestore](https://firebase.google.com/docs/firestore) | 25.1.2 | NoSQL cloud database |
| [Google Play Services Auth](https://developers.google.com/identity/sign-in/android) | 21.2.0 | Google Sign-In |
| [Credential Manager](https://developer.android.com/identity/sign-in/credential-manager) | 1.5.0-rc01 | Modern credential/sign-in API |
| [Google Identity](https://developers.google.com/identity) | 1.1.1 | Google ID token for Credential Manager |
| [Supabase](https://supabase.com) | BOM 1.4.1 | File & media storage |
| [Supabase Storage-kt](https://github.com/supabase-community/supabase-kt) | via BOM | Kotlin client for Supabase Storage |
| [Supabase PostgREST-kt](https://github.com/supabase-community/supabase-kt) | via BOM | Kotlin client for PostgREST |
| [Ktor Client Android](https://ktor.io/docs/client-create-new-application.html) | 3.1.1 | HTTP client engine for Supabase |

### Networking & Serialization
| Library | Version | Purpose |
|---|---|---|
| [OkHttp](https://square.github.io/okhttp/) | 4.12.0 | HTTP client for file uploads |
| [Okio](https://square.github.io/okio/) | 3.8.0 | I/O operations |
| [Kotlin Serialization](https://github.com/Kotlin/kotlinx.serialization) | 2.1.0 | JSON serialization |

### Build & Tooling
| Tool | Version | Purpose |
|---|---|---|
| Android Gradle Plugin (AGP) | 8.8.0 | Build system for Android |
| Gradle Version Catalog (`libs.versions.toml`) | — | Centralized dependency management |
| ProGuard | — | Code shrinking & obfuscation for release builds |

---

## 🏗️ Project Architecture

Tutoria follows a full **MVVM (Model-View-ViewModel)** architecture with a clean, layered package structure.

```
app/
└── src/
    └── main/
        └── java/com/example/raionapp/
            ├── common/
            │   └── Resource.kt                    # Sealed class: Loading / Success / Error
            ├── exoPlayer/
            │   ├── Media3AndroidView.kt            # AndroidView wrapper for ExoPlayer
            │   ├── Media3PlayerView.kt             # Composable player surface
            │   └── PlayerViewModel.kt             # ViewModel for media playback state
            ├── firestore/
            │   ├── CommentCollection.kt            # Firestore: thread comments
            │   ├── LessonCollection.kt             # Firestore: lessons & sub-lessons
            │   ├── ProfileCollection.kt            # Firestore: user profiles
            │   ├── SavedCollection.kt              # Firestore: saved answers
            │   ├── ThreadCollection.kt             # Firestore: forum threads
            │   └── model/
            │       ├── CommentDataClass.kt
            │       ├── LessonDataClass.kt
            │       ├── MentorshipDataClass.kt
            │       ├── ProfileDataClass.kt
            │       ├── SublessonDataClass.kt
            │       └── ThreadDataClass.kt
            ├── mentorship/
            │   ├── CreateNewClassPage.kt           # Mentor: create a new class
            │   ├── CreateNewSubLessonPage.kt       # Mentor: add sub-lesson (video/file)
            │   ├── MyCoursePageViewModel.kt
            │   └── myCoursePage.kt                 # Mentor's course management dashboard
            ├── pdfRender/
            │   ├── PdfBitmapConverter.kt           # Renders PDF pages to bitmaps
            │   ├── PdfPage.kt                      # Single PDF page composable
            │   ├── PdfScreen.kt                    # Full PDF viewer screen
            │   ├── PdfViewerScreen.kt
            │   └── SearchResult.kt
            ├── presentation/
            │   ├── AppNavHost.kt                   # Central navigation graph
            │   ├── MainActivity.kt                 # App entry point
            │   ├── homePage/
            │   │   ├── HomePageScreen.kt           # Main home/forum screen
            │   │   ├── NavBar.kt                   # Bottom navigation bar
            │   │   ├── TopBarAndProfile.kt
            │   │   ├── threadDataSync.kt
            │   │   ├── bankPage/
            │   │   │   ├── BankPageHome.kt         # Question bank home
            │   │   │   ├── BankPageContent.kt
            │   │   │   ├── bankList.kt
            │   │   │   └── bankListContent.kt
            │   │   ├── comments/
            │   │   │   ├── ThreadComment.kt        # View thread comments
            │   │   │   ├── ThreadCommentAdd.kt     # Add a comment
            │   │   │   └── ThreadCommentSub.kt
            │   │   ├── learningPage/
            │   │   │   ├── LearningPageHome.kt     # Browse all lessons
            │   │   │   ├── LearningContent.kt
            │   │   │   ├── LearningContentRow.kt
            │   │   │   └── LessonPages/
            │   │   │       ├── AboutPage.kt        # Lesson about/details
            │   │   │       ├── LessonPage.kt       # Lesson overview
            │   │   │       ├── ReviewPage.kt       # Lesson reviews
            │   │   │       ├── ReviewPageBox.kt
            │   │   │       ├── SubLessonLocked.kt  # Locked sub-lesson placeholder
            │   │   │       └── lessonPageUnlocked/
            │   │   │           ├── lessonPageUnlocked.kt       # Unlocked lesson home
            │   │   │           ├── lessonPageUnlockedMaterial.kt
            │   │   │           ├── videoListPage.kt            # List of video sub-lessons
            │   │   │           ├── videoListPageContent.kt
            │   │   │           ├── videoPage.kt                # Video player screen
            │   │   │           ├── videoPracticeListPage.kt    # Practice videos
            │   │   │           ├── videoPracticeListPageContent.kt
            │   │   │           ├── modulListPage.kt            # Module/file list
            │   │   │           ├── modulListPageContent.kt
            │   │   │           ├── filePage.kt                 # File viewer
            │   │   │           ├── chatWithMentorPage.kt       # Chat with mentor
            │   │   │           ├── chatBubbleMentor.kt
            │   │   │           ├── chatBubbleUser.kt
            │   │   │           └── paymentOverview.kt          # Payment screen
            │   │   ├── model/
            │   │   │   ├── HomeViewModel.kt
            │   │   │   ├── LearningPageViewModel.kt
            │   │   │   ├── CommentViewModel.kt
            │   │   │   ├── ImagePickerHandler.kt
            │   │   │   └── profileData.kt
            │   │   ├── semesterSelect/
            │   │   │   ├── semesterSelectPage.kt
            │   │   │   └── semesterSelectButton.kt
            │   │   ├── subjectSelect/
            │   │   │   ├── subjectSelectPage.kt
            │   │   │   └── subjectSelectButton.kt
            │   │   └── threads/
            │   │       ├── AddThreadPage.kt        # Create a new forum thread
            │   │       └── ThreadContent.kt        # Thread list item
            │   ├── profile/
            │   │   ├── ProfilePage.kt              # User profile
            │   │   ├── aboutProfilePage.kt
            │   │   ├── becomeAMentorPage.kt        # Mentor onboarding
            │   │   ├── mentorRegistration.kt       # Mentor registration form
            │   │   ├── SavedAnswersPage.kt         # Saved question bank answers
            │   │   ├── AnswersBox.kt
            │   │   └── postedQuestionsPage.kt      # User's posted questions
            │   ├── register/
            │   │   ├── LoginPage.kt                # Login screen
            │   │   ├── SignUpPage.kt               # Registration screen
            │   │   ├── AuthViewModel.kt            # Auth state management
            │   │   ├── AuthState.kt                # Sealed auth state class
            │   │   └── nantiAja/
            │   │       ├── ForgotPassword.kt       # Forgot password screen
            │   │       └── VerifyPassPage.kt       # Email verification screen
            │   └── ui/theme/
            │       ├── Color.kt
            │       ├── Theme.kt
            │       └── Type.kt
            └── supabase/
                └── SupabaseStorageCollection.kt    # Supabase file upload/download
```

### Key Design Decisions

- **MVVM Architecture** — ViewModels (`HomeViewModel`, `LearningPageViewModel`, `AuthViewModel`, `PlayerViewModel`, `MyCoursePageViewModel`) manage UI state and business logic, keeping Composables clean and testable.

- **`Resource<T>` Sealed Class** — A generic wrapper in `common/Resource.kt` that represents the three states of any async operation: `Loading`, `Success`, and `Error`, ensuring type-safe, predictable data flow.

- **Dagger-Hilt Dependency Injection** — Hilt is used for compile-time DI, wiring ViewModels, repositories, and services without boilerplate.

- **Centralized Navigation** — `AppNavHost.kt` defines the entire navigation graph in one place using Jetpack Navigation Compose, with type-safe route arguments.

- **Dual Backend** — Firebase handles authentication and the Firestore NoSQL database (threads, lessons, profiles, comments). Supabase handles media/file storage (video uploads, PDF uploads) via `SupabaseStorageCollection`.

- **Declarative UI with Jetpack Compose** — Every screen is a `@Composable` function, making UI logic easy to read, preview, and test in isolation.

- **Dynamic Theming** — On Android 12+ (API 31+), the app adapts to the user's system wallpaper colors via Material You dynamic theming. On older devices, a curated blue-based palette is applied.

- **Edge-to-Edge Layout** — `enableEdgeToEdge()` is called in `MainActivity` so app content extends under system bars for an immersive experience.

---

## 📱 Screens

### 🔐 Authentication Screens
- **Login Screen** (`LoginPage.kt`) — Email/password login, Google Sign-In via Credential Manager, "Forgot Password?" link.
- **Sign-Up Screen** (`SignUpPage.kt`) — Full name, username, email, password registration with client-side validation (min 6 chars). Also supports Google Sign-In.
- **Forgot Password Screen** (`ForgotPassword.kt`) — Enter email to receive a password reset link.
- **Verify Screen** (`VerifyPassPage.kt`) — Email verification code entry.

### 🏠 Home Screen (`HomePageScreen.kt`)
The main hub after login. Displays a community forum feed of threads. Users can create new threads via the floating action button. Bottom navigation provides access to Learning, Bank, and Profile sections.

### 📚 Learning Page
- **Learning Page Home** (`LearningPageHome.kt`) — Browse available lessons filtered by subject and semester.
- **Subject / Semester Select** — Filter screens for choosing a subject or semester.
- **Lesson Page** (`LessonPage.kt`) — Lesson overview with instructor info and sub-lesson list.
- **About Page** (`AboutPage.kt`) — Detailed lesson description.
- **Review Page** (`ReviewPage.kt`) — User ratings and reviews for a lesson.
- **Lesson Page Unlocked** (`lessonPageUnlocked.kt`) — Full lesson access after enrollment:
  - **Video List** — Browse and play video lessons via ExoPlayer.
  - **Practice Video List** — Practice/exercise video content.
  - **Module List** — Browse and view downloadable file modules.
  - **File/PDF Viewer** — In-app PDF viewer rendered page-by-page.
  - **Chat with Mentor** (`chatWithMentorPage.kt`) — Direct messaging with the lesson's mentor.
  - **Payment Overview** — Enrollment/payment details screen.

### 🗂️ Question Bank (`BankPageHome.kt`)
Browse and answer questions from the question bank, organized by category. Users can save answers to their profile.

### 💬 Forum & Comments
- **Add Thread** (`AddThreadPage.kt`) — Create a new discussion thread.
- **Thread Comments** (`ThreadComment.kt`) — View comments on a thread.
- **Add Comment** (`ThreadCommentAdd.kt`) — Post a reply to a thread.

### 👤 Profile
- **Profile Page** (`ProfilePage.kt`) — View and edit user profile with profile picture upload.
- **About Profile Page** (`aboutProfilePage.kt`) — Extended personal info.
- **Saved Answers** (`SavedAnswersPage.kt`) — Revisit saved question bank answers.
- **Posted Questions** (`postedQuestionsPage.kt`) — View questions the user has posted.
- **Become a Mentor** (`becomeAMentorPage.kt`) — Onboarding flow for becoming a mentor.
- **Mentor Registration** (`mentorRegistration.kt`) — Mentor application form.

### 🧑‍🏫 Mentorship (Mentor-only)
- **My Course** (`myCoursePage.kt`) — Dashboard for managing published courses.
- **Create New Class** (`CreateNewClassPage.kt`) — Add a new course/lesson.
- **Create New Sub-Lesson** (`CreateNewSubLessonPage.kt`) — Upload videos or files as sub-lessons.

---

## 🚀 Getting Started

### Prerequisites

- **Android Studio** Hedgehog (2023.1.1) or newer
- **JDK 11** or higher
- **Android device or emulator** running Android 9 (API 28) or higher
- A **Firebase project** with Authentication and Firestore enabled, and a `google-services.json` file
- A **Supabase project** with a storage bucket configured

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

3. **Configure Supabase**

   The demo project ships with a Supabase URL and anon key already configured in `SupabaseStorageCollection.kt`. If you are forking this project and setting up your own Supabase backend, replace those values with your own project credentials from the [Supabase Dashboard](https://supabase.com/dashboard). For production use, consider storing credentials in `local.properties` and reading them via the build config rather than hardcoding them in source files.

4. **Open in Android Studio**

   Open the project root directory in Android Studio and let Gradle sync complete.

5. **Run the app**

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
| `app_logo` | Main application logo |
| `splashscreenpng` | Splash screen background image |
| `login_and_signup` | Tab/toggle graphic for Login and Sign-Up navigation |
| `log_in_button` | Branded primary login action button |
| `continue_with_google` | Google OAuth sign-in button |
| `or_line` | Visual divider between login methods |
| `check_box_outline` | "Remember Me" checkbox icon |
| `back_button` / `left_arrow_icon` | Back navigation icons |
| `password_not_visible` / `password_visible` | Password visibility toggle icons |
| `sign_up_screen_background` | Background image for the sign-up screen |
| `home_icon_clicked` / `home_icon_unclicked` | Bottom nav: Home |
| `learn_icon_clicked` / `learn_icon_unclicked` | Bottom nav: Learning |
| `bank_soal_icon_clicked` / `bank_soal_icon_unclicked` | Bottom nav: Question Bank |
| `profile_icon_clicked` / `profile_icon_unclicked` | Bottom nav: Profile |
| `navbar_container` / `navbar_small_circle` | Bottom navigation bar assets |
| `logo_tutoria_header` | Header logo |
| `heading_background` | Heading section background |
| `default_profile_picture` | Placeholder profile avatar |
| `mentor_icon_human` | Mentor icon |
| `lesson_icon_book` | Lesson/book icon |
| `video_icon_sublesson` / `file_icon_sublesson` / `video_practice_icon_sublesson` | Sub-lesson type icons |
| `play_circle_icon` | Video play button |
| `time_icon_clock` | Duration/time icon |
| `upload_file_icon` | File upload icon |
| `cloud_saved_answer` | Saved answer indicator |
| `mentorship_icon` | Mentorship feature icon |
| `faq_icon` | FAQ icon |
| `log_out_icon` | Logout icon |

---

## 🎨 Theme & Design Language

Tutoria uses **Material Design 3** with a custom color palette. The MaterialTheme tokens use a purple/pink palette, while the brand blue (`#1A5294`) is used as a direct color accent in UI components such as buttons and links:

| Token | Light | Dark |
|---|---|---|
| Primary | `Purple40` (`#6650A4`) | `Purple80` (`#D0BCFF`) |
| Secondary | `PurpleGrey40` (`#625B71`) | `PurpleGrey80` (`#CCC2DC`) |
| Tertiary | `Pink40` (`#7D5260`) | `Pink80` (`#EFB8C8`) |
| Brand Blue (UI accent) | `#1A5294` | `#1A5294` |

**Dynamic Color** (Material You) is enabled by default on Android 12+, automatically pulling colors from the user's wallpaper for a personalized experience.

**Typography** uses the **Montserrat** font family, loaded from local resources (`res/font/montserrat.ttf`, `montserrat_italic.ttf`).

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

Made with ❤️ using **Jetpack Compose**, **Firebase** & **Supabase**

</div>
