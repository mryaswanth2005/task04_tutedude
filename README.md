## Change App Name & Home Page Title

drive link: https://drive.google.com/drive/folders/1drxoRHnJoTLdAJFBBwRr6OSoUm96E9Rk?usp=sharing

This guide explains how to modify the default Flutter app by changing:

* App name (shown on device)
* Home screen title (AppBar text)

---

## 📱 1. Change App Name

### 🔹 For Android

1. Go to:

```
android/app/src/main/AndroidManifest.xml
```

2. Find this line:

```
android:label="demo_app"
```

3. Replace it with your app name:

```
android:label="My Awesome App"
```

---

### 🔹 For iOS

1. Go to:

```
ios/Runner/Info.plist
```

2. Find:

```
<key>CFBundleName</key>
<string>demo_app</string>
```

3. Change it to:

```
<string>My Awesome App</string>
```

---

## 🏠 2. Change Home Page Title

1. Open:

```
lib/main.dart
```

2. Find the AppBar section:

```
appBar: AppBar(
  title: Text('Flutter Demo Home Page'),
),
```

3. Update the title:

```
appBar: AppBar(
  title: Text('My Home Page'),
),
```

---

## 🎨 3. Change App Title (Top-level)

Inside `MaterialApp`, update:

```
MaterialApp(
  title: 'Flutter Demo',
)
```

Change to:

```
MaterialApp(
  title: 'My Awesome App',
)
```

---

## 🔄 4. Apply Changes

After making changes, run:

```
flutter clean
flutter pub get
flutter run
```

---

## ✅ Result

After completing the steps:

* App name will be updated on device
* Home page title will display your custom text



---
