# Health Tracker App UI By Engr. Hamid Raza

A comprehensive health and fitness tracking application built with Flutter and GetX state management.

## Demo & Download

### 📱 Demo Video
Watch the app in action:
[![Watch Demo Video](https://img.shields.io/badge/Watch-Demo%20Video-red?style=for-the-badge&logo=youtube)](https://drive.google.com/file/d/1amUU_A8bIrqjy8pkHr34kqJ43Z3yPR7Y/view)

### 📲 Download APK
Download the latest APK file:
[![Download APK](https://img.shields.io/badge/Download-APK-green?style=for-the-badge&logo=android)](https://github.com/Hamid-Raza-22/HealthTrackerApp/blob/main/Health%20App%20By%20Hamid.apk)

### 📸 App Screenshots
**Home Screen**
![Home Screen](https://github.com/Hamid-Raza-22/HealthTrackerApp/blob/main/Home%20Screen.png)

**Calendar Screen**
![Calendar Screen](https://github.com/Hamid-Raza-22/HealthTrackerApp/blob/main/Calender%20Screen.png)

**Training Calendar Screen**
![Training Calendar Screen](https://github.com/Hamid-Raza-22/HealthTrackerApp/blob/main/Training%20Calender%20Screen.png)

**Mood Screen**
![Mood Screen](https://github.com/Hamid-Raza-22/HealthTrackerApp/blob/main/Mood%20Screen.png)


## Features

- **Home Screen**: Track calories, weight, and hydration with interactive widgets
- **Mood Tracking**: Visual mood ring selector with emotional state tracking
- **Training Calendar**: Weekly workout planning and scheduling
- **Theme Switching**: Professional light/dark mode with smooth transitions
- **Responsive UI**: Pixel-perfect design matching Figma specifications

## Tech Stack

- **Framework**: Flutter 3.x
- **State Management**: GetX (exclusive use, no setState)
- **Architecture**: Clean Architecture with separation of concerns
- **Navigation**: GetX Navigation
- **Fonts**: Mulish (Google Fonts)
- **Dependencies**:
  - `get`: State management and navigation
  - `google_fonts`: Typography
  - `flutter_svg`: SVG assets
  - `http`: API calls

## Project Structure

```
lib/
├── core/
│   ├── constants/
│   │   └── app_colors.dart
│   └── themes/
│       └── app_theme.dart
├── domain/
│   └── entities/
│       ├── calendar_day_entity.dart
│       ├── insight_entity.dart
│       ├── mood_entity.dart
│       └── training_entity.dart
├── presentation/
│   ├── controllers/
│   │   ├── home_controller.dart
│   │   ├── mood_controller.dart
│   │   ├── navigation_controller.dart
│   │   ├── plan_controller.dart
│   │   └── theme_controller.dart
│   ├── views/
│   │   ├── home_view.dart
│   │   ├── mood_view.dart
│   │   ├── plan_view.dart
│   │   └── main_screen.dart
│   ├── widgets/
│   │   ├── calendar_week_widget.dart
│   │   ├── calendar_picker_widget.dart
│   │   ├── workout_card_widget.dart
│   │   ├── calories_card_widget.dart
│   │   ├── weight_card_widget.dart
│   │   ├── hydration_card_widget.dart
│   │   ├── week_header_widget.dart
│   │   └── training_day_item_widget.dart
│   └── bindings/
│       └── home_binding.dart
└── main.dart
```

## Getting Started

### Prerequisites

- Flutter SDK (>= 3.0.0)
- Dart SDK (>= 2.17.0)
- Android Studio / VS Code with Flutter extensions

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd hamid_test_task
```

2. Install dependencies:
```bash
flutter pub get
```

3. Run the app:
```bash
flutter run
```

### Build Commands

```bash
# Debug build
flutter build apk --debug

# Release build
flutter build apk --release

# iOS build
flutter build ios --release
```

## Key Features Implementation

### Theme Switching
- Centralized theme management via `ThemeController`
- Reactive theme updates using GetX `Obx`
- Theme-aware colors throughout the app
- Smooth transitions between light and dark modes

### State Management
- Exclusive use of GetX for all state management
- No `setState` usage anywhere in the codebase
- Reactive programming with `Rx` and `Obx`
- Proper dependency injection with `Get.put()` and `Get.lazyPut()`

### UI Components
- One class per file principle for maintainability
- Reusable widgets with proper separation of concerns
- Theme-aware color system
- Responsive layouts with proper overflow handling

### Calendar System
- Interactive weekly calendar view
- Bottom sheet calendar picker
- Day selection with gradient indicators
- Training schedule integration

## Code Quality Standards

- **Clean Architecture**: Clear separation between UI, domain, and data layers
- **GetX Best Practices**: Proper controller lifecycle and reactive patterns
- **Widget Organization**: One widget class per file
- **Theme Consistency**: Centralized color management with theme-aware getters
- **Error Handling**: Proper error boundaries and user feedback

## Assets

Ensure the following assets are available in the `assets/` directory:

```
assets/
├── icons/
└── images/
```

Update `pubspec.yaml` to include asset paths if needed.

## Contributing

1. Follow the existing code structure and patterns
2. Use GetX for all state management
3. Maintain one class per file principle
4. Ensure theme compatibility for all new components
5. Test on both light and dark themes


