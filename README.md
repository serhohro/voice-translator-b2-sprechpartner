# Voice Translator (Android) & B2 Sprechpartner

A unique Android application designed for quick voice translation, as well as for practicing conversational German and preparing for the oral part of the Goethe B2 exam.

## 🚀 Features
*   **🎤 Voice Translator:** Real-time two-way voice translation between Ukrainian and German.
*   **🎓 AI B2 Examiner:** A live conversation with Artificial Intelligence playing the role of a Goethe B2 examiner. Includes three scenarios: *Selbstpräsentation*, *Diskussion*, and *Gemeinsame Planung*. The AI responds in German, asks questions, and gently points out mistakes.
*   **🔄 Dual AI System (Gemini + Groq):** The app uses Google Gemini as the primary AI, but automatically falls back to Groq (Llama 3.3) if the Gemini API rate limit is exceeded (Error 429) or the server is unavailable (Error 503). This ensures 100% uninterrupted operation.
*   **🔊 Text-to-Speech (TTS):** Utilizes the native Android Text-to-Speech engine to voice translations and examiner responses.
*   **🔑 Bring Your Own Key (BYOK):** The app runs on your own free Gemini and Groq API keys. No paid subscriptions required.

## 🛠️ Technologies Used
*   **Language:** Kotlin
*   **UI:** Jetpack Compose (WebView integration)
*   **AI Models:** Google Gemini API (`gemini-2.5-flash`) & Groq API (`llama-3.3-70b-versatile`)
*   **Bridge:** HTML/CSS/JS for the UI, integrated via `@JavascriptInterface` to access the device's microphone and TTS engine.

## ⚙️ How to Run

**Option 1: Use the ready-to-install APK (For regular users)**
If you just want to use the app and don't want to build it yourself, you can download the ready-to-install APK file directly from the [Releases](https://github.com/serhohro/voice-translator-b2-sprechpartner/releases) section. Just download the `.apk` file, transfer it to your Android phone, and install it (allow installation from unknown sources if prompted).

