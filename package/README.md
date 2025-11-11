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
> `py __init__.py`
> 
>  or
> 
> `python __init__.py`


# youtube-selenium-cookie

```python
from youtube-selenium-cookie import Youtube

upload_info = {
    "title": "rema calm down",
    "description": "Another banger",
    "video": "C:/Users/HP/Desktop/youtube automation video/channels/4th.mp4",
    "thumbnail": "",
    "category": "Music",
    "privacy": "Public",
    "tags": ["rema", "banger", "loudness", "music", "holiday"],
    "kids": False
}

Youtube("./cookies.json", upload_info, True).upload()
```

This packages solely works on cookies. You can grab your cookies by installing edit-the-cookies chrome extension.

The only method available now is upload which uploads to your channel whose cookie you provided.

the video and thumbnail path must be absolute

feel free to make PRs. In case something breaks.

@Dataslid softwares

wpk