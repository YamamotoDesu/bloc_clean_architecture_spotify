# bloc_clean_architecture_spotify

## Folder Structure
```
└── 📁lib
    └── 📁common
    └── 📁core
    └── 📁data
        └── 📁models
        └── 📁repository
        ├── sources
    └── 📁domain
        └── 📁entities
        ├── usecases
    └── main.dart
    └── 📁presentation
        └── 📁bloc
        └── 📁pages
        ├── widgets
```

## Theme
![image](https://github.com/YamamotoDesu/bloc_clean_architecture_spotify/assets/47273077/76ef948c-745d-4a4d-8b51-dbdec39a8205)

lib/core/cofigs/theme/app_theme.dart
```dart
import 'package:bloc_clean_architecture_spotify/core/cofigs/theme/app_colotrs.dart';
import 'package:flutter/material.dart';

class AppTheme {
  static final lightTheme = ThemeData(
      primaryColor: AppColors.primary,
      scaffoldBackgroundColor: AppColors.lightBackground,
      brightness: Brightness.light,
      fontFamily: 'Satoshi',
      sliderTheme:
          SliderThemeData(overlayShape: SliderComponentShape.noOverlay),
      inputDecorationTheme: InputDecorationTheme(
          filled: true,
          fillColor: Colors.transparent,
          contentPadding: const EdgeInsets.all(30),
          hintStyle: const TextStyle(
            color: Color(0xff383838),
            fontWeight: FontWeight.w500,
          ),
          border: OutlineInputBorder(
              borderRadius: BorderRadius.circular(30),
              borderSide: const BorderSide(color: Colors.white, width: 0.4)),
          enabledBorder: OutlineInputBorder(
              borderRadius: BorderRadius.circular(30),
              borderSide: const BorderSide(color: Colors.black, width: 0.4))),
      elevatedButtonTheme: ElevatedButtonThemeData(
          style: ElevatedButton.styleFrom(
              backgroundColor: AppColors.primary,
              elevation: 0,
              textStyle:
                  const TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
              shape: RoundedRectangleBorder(
                  borderRadius: BorderRadius.circular(30)))));

  static final darkTheme = ThemeData(
      primaryColor: AppColors.primary,
      scaffoldBackgroundColor: AppColors.darkBackground,
      brightness: Brightness.dark,
      fontFamily: 'Satoshi',
      sliderTheme: SliderThemeData(
          overlayShape: SliderComponentShape.noOverlay,
          activeTrackColor: const Color(0xffB7B7B7),
          inactiveTrackColor: Colors.grey.withOpacity(0.3),
          thumbColor: const Color(0xffB7B7B7)),
      inputDecorationTheme: InputDecorationTheme(
          filled: true,
          fillColor: Colors.transparent,
          hintStyle: const TextStyle(
            color: Color(0xffA7A7A7),
            fontWeight: FontWeight.w500,
          ),
          contentPadding: const EdgeInsets.all(30),
          border: OutlineInputBorder(
              borderRadius: BorderRadius.circular(30),
              borderSide: const BorderSide(color: Colors.white, width: 0.4)),
          enabledBorder: OutlineInputBorder(
              borderRadius: BorderRadius.circular(30),
              borderSide: const BorderSide(color: Colors.white, width: 0.4))),
      elevatedButtonTheme: ElevatedButtonThemeData(
          style: ElevatedButton.styleFrom(
              backgroundColor: AppColors.primary,
              elevation: 0,
              textStyle:
                  const TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
              shape: RoundedRectangleBorder(
                  borderRadius: BorderRadius.circular(30)))));
}

```
