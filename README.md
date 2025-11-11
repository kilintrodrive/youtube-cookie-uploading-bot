> [!TIP] 
> # How to run
> 
> ## Install Python
> 
> 1. Go to the official Python website: https://www.python.org/downloads/release/python-3139/
> 2. Scroll down to the files part. Then download the Windows installer (64-bit)
> 3. Once downloaded, run the installer.
> 4. ✅ Important: On the first screen of the installer, check the box that says
> “Add Python to PATH” before clicking Install Now.
> ## How to download the repo
> Click the button below to download the code as a .zip:
>
> <a href="https://github.com/kilintrodrive/youtube-cookie-uploading-bot/archive/refs/heads/main.zip"><img src="https://img.shields.io/badge/⬇️_Download_ZIP-2ea44f?style=for-the-badge&logo=github&logoColor=white" alt="Download ZIP"></a>
>
> 
> Now extract the .zip folder
> 
> ## Run the script
> 
> Open the command prompt inside the extracted folder and run:
>
> `py example.py`
> 
>  or
> 
> `python example.py`


# 🎬 YouTube Upload Automation

This project automates video uploads to **YouTube** using **Python** and **Selenium**, by leveraging a saved login session through browser cookies.

---

## ⚙️ Features

* Automated login and cookie saving for YouTube using Selenium
* Video upload automation with metadata (title, description, tags, privacy, etc.)
* Simple example usage for customization

---

## 📁 Project Structure

```
.
├── example.py        # Example script showing how to upload a YouTube video
├── login.py          # (Legacy) Script that logs into Gmail and saves cookies
├── gl.py             # (Legacy) Experimental Google login with PhantomJS
├── cookies.json      # Saved YouTube cookies for authentication
└── README.md         # Project documentation
```

---

## 🧠 How It Works

1. **`login.py`** uses Selenium to log into Gmail/YouTube manually, waits for authentication, and saves the session cookies into `cookies.json`.
2. **`example.py`** loads those cookies and uploads a YouTube video automatically using a `Youtube` class (from the imported `package` module).
3. The upload includes metadata such as title, description, category, tags, and privacy settings.

---

## 🪄 How to Use

### 1. Install Requirements

Make sure you have **Python 3.8+** installed.
Then, install dependencies:

```bash
pip install selenium webdriver-manager
```

---

### 2. Set Up Cookies

Run the login script to create a cookie file:

```bash
python login.py
```

> 💡 You will need to log in manually during this step. Once complete, `cookie.json` will be saved automatically.

---

### 3. Edit `example.py`

Update the `upload_info` dictionary with your desired video details:

```python
upload_info = {
    "title": "My Awesome Video",
    "description": "This is an automated upload.",
    "video": "C:/path/to/video.mp4",
    "thumbnail": "",
    "category": "Music",
    "privacy": "Public",
    "tags": ["automation", "python", "youtube"],
    "kids": False
}
```

---

### 4. Run the Script

Finally, run:

```bash
python example.py
```

The script will automatically upload your video using the stored login session.

---

## ⚠️ Important Notes

* **Do not share your `cookies.json`** — it contains authentication data.
* Using automation to log into or upload content to YouTube may violate Google’s **Terms of Service**.
  Use this project only for educational or personal testing.
* `login.py` currently hardcodes credentials — remove or modify before using securely.
* The project depends on a missing module called `package` (providing the `Youtube` class). Ensure it’s installed or implemented in your environment.

---

## 🧩 Future Improvements

* Replace password-based login with OAuth2 for security
* Use YouTube Data API for compliant video uploads
* Add error handling and progress tracking for uploads

---

## 📝 License

This project is provided **for educational purposes only**.
You are responsible for ensuring compliance with YouTube and Google policies.

eqy