# 📰 NY Times Most Popular Articles App  
A Flutter application by **Mariam Alahmar** to fetch and display the most popular articles from The New York Times.

---

## 📌 Overview

This Flutter app fetches the most viewed articles from The New York Times using their **Most Popular Articles API**. It follows a **Clean Architecture** and supports **mobile** and **web** platforms. The goal is to build maintainable, testable, and scalable software using best practices.

---

## ✨ Features

- 📃 **List View**: Displays a list of popular NYT articles.
- 🔍 **Detail View**: Tap to view the full article details.
- 💻📱 **Responsive UI**: Optimized for both web and mobile.
- 🔌 **API Integration**: Powered by NYT’s official API.
- 🧱 **Clean Architecture**: Built with BLoC + GetIt for separation of concerns.
- 🧪 **Unit Testing**: Code tested for reliability and coverage.
- 🛡️ **Error Handling**: Gracefully handles API/data failures.

---

## 🧰 Prerequisites

- [Flutter SDK](https://flutter.dev/docs/get-started/install)
- [NYT API Key](https://developer.nytimes.com/get-started)

---

## 🚀 Getting Started

### 🧬 Installation

```bash
git clone https://github.com/your-username/nytimes-most-popular-articles.git
cd nytimes-most-popular-articles
flutter pub get
flutter pub run build_runner build # If using JSON serialization
```

### 🔑 API Key Setup

Replace `sample-key` in the API URL with your real key inside the project files.

### ▶️ Run the App

- **On Mobile**:
```bash
flutter run
```
- **On Web**:
```bash
flutter run -d chrome
```

---

## 🗂 Project Structure

```
lib/
│
├── core/         # Constants, utilities, base widgets
├── data/         # API integration, models
├── domain/       # Use cases, entities
├── presentation/ # Screens, BLoC, widgets
└── di/           # Dependency Injection (GetIt)
```

---

## ⚙️ Architecture

This app follows the **Clean Architecture** model:

- **Presentation Layer**: Screens, widgets, and BLoCs
- **Domain Layer**: Core business logic and entities
- **Data Layer**: Network/API logic and model mapping

### 📦 State Management

- **BLoC**: Used for predictable state handling.

### 💉 Dependency Injection

- **GetIt**: Enables decoupled and testable architecture.

---

## 🧪 Testing

Run tests using:

```bash
flutter test
```

You can also generate **code coverage** reports for quality checks.

---

## 🔗 API Integration

**Endpoint used**:  
```
https://api.nytimes.com/svc/mostpopular/v2/mostviewed/all-sections/30.json?api-key=YOUR_KEY
```

- `Section`: all-sections  
- `Period`: 30 days  
- `API Key`: Replace `YOUR_KEY` with your key.

---

## 🛠 Deployment

To build for web:

```bash
flutter build web
```

Files will be in the `/build/web` directory.

---

## 📈 Future Improvements

- 🔍 Add integration (end-to-end) tests
- 🧠 Smarter error handling
- 💾 Add caching for offline mode

---

## 👩‍💻 Author

**Mariam Alahmar**  
_Software Engineer passionate about product thinking and real-world apps._

---

## 📜 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file.

---

## 🙏 Acknowledgments

Special thanks to [The New York Times](https://developer.nytimes.com/) for the open API.
