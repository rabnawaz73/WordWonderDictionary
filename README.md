# WordWonder - Build Vocabulary 📚✨

**WordWonder** is a feature-rich Flutter dictionary application designed to help users build their vocabulary. It provides instant access to word definitions, phonetics, synonyms, and examples, all wrapped in a modern, beautiful user interface.

## 🚀 Features

* **Comprehensive Dictionary Search**: Fetch detailed meanings, parts of speech, synonyms, and example sentences for thousands of words.
* **Search History**: Automatically saves your recently searched words so you can revisit them later. includes a feature to delete individual history items.
* **Audio/Phonetics**: (Supported by data model) Access phonetic text and audio links to learn correct pronunciation.
* **AdMob Integration**: 
    * **Banner Ads**: Integrated seamlessly into the main search screen.
    * **Native Ads**: Custom native ads displayed within the search history list.
* **Modern UI/UX**:
    * Beautiful gradient AppBar with decorative elements.
    * **Salomon Bottom Bar** for intuitive navigation between Search, History, and Answer screens.
    * Custom circular avatar and decorative dropdowns.
    * Smooth animations when loading results.
* **Cross-Platform**: Built for Android, iOS, Windows, and Web.

## 🛠️ Tech Stack & Dependencies

This project is built using **Flutter** and relies on several key packages:

* **[http](https://pub.dev/packages/http)**: For making API requests to fetch dictionary data.
* **[google_mobile_ads](https://pub.dev/packages/google_mobile_ads)**: For monetizing the app with Google AdMob (Banner & Native ads).
* **[salomon_bottom_bar](https://pub.dev/packages/salomon_bottom_bar)**: For the stylish bottom navigation bar.
* **[webview_windows](https://pub.dev/packages/webview_windows)** & **[window_manager](https://pub.dev/packages/window_manager)**: For Windows desktop support.
* **[google_fonts](https://pub.dev/packages/google_fonts)**: For custom typography.
* **[flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons)**: For managing app icons across platforms.

## 🌐 API Reference

WordWonder uses the free and open-source **Dictionary API** to fetch word data:
* **Endpoint**: `https://api.dictionaryapi.dev/api/v2/entries/en/<word>`

## 📸 Screenshots

| Home Screen | Search Results | History |
|:-![unnamed](https://github.com/user-attachments/assets/89ab5937-dc3d-4166-9048-4dddf1187d7b)
|:-![![unnamed (1)](https://github.com/user-attachments/assets/aec52e43-6c8c-4544-a1ae-027cb74c1d20)
unnamed (2)](https://github.com/user-attachments/assets/40b7ec34-3dcc-4f3c-baf7-36c974e58d5a)
--:|:-![unnamed (3)](https://github.com/user-attachments/assets/61c00464-b086-432e-9acf-d13b80b439bd)
--:|
| ![Home](assets/image.png) | | |

## ⚙️ Installation & Setup

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/rabnawaz73/wordwonderdictionary.git](https://github.com/rabnawaz73/wordwonderdictionary.git)
    ```

2.  **Install dependencies**:
    ```bash
    cd wordwonderdictionary
    flutter pub get
    ```

3.  **Run the app**:
    ```bash
    flutter run
    ```

## ⚠️ Configuration (AdMob)

The project is currently configured with hardcoded AdMob Unit IDs in `Search_Screen.dart` and `history.dart`. 

**Before publishing**, please replace the Test/Hardcoded IDs with your own production IDs from the Google AdMob console:

1.  **Banner Ad**: Update `adUnitId` in `lib/Screens/Search_Screen.dart`.
2.  **Native Ad**: Update `adUnitId` in `lib/Screens/history.dart`.

## 📂 Project Structure
lib/ ├── Models/ │ └── dictionary_model.dart # JSON serialization model for API response ├── Screens/ │ ├── Search_Screen.dart # Main search UI and logic │ ├── answer_Screen.dart # Displays detailed word results │ ├── history.dart # Displays search history list │ └── SplashScreen.dart # Initial splash screen ├── Services/ │ └── DicService.dart # HTTP service to fetch data from API ├── main.dart # App entry point and theme config └── custom_native_ad.dart # Widget for rendering Native Ads
## 👤 Author

**Rabnawaz**
* GitHub: [rabnawaz73](https://github.com/rabnawaz73)


