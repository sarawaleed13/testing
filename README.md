# testing

A new Flutter project.
# Firebase App Distribution Integration

This project demonstrates how to integrate Firebase App Distribution in a Flutter app to manage beta testing with selected testers.

## Task Overview
Integrate Firebase App Distribution to:
1. Distribute pre-release app versions
2. Manage beta testers
3. Collect feedback before production releases

## Requirement 1: Firebase Project Setup

### Steps Completed
1. **Created Firebase Project**
   - Set up new project in [Firebase Console](https://console.firebase.google.com/)
   - Named project: `[Your_Project_Name]`

2. **Added Android App**
   - Registered Android package name: `[your.package.name]`
   - Downloaded `google-services.json` configuration file

3. **Configured Flutter Project**
   - Placed `google-services.json` in:
     ```
     android/app/google-services.json
     ```
   - Added required dependencies to `pubspec.yaml`:
     ```yaml
     dependencies:
       firebase_core: ^2.18.0
       firebase_app_distribution: ^5.0.0
     ```

4. **Initialized Firebase**
   - Generated Firebase configuration:
     ```bash
     dart run flutterfire_cli:flutterfire configure
     ```
   - Initialized Firebase in `main.dart`:
     ```dart
     await Firebase.initializeApp(
       options: DefaultFirebaseOptions.currentPlatform,
     );
     ```

### Verification Steps
1. Build the app to confirm Firebase connection:
   ```bash
   flutter run

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
