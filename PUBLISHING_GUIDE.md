# StudyHabit: Free Community Publishing & Update Guide

## 1. How to Host 100% Free on GitHub Pages (Zero Cost)
1. Go to [GitHub.com](https://github.com) and create a free account.
2. Click **New Repository** and name it `studyhabit` (set to **Public**).
3. Upload all files from this folder (`index.html`, `manifest.json`, `sw.js`, `icons/`).
4. Go to **Settings > Pages > Branch: main / root > Save**.
5. In 60 seconds, your app will be live at: `https://<your-username>.github.io/studyhabit/`.

## 2. How Students Install It on Android & iPhone
- **Android**: Students open your link in Chrome. They will see an **"Install App"** prompt, or tap the 3 dots > **"Install App / Add to Home screen"**. It installs with an app icon and runs full-screen offline with no app store needed!
- **iPhone / iPad**: Open in Safari > Tap the **Share icon** > Tap **"Add to Home Screen"**.

## 3. How to Publish on the Google Play Store
1. Open [PWABuilder.com](https://www.pwabuilder.com) (free Microsoft tool).
2. Enter your live website URL (e.g. `https://<your-username>.github.io/studyhabit`).
3. Click **Package for Android** -> Download the generated `.aab` file.
4. Upload the `.aab` to your Google Play Console account and mark the price as **Free ($0.00)**.

## 4. How Future Updates Work & How Students Get Notified
- **Instant Cloud Sync**: Whenever you want to add new features or fix bugs, simply upload the new `index.html` to your GitHub repository.
- **Auto-Notification**: The Service Worker (`sw.js`) automatically detects the changed files when a student opens the app.
- An in-app banner immediately prompts the student: *"🚀 New Community Update Available! [Update Now]"*.
- Clicking **Update Now** reloads the app with your latest improvements, while keeping their saved study sessions, 80/20 records, and custom timers 100% safe in `localStorage`!
