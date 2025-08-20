# ClipCanvas: Your Personal Media Dashboard

Welcome to ClipCanvas! This document provides a comprehensive overview of the application, its features, and how to use them.

---

## 🚀 Introduction

**ClipCanvas** is a powerful, browser-based media dashboard designed for a seamless and highly customizable viewing experience. It acts as a personal media player and gallery, allowing you to watch videos and view images from various sources in a beautiful, immersive interface. All your data, playlists, and preferences are stored locally in your browser, ensuring your privacy.

---

## ✨ Key Features

* **Multiple Media Feeds:** Switch between a pre-loaded **Social Feed**, your own **Local Feed**, and a powerful **Folder Feed** that plays directly from a directory on your computer.
* **Advanced Video Player:** Enjoy a custom video player with features like ambient mode, screen lock, rotation, zoom & pan, and extensive keyboard shortcut support.
* **Comprehensive Library:** View all your media in a responsive gallery, create and manage custom playlists, and easily access recently played folders.
* **User Profiles:** The app supports user profiles, allowing for a personalized experience.
* **Powerful Admin Panel:** Get an overview of your library statistics, manage users, and upload media for different profiles.
* **Deeply Customizable Settings:** A beautiful, Android-style settings panel with a search bar lets you tweak every aspect of your viewing experience, from theme and layout to button visibility and shortcut mapping.
* **100% Local & Private:** All media metadata, settings, playlists, and user profiles are stored securely in your browser's IndexedDB. No data is ever uploaded to a server.

---

## 🖥️ Getting Started

To use ClipCanvas, simply **open the `ClipCanvasPro.html` file in a modern web browser** like Google Chrome, Firefox, or Microsoft Edge. The app will initialize, and you can start exploring your media right away.

---

## 核心概念

### The Feeds

ClipCanvas organizes your media into three distinct feeds, which you can switch between using the buttons at the top of the screen when in the video player view.

* **Social Feed:** This is the default feed, pre-loaded with sample videos to demonstrate the player's functionality.
* **Local Feed:** This feed contains all the video and image files you have personally added to the ClipCanvas library.
* **Folder Feed:** This powerful feature allows you to select a folder from your computer. ClipCanvas will then scan it for compatible video files and let you play them directly without adding them to your library. This is perfect for browsing through folders of media quickly.

### The Video Player

The video player is the heart of ClipCanvas and is packed with features.

* **Ambient Mode:** Creates a blurred, colorful background based on the current video for a more immersive experience.
* **Lock Mode:** Prevents accidental touches and hides the UI, perfect for uninterrupted viewing.
* **Rotation:** Rotates the video by 90-degree increments.
* **Zoom & Pan:** Zoom into the video up to 3x and pan around to focus on details.
* **Double-Tap to Seek:** Double-tapping on the left or right side of the video will seek backward or forward by 10 seconds.
* **Controls:** All standard controls are available, including play/pause, fullscreen, and access to playlists.

### The Gallery View

The Gallery is the default home screen. It shows thumbnails for all media across your library. You can click on any video thumbnail to start playing it in the video player or click on an image to view it in a full-screen overlay.

---

## 📚 Library Management

You can manage your library and playlists using the sidebar on the left.

* **Adding Media:** Click **"Add to Local Feed"** in the sidebar to open a file dialog. You can select multiple video or image files to add them to your local library.
* **Playing from a Folder:** Click **"Play From Folder"** to select a directory on your computer. The player will launch into the Folder Feed.
* **Recent Folders:** The sidebar will automatically keep track of your 5 most recently used folders for quick access.
* **Playlists:**
    * Create a new playlist by clicking the **"Create New Playlist"** button.
    * Add the current video to a playlist by tapping the playlist icon in the player controls.
    * View a playlist's contents by clicking its name in the sidebar. This will open the gallery view filtered to that playlist.
    * Click **"EDIT"** above the playlist list to enter edit mode, where you can delete custom playlists.

---

## ⚙️ The Settings Panel

ClipCanvas features a comprehensive, Android-style settings panel with a search bar. You can access it by clicking **"Settings"** in the sidebar.

### Search

The search bar at the top allows you to instantly filter all available settings by title or description.

### Appearance

* **Theme:** Switch between the default Dark mode and a new Light mode.
* **Ambient Mode:** Enable or disable the immersive ambient background effect.
* **Default Home View:** Choose whether the app opens to the **Gallery** or the **Feed** (video player) view.

### Behavior

* **Mute All Videos:** Force all videos to start in a muted state.
* **Enable Auto-Scroll:** When a video finishes, automatically scroll to and play the next one in the feed.
* **Zoom Controls Auto-Hide:** Use a slider to set the delay (1-10 seconds) before the zoom controls disappear.

### Visible Player Buttons

This section lets you show or hide specific control buttons in the video player UI to create a more minimal interface. You can toggle the visibility of:

* Watch Later Button
* Save Button
* Orientation Button
* Zoom Controls
* Fullscreen Button

### Keyboard Shortcuts

This section allows you to view and remap every available keyboard shortcut. To change a shortcut:

1.  Click the **"Remap"** button next to the action you want to change.
2.  The button will change to **"Listening..."**.
3.  Press the new key you want to assign. The shortcut is now saved.

The shortcuts are organized into three groups:

* **Playback Controls:** Play/Pause, Next/Previous Video, Seek Forward/Backward.
* **Player Actions:** Lock Mode, Fullscreen, Rotate, Save, and Add to Playlist.
* **Zoom & Pan Controls:** Zoom In/Out and Pan Up/Down/Left/Right.

### Danger Zone

* **Reset All App Data:** This button will completely wipe all data stored by ClipCanvas in your browser, including all media, users, playlists, and settings. **This action cannot be undone.**

---

## 🛠️ Technical Overview

ClipCanvas is built with modern web technologies and runs entirely in the browser.

* **Frontend:** Plain HTML, CSS, and JavaScript.
* **Styling:** Utility classes are provided by **Tailwind CSS**.
* **Data Storage:** All application data is stored locally using **IndexedDB**, a powerful browser-based database.
* **Charts:** The Admin Panel uses **Chart.js** to render statistics.
