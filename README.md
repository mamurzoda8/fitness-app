# 🏋️‍♂️ Fitness App - Your Personal Fitness Companion

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" alt="Dart">
  <img src="https://img.shields.io/badge/Platform-iOS%20%7C%20Android-blue?style=for-the-badge" alt="Platform">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="License">
</p>

<p align="center">
  <b>A beautiful and modern Flutter application designed to help you achieve your fitness goals! 🚀</b>
</p>

## ✨ Features

- 🍎 **Personalized Diet Recommendations** - Get tailored diet suggestions based on your preferences
- 🔥 **Popular Workouts Collection** - Access curated list of effective training programs
- 🏷️ **Smart Categories** - Browse exercises by different categories
- 🔍 **Advanced Search** - Find meals and workouts quickly with intuitive search
- 🎨 **Beautiful UI** - Modern design with smooth gradients and SVG icons
- 📱 **Fully Responsive** - Optimized for both iOS and Android devices

## 🏗️ Project Structure

```
FITNESS_APP/
├── 📁 android/                 # Android platform-specific code
├── 📁 assets/                 # Resources folder
│   ├── 📁 icons/              # SVG icons for the app
│   └── 📁 fonts/              # Custom fonts (Poppins)
├── 📁 lib/                    # Main application code
│   ├── 📁 models/             # Data models
│   │   ├── 📄 category_models.dart
│   │   ├── 📄 diet_model.dart
│   │   └── 📄 popular_mode.dart
│   ├── 📁 pages/              # Application screens
│   │   ├── 📄 home.dart       # Main homepage
│   │   └── 📄 main.dart       # App entry point
│   └── 📁 widgets/            # Reusable UI components
├── 📄 pubspec.yaml            # Dependencies configuration
└── 📄 README.md               # Project documentation
```

## 🧩 Data Models

### 🍽️ DietModel
```dart
class DietModel {
  String name;           // Diet name (e.g., "Honey Pancake")
  String iconPath;       // SVG icon path
  String level;          // Difficulty level
  String duration;       // Preparation time
  String calorie;        // Calorie count
  bool viewIsSelected;   // Selection state
  Color boxColor;        // Background color
}
```

### ⭐ PopularDietsModel
```dart
class PopularDietsModel {
  String name;           // Diet name
  String iconPath;       // SVG icon path
  String level;          // Difficulty level
  String duration;       // Duration
  String calorie;        // Calorie information
  bool boxIsSelected;    // Selection state
}
```

### 📁 CategoryModel
```dart
class CategoryModel {
  String name;           // Category name
  String iconPath;       // Icon path
  Color boxColor;        // Background color
}
```

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (version 3.0+)
- Dart SDK (version 2.17+)
- Android Studio or VS Code

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/fitness-app.git
   cd fitness-app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the application**
   ```bash
   flutter run
   ```

## 📦 Dependencies

Add to your `pubspec.yaml`:

```yaml
dependencies:
  flutter:
    sdk: flutter
  flutter_svg: ^2.0.0+1  # For SVG icon support

dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^2.0.0
```

## 🎨 UI Overview

### Home Page Structure
- **App Bar**: Custom bar with navigation and menu buttons
- **Search Field**: With filter functionality and SVG icons
- **Categories Section**: Horizontal scrolling categories
- **Diet Recommendations**: Interactive diet cards with gradients
- **Popular Diets**: List view with selection states

### Design Features
- 🔹 Custom SVG icons throughout the app
- 🔹 Gradient buttons and selection effects
- 🔹 Poppins font family for modern typography
- 🔹 Soft shadows and smooth animations
- 🔹 Responsive card layouts

## 🛠️ Development Guide

### Adding New Diets
Edit `lib/models/diet_model.dart`:

```dart
diets.add(
  DietModel(
    name: 'New Diet Name',
    iconPath: 'assets/icons/new-icon.svg',
    level: 'Easy',
    duration: '25 mins',
    calorie: '200 kCal',
    viewIsSelected: false,
    boxColor: Color(0xffYOUR_COLOR),
  ),
);
```

### Adding New Categories
Modify the `getCategories()` method in `category_models.dart` to include new categories.

## 📱 Main Application Entry

```dart
void main() {
  WidgetsFlutterBinding.ensureInitialized();
  runApp(MainApp());
}

class MainApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      theme: ThemeData(fontFamily: 'Poppins'),
      home: HomePage(),  // Main homepage
    );
  }
}
```

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Icons designed by Freepik
- UI inspiration from modern fitness applications
- Flutter community for excellent support

## 📞 Support

If you need help:

1. Check the [Flutter documentation](https://flutter.dev/docs)
2. Open an issue on GitHub
3. Join our community Discord

---

<p align="center">
⭐ Don't forget to star this repository if you found it helpful! ⭐
</p>

<p align="center">
Made with ❤️ using Flutter & Dart
</p>
```