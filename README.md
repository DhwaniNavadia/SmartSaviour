# SmartSaviour

>> Dr. AI - Your Medical Assistant



Dr. AI is an advanced, Flutter-based mobile application developed to act as your personal medical assistant. It combines state-of-the-art technology with medical expertise to provide users with a comprehensive healthcare companion right on their smartphones. The application offers a range of features designed to make healthcare information and services easily accessible, ensuring users can manage their medical needs effectively and promptly.

>> Key Capabilities

- Medical Queries: Users can ask medical questions and receive accurate, timely responses. This feature is powered by a robust backend that sources information from reliable medical databases and expert systems, ensuring the advice and information provided are trustworthy and up-to-date.

- Hospital Locator: In case of emergencies, users can leverage the integrated Google Maps functionality to search for hospitals. The app provides real-time data on the nearest hospitals, helping users navigate quickly to the closest medical facility when every second counts.

- Medical History Access: Dr. AI securely stores users' medical histories in Firebase, allowing users to access their records at any time. This is particularly useful during emergencies, where having quick access to medical history can be crucial. Users can also share their medical history with healthcare providers through NFC technology.

- Emergency Support: The application features an emergency support system that allows users to initiate a chat with a medical assistant or call emergency services directly from the app. This ensures that users can get immediate help in critical situations.

- Data Privacy and Control: Users have full control over their personal data. The app includes options to show or hide specific information, ensuring that users can manage their privacy preferences according to their comfort level. All data is securely stored in Firebase, adhering to best practices in data security and privacy.

>> Technical Stack

- Frontend: Developed using Flutter, the app boasts a responsive and intuitive user interface.

- Backend: Firebase serves as the backbone for data storage, authentication, and real-time database management, ensuring reliable and secure data handling.

- APIs and Integrations: The app integrates various third-party APIs such as ChatGPT 4 & Gemini-1.5-flash for medical assistant, Google Maps for location services, and NFC technology for sharing medical data.
- Data Storage: Hive database is used for storing chat messages locally, providing fast and efficient data retrieval.

>> Why Choose Dr. AI?

Dr. AI is designed to be more than just a medical app; it's a comprehensive health assistant that combines the power of modern technology with essential healthcare services. Whether it's a routine checkup or an emergency, Dr. AI is equipped to provide users with the necessary tools and information to manage their health proactively and effectively. With features like real-time hospital navigation, instant medical queries, and secure medical history access, Dr. AI stands out as a reliable companion in the digital health landscape.



- Step 1: Install Dependencies
After navigating to the project directory, you need to install all the necessary dependencies. 
Run:

flutter pub get

This command fetches all the dependencies listed in the 'pubspec.yaml' file.

- Step 2: Set Up Firebase
Dr. AI uses Firebase for authentication, data storage, and other backend services. Follow these steps to set up Firebase:

1. Add 'Firebase' to Your Project:

- Go to the 'Firebase Console'.

- Create a new project or select an existing one.

- Add an Android to your Firebase project.

2. Download Configuration Files:

- Download the google-services.json file and place it in the android/app directory.
 
3. Initialize Firebase in Your Project:

- Open main.dart and initialize Firebase by adding the following code:


import 'package:firebase_core/firebase_core.dart';
import 'package:flutter/material.dart';

void main() async {
  WidgetsFlutterBinding.ensureInitialized();
  await Firebase.initializeApp();
  runApp(MyApp());
}


- Step 3: Configure the App
Ensure all necessary configurations are done. This includes adding your assets and setting up environment variables if needed. Verify that your `pubspec.yaml` file includes all required `assets` and `fonts`.

- Step 4: Run the Application
Finally, run the application on your desired device using the following command:

flutter run

This command compiles your Flutter app and deploys it to the connected device or simulator.

>> Additional Tips
Updating Dependencies: If there are any updates to the dependencies, you can update them using:

flutter pub upgrade --major-versions

Flutter Doctor: Run flutter doctor to ensure that your development environment is set up correctly.

flutter doctor

This command checks your environment and displays a report of the status of your Flutter installation, dependencies, and connected devices.

By following these steps, you'll have the Dr. AI app up and running on your device, ready to serve as your personal medical assistant. If you encounter any issues during installation, please refer to the Flutter documentation or the Firebase setup guide for additional help.

>> Dependencies

Dr. AI uses various packages to provide its functionality, including but not limited to:

- animated_bottom_navigation_bar: Animated bottom navigation bar widget.
- bloc: Business Logic Component for state management.
- build_runner: Automates build tasks for Dart projects.
- cloud_firestore: NoSQL cloud database service by Firebase.
- cupertino_icons: Cupertino style icons library for Flutter.
- dio: Powerful HTTP client for Dart applications.
- dropdown_button2: Customizable and feature-rich dropdown button.
- easy_stepper: Customizable stepper widget for Flutter.
- firebase_auth: Firebase SDK for user authentication.
- firebase_core: Essential Firebase functionality for Flutter apps.
- flutter_bloc: Bloc state management library for Flutter.
- flutter_dotenv: Manage environment variables in Flutter.
- flutter_facebook_auth: Integrate Facebook login in Flutter apps.
- flutter_polyline_points: Decode Google Maps polylines easily.
- flutter_screenutil: Adaptive screen size and layout utility.
- flutter_svg: Render SVG images in Flutter applications.
- formatted_text: Format and display rich text easily.
- gap: Utilities and helper functions for Dart.
- geolocator: Access geolocation services and GPS coordinates.
- google_generative_ai: Google's generative AI integration tools.
- google_maps_flutter: Google Maps integration for Flutter applications.
- google_sign_in: Google Sign-In for Flutter apps.
- hive: Lightweight, fast, and secure NoSQL database.
- hive_flutter: Hive database integration for Flutter apps.
- hive_generator: Generates TypeAdapters for Hive database.
- image_picker: Select images from gallery or camera.
- intl: Internationalization and localization support for Dart.
- loading_indicator: Animated loading indicators for Flutter apps.
- location: Retrieve location data on Android and iOS.
- lottie: Render animations created with Lottie.
- material_floating_search_bar_2: Material design floating search bar.
- meta: Provides metadata annotations for Dart code.
- modal_progress_hud_nsn: Displays modal progress indicators.
- path_provider: Access filesystem paths for storage.
- shared_preferences: Persistent key-value storage for Flutter.
- sign_in_with_apple: Apple Sign-In authentication for Flutter.
- speech_to_text: Convert speech to text using microphone.
- url_launcher: Launch URLs in the mobile browser.
- uuid: Generate and parse UUIDs in Dart.
  
>> dev_dependencies:

- flutter_launcher_icons: A package to help with creating app launcher icons.
- flutter_lints: A package that provides recommended lints for Flutter projects.
  
For a complete list of dependencies, refer to the 'pubspec.yaml' file.
