# 📱 prodev-mobile-setup

## Objective

Set up your first **mobile application** using the **Expo Router template**, understand the project structure, and document the scaffolding and reset process.

---

## 🚀 Project Setup Steps

### 1. Navigate to Your Project Directory

```bash
cd prodev-mobile-setup
```

### 2. Initialize a New Expo Project

Used the **Expo Router template** to scaffold the project:

```bash
npx create-expo-app@latest .
```

This command created a React Native project using Expo, with a pre-configured folder structure that includes **app routing, tabs, and theming**.

---

## 🧩 Understanding the File Structure

After setup, the main structure looked like this:

```
prodev-mobile-setup/
├── app/
│   ├── (tabs)/
│   │   ├── index.tsx         # Main Home (Tab One) screen
│   │   ├── two.tsx           # Second tab
│   ├── _layout.tsx           # Layout configuration for tabs
├── components/
│   ├── EditScreenInfo.tsx
│   ├── Themed.tsx
├── package.json
├── App.tsx
```

**Key point:**
Expo Router automatically turns files inside `/app` into navigable screens — similar to Next.js pages.

---

## 🛠️ Modifying the Home Screen

Edited the file:

```
app/(tabs)/index.tsx
```

Replaced the default text with:

```tsx
<Text style={styles.title}>** First App Created **</Text>
```

This change updates the app’s home screen message.

---

## ▶️ Running and Testing the Application

To start the development server:

```bash
npx expo start
```

Then:

- **For Android:** Scan the QR code using the **Expo Go** app.
- **For iOS:** Scan the QR code using your phone’s **Camera app**.

The app will load live updates from your local server.

---

## 🔄 Resetting the Application

A new script was added to `package.json`:

```json
"scripts": {
  "reset-project": "expo start --clear"
}
```

To reset the project, run:

```bash
npm run reset-project
```

### 🧹 What It Does

This command:

- Clears the **Metro bundler cache** (used by Expo to speed up builds),
- Removes stale files or configurations,
- Restarts the development server from a clean state.

### 🧠 Observation

After running the reset command:

- The terminal restarted Expo with a **fresh build**.
- Old caches and temporary files were cleared.
- The QR code reappeared, and the app loaded as if freshly installed.

---

## 📘 Summary

| Step  | Description                                              |
| ----- | -------------------------------------------------------- |
| **1** | Initialized project using `npx create-expo-app@latest .` |
| **2** | Edited the home screen text in `app/(tabs)/index.tsx`    |
| **3** | Ran and tested app with `npx expo start`                 |
| **4** | Reset project with `npm run reset-project`               |
| **5** | Documented structure, setup, and reset behavior          |

---

## 🧭 Repository Info

- **GitHub Repository:** `prodev-mobile-setup`
- **Directory:** `prodev-mobile-app-0x00`
- **Files Included:**

  - `README.md`
  - `app-example/app/(tabs)/index.tsx`
  - `app-example/constants/Colors.tsx`
