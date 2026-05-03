```markdown
# 🔒 Secure Proxy Browser

<div align="center">

![Android](https://img.shields.io/badge/Android-5.0+-green.svg)
![Java](https://img.shields.io/badge/Java-8+-red.svg)
![Status](https://img.shields.io/badge/Status-Stable-brightgreen.svg)

### An Android browser that automatically fetches and applies proxy credentials from a remote server.
### No manual configuration. Zero settings. Just browse.

</div>

---

## 📱 Screenshots

<div align="center">
  <img src="screenshots/1.jpg" width="250" alt="Browser Home">
  <img src="screenshots/2.jpg" width="250" alt="Proxy Working">
</div>

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🚀 Auto Proxy Fetch | Gets live IP, port, username, password from server automatically |
| 🔐 Seamless Authentication | Handles HTTP proxy auth without annoying popups |
| 🧹 Session Isolation | Clean cookies and cache for each new session |
| ⚡ One-Tap Browsing | Just enter URL and press Go |
| 🎨 Modern UI | Clean, premium design with navigation controls |
| 🔄 Back/Forward/Refresh | Full browser navigation buttons |
| 📊 Progress Bar | See page loading progress |
| 🛡️ Proxy Status | Live indicator showing proxy connection status |

---

## 🛠️ Tech Stack

<div align="center">

| Technology | Purpose |
|------------|---------|
| Java | Core programming language |
| Android SDK | Mobile application framework |
| WebView | Browser rendering engine |
| NetCipher | Proxy binding library by Guardian Project |
| REST API | Server communication |
| JSON | Data exchange format |
| ExecutorService | Async network operations |

</div>

---

## 🔧 How It Works

```

┌─────────────────────────────────────────────────────────┐
│                                                         │
│   1. App Starts                                         │
│         ↓                                               │
│   2. Fetches proxy from server (IP, Port, User, Pass)   │
│         ↓                                               │
│   3. NetCipher binds WebView to the proxy               │
│         ↓                                               │
│   4. User enters URL → Traffic routes through proxy     │
│         ↓                                               │
│   5. Browse securely & anonymously                      │
│                                                         │
└─────────────────────────────────────────────────────────┘

```

---

## 📦 Download Source Code

### Option 1: Direct Download
Click on `Secure-Proxy-Browser-(src).zip` from the files above and extract.

### Option 2: Clone Repository
```bash
git clone https://github.com/iamDineshChavan/Secure-Proxy-Browser.git
```

---

🔑 Server Setup

Create a PHP endpoint that returns JSON response:

PHP Code (proxy.php):

```php
<?php
header('Content-Type: application/json');

$response = [
    'proxy1_ip' => '45.38.107.97',
    'proxy1_port' => '6014',
    'proxy1_user' => 'your_username',
    'proxy1_pass' => 'your_password'
];

echo json_encode($response);
?>
```

Sample Response:

```json
{
  "proxy1_ip": "45.38.107.97",
  "proxy1_port": "6014",
  "proxy1_user": "tjnlwvzk",
  "proxy1_pass": "bl153f7ry9tp"
}
```

---

📱 How to Use

1. Install the App
   · Build APK from source or install directly
2. Automatic Proxy
   · App fetches proxy on startup
   · Status shows "Proxy: Active ✓"
3. Start Browsing
   · Enter URL in search bar
   · Press "Go" button
   · Use Back/Forward/Refresh buttons
4. Verify Proxy
   · Visit ipinfo.io
   · Check if IP is different from your real IP

---

📁 Project Structure

```
Secure-Proxy-Browser/
│
├── Secure-Proxy-Browser-(src).zip    # Complete source code
├── README.md                          # This file
│
├── screenshots/
│   ├── 1.jpg                          # Browser home screen
│   └── 2.jpg                          # Proxy working proof
│
└── app/
    └── src/
        └── main/
            ├── java/com/secure/browser/
            │   └── MainActivity.java   # Main browser code
            └── res/layout/
                └── main.xml            # UI layout
```

---

⚙️ Requirements

Requirement Minimum
Android Version 5.0 (Lollipop)
RAM 2GB
Internet Required
Server PHP endpoint for proxy

---

🧪 Testing

Tested on:

· ✅ Google Pixel (Android 14)
· ✅ Samsung Galaxy (Android 13)
· ✅ OnePlus (Android 12)
· ✅ Xiaomi (Android 11)

---

🤝 Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Open Pull Request

---

📄 License

No License – All rights reserved.

You may:

· View the code
· Download for personal use

You may NOT:

· Copy or redistribute
· Use commercially
· Claim as your own

---

👨‍💻 Author

<div align="center">

iamDineshChavan

https://img.shields.io/badge/GitHub-iamDineshChavan-black?logo=github

</div>

---

⭐ Show Support

<div align="center">

If this project helped you, please give it a ⭐ on GitHub!

Star this repo → https://github.com/iamDineshChavan/Secure-Proxy-Browser

</div>

---

<div align="center">

Built with ☕ and Java

"Simple, secure, proxy-enabled browsing for everyone"

</div>
```
