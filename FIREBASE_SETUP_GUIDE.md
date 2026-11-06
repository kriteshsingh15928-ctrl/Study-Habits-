# How to Enable Real Google Sign-In in 5 Minutes (100% Free)

By default in web browsers, real Google Sign-In popups require connecting to a free Google Firebase project so Google knows which app is asking to authenticate the student.

Google gives you 50,000 monthly active users for free forever. Here is the exact 5-minute setup:

### Step 1: Create a Free Project in Firebase
1. Go to [console.firebase.google.com](https://console.firebase.google.com) and log in with your Google account.
2. Click **Add Project** -> name it `studyhabit`.
3. Disable Google Analytics (optional, for simpler setup) -> click **Create Project**.

### Step 2: Enable Google Authentication
1. In your Firebase dashboard, click **Build > Authentication > Get Started**.
2. Under the **Sign-in method** tab, click **Google**.
3. Toggle the **Enable** switch.
4. Set your support email (your Gmail) and click **Save**.

### Step 3: Get Your Free Configuration Keys
1. In your Firebase Project Overview (gear icon in the top left), click **Project settings**.
2. Scroll down to **Your apps** and click the Web icon (`</>`).
3. Name it `StudyHabit Web` and click **Register app**.
4. You will see a `firebaseConfig` object that looks like this:
```javascript
const firebaseConfig = {
  apiKey: "AIzaSy...",
  authDomain: "studyhabit.firebaseapp.com",
  projectId: "studyhabit",
  storageBucket: "studyhabit.appspot.com",
  messagingSenderId: "...",
  appId: "..."
};
```

### Step 4: Paste into index.html
Open `index.html` in Notepad or VS Code, paste your `firebaseConfig` inside the script section, and real Google Sign-In popups will immediately work across all student devices!
