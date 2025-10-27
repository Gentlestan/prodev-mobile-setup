Create Your First Mobile App — Expo Router Setup
🎯 Objective

This project demonstrates how to set up and scaffold your first React Native mobile app using the Expo Router template.
It includes documentation of the setup steps, folder structure, and the effect of resetting the project.

🧩 Project Information
Repository: prodev-mobile-setup
Directory: prodev-mobile-app-0x00
Framework: React Native (Expo)
Platform Tested: Android (Expo Go)
🪜 Steps Followed

1. Navigate to the Project Directory

Opened the terminal and moved into the parent folder:

cd prodev-mobile-setup

2. Initialize the Project

Created a new Expo app using the Expo Router template:

npx create-expo-app@latest .

After running the command, Expo scaffolded the project with the following main folders:

app/
┣ (tabs)/
┃ ┣ index.tsx
┃ ┣ explore.tsx
┃ ┗ \_layout.tsx
┣ \_layout.tsx
assets/
constants/

3. Modify the Home Screen

Opened the file:

app/(tabs)/index.tsx

Found the default text:

<Text>Welcome!</Text>

Replaced it with:

<Text>**First App Created**</Text>

This change updates the welcome message displayed on the app’s home screen.

4. Run and Test the Application

Started the Expo development server:

npx expo start

Then scanned the QR code with Expo Go on my Android device.
The app successfully launched and displayed the updated text:

First App Created

5. Reset the Application

Ran the reset command:

npm run reset-project

🧠 Observation:

The reset-project command:

Cleared the node_modules folder.
Reinstalled dependencies.
Reset the Metro bundler cache.
Removed any local build and temporary files.

After running it, I had to restart the development server again using:

npx expo start

📁 Key Files Updated
File Description
app/(tabs)/index.tsx Home screen updated to display “First App Created”.
constants/Colors.tsx Used for color themes and styling across the app.
README.md Documenting setup process and reset command behavior.
✅ Summary
Successfully scaffolded and ran an Expo Router project.
Modified the home screen text.
Tested on Android using Expo Go.
Verified project reset functionality.