**Option 2: Build from source (For developers)**
1. Clone this repository.
2. Open the project in Android Studio.
3. **Note:** The project includes both Gradle wrapper scripts (`gradlew` for macOS/Linux and `gradlew.bat` for Windows). Android Studio will automatically use the correct one for your operating system.
4. Build the APK (`Build -> Build Bundle(s) / APK(s) -> Build APK(s)`).
5. Install the app on your Android device.
6. Get a free Gemini API key from [Google AI Studio](https://aistudio.google.com/) and a free Groq API key from [Groq Console](https://console.groq.com/). Paste both keys into the app's input fields.

## 🔒 Security Note
The application does not store your API keys on any external server. The keys are saved locally in your device's memory (`localStorage`) and are only used to make direct requests to the respective AI APIs.

## 📄 License
This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for details.

---

# Sprachübersetzer (Android) & B2 Sprechpartner

Eine einzigartige Android-Anwendung für schnelle Sprachübersetzung sowie für die Übung der deutschen Konversation und die Vorbereitung auf den mündlichen Teil der Goethe-Prüfung B2.

## 🚀 Funktionen
*   **🎤 Sprachübersetzer:** Echtzeit-Zweiweg-Sprachübersetzung zwischen Ukrainisch und Deutsch.
*   **🎓 KI B2-Prüfer:** Ein Live-Gespräch mit Künstlicher Intelligenz, die die Rolle eines Goethe B2-Prüfers spielt. Beinhaltet drei Szenarien: *Selbstpräsentation*, *Diskussion* und *Gemeinsame Planung*. Die KI antwortet auf Deutsch, stellt Fragen und weist höflich auf Fehler hin.
*   **🔄 Duales KI-System (Gemini + Groq):** Die App verwendet Google Gemini als primäre KI, wechselt aber automatisch zu Groq (Llama 3.3), wenn das Gemini-API-Limit überschritten wird (Fehler 429) oder der Server nicht verfügbar ist (Fehler 503).
*   **🔊 Text-to-Speech (TTS):** Nutzt die native Android-TTS-Engine zur Sprachausgabe von Übersetzungen und Antworten.
*   **🔑 Eigener API-Schlüssel:** Die App läuft mit Ihren eigenen kostenlosen Gemini- und Groq-API-Schlüsseln. Keine Abonnements erforderlich.

## ⚙️ Wie man es startet

**Option 1: Fertige APK verwenden (Für normale Nutzer)**
Wenn Sie die App nur nutzen und nicht selbst erstellen möchten, können Sie die fertige APK-Datei direkt im Bereich [Releases](https://github.com/serhohro/voice-translator-b2-sprechpartner/releases) herunterladen. Laden Sie einfach die `.apk`-Datei herunter, übertragen Sie sie auf Ihr Android-Smartphone und installieren Sie sie (erlauben Sie bei Aufforderung die Installation aus unbekannten Quellen).

**Option 2: Aus dem Quellcode erstellen (Für Entwickler)**
1. Klonen Sie dieses Repository.
2. Öffnen Sie das Projekt in Android Studio.
3. **Hinweis:** Das Projekt enthält sowohl Gradle-Wrapper-Skripte (`gradlew` für macOS/Linux als auch `gradlew.bat` für Windows). Android Studio verwendet automatisch die richtige Version für Ihr Betriebssystem.
4. Bauen Sie die APK (`Build -> Build Bundle(s) / APK(s) -> Build APK(s)`).
5. Installieren Sie die App auf Ihrem Android-Gerät.
6. Holen Sie sich einen kostenlosen Gemini API-Schlüssel von [Google AI Studio](https://aistudio.google.com/) und einen kostenlosen Groq API-Schlüssel von [Groq Console](https://console.groq.com/). Fügen Sie beide Schlüssel in die Eingabefelder der App ein.

## 🔒 Sicherheit
Die Anwendung speichert Ihre API-Schlüssel nicht auf einem externen Server. Die Schlüssel werden lokal im Speicher Ihres Geräts (`localStorage`) gespeichert und nur für direkte Anfragen an die jeweiligen KI-APIs verwendet.

## 📄 Lizenz
Dieses Projekt ist unter der **Apache License 2.0** lizenziert. Weitere Informationen finden Sie in der Datei [LICENSE](LICENSE).

---

# Голосовий перекладач (Android) & B2 Sprechpartner

Унікальний Android-додаток, створений для швидкого голосового перекладу, а також для практики розмовної німецької мови та підготовки до усної частини іспиту Goethe B2.

## 🚀 Функції
*   **🎤 Голосовий перекладач:** Двосторонній голосовий переклад у реальному часі між українською та німецькою мовами.
*   **🎓 AI-екзаменатор B2:** Живий діалог зі штучним інтелектом, який грає роль екзаменатора Goethe B2. Включає три сценарії: *Selbstpräsentation* (Самопрезентація), *Diskussion* (Дискусія) та *Gemeinsame Planung* (Спільне планування). ШІ відповідає німецькою, ставить питання та делікатно вказує на помилки.
*   **🔄 Подвійна система ШІ (Gemini + Groq):** Додаток використовує Google Gemini як основний ШІ, але автоматично перемикається на Groq (Llama 3.3), якщо ліміт запитів Gemini вичерпано (Помилка 429) або сервер недоступний (Помилка 503). Це забезпечує 100% безперебійну роботу.
*   **🔊 Озвучення (TTS):** Використання нативного Android-синтезатора мовлення для озвучення перекладів та відповідей екзаменатора.
*   **🔑 Власний API-ключ:** Додаток працює на ваших безкоштовних ключах Gemini та Groq. Жодних платних підписок.

## 🛠️ Використані технології
*   **Мова:** Kotlin
*   **Інтерфейс:** Jetpack Compose (інтеграція WebView)
*   **ШІ-моделі:** Google Gemini API (`gemini-2.5-flash`) та Groq API (`llama-3.3-70b-versatile`)
*   **Місток:** HTML/CSS/JS для інтерфейсу, інтегрований через `@JavascriptInterface` для доступу до мікрофона пристрою та двигуна TTS.

## ⚙️ Як запустити

**Варіант 1: Використати готовий APK (Для звичайних користувачів)**
Якщо ви просто хочете користуватися додатком і не бажаєте збирати його самостійно, ви можете завантажити готовий APK-файл прямо з розділу [Releases](https://github.com/serhohro/voice-translator-b2-sprechpartner/releases). Просто завантажте файл `.apk`, перенесіть його на свій Android-телефон і встановіть (дозвольте встановлення з невідомих джерел, якщо з'явиться запит).

**Варіант 2: Збірка з вихідного коду (Для розробників)**
1. Клонуйте цей репозиторій.
2. Відкрийте проєкт в Android Studio.
3. **Примітка:** Проєкт містить обидва скрипти Gradle (`gradlew` для macOS/Linux та `gradlew.bat` для Windows). Android Studio автоматично використає правильний варіант для вашої операційної системи.
4. Зберіть APK (`Build -> Build Bundle(s) / APK(s) -> Build APK(s)`).
5. Встановіть додаток на ваш Android-пристрій.
6. Отримайте безкоштовний API-ключ Gemini на [Google AI Studio](https://aistudio.google.com/) та безкоштовний ключ Groq на [Groq Console](https://console.groq.com/). Вставте обидва ключі у відповідні поля в додатку.

## 🔒 Безпека
Додаток не зберігає ваші API-ключі на зовнішніх серверах. Ключі зберігаються локально в пам'яті вашого пристрою (`localStorage`) і використовуються лише для прямих запитів до відповідних ШІ-сервісів.

## 📄 Ліцензія
Цей проєкт ліцензовано відповідно до **Apache License 2.0**. Деталі дивіться у файлі [LICENSE](LICENSE).
