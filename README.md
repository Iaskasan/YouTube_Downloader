# YouTube Downloader

`youtube_downloader` is a simple tool that allows you to download either videos or audio from YouTube. An option for full playlist download is also available. Here's a preview of the GUI:


## Disclaimer

`youtube_downloader` is made for personnal-use only. Please do not make any profit over the downloaded content.

## Requirements

- **Python3.8.x +**: https://www.python.org/downloads/

- **pip Windows**:
```
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`
python get-pip.py
```

- **pip Debian-based distributions** (e.g., Ubuntu):

```
sudo apt update
sudo apt install python3-pip
```


- **tkinter module for Windows**: Tkinter usually comes pre-installed with Python. However, if you encounter issues or need to reinstall it, you can use the following command: 
``` 
pip install tk
```

- **tkinter module for Debian-based distributions** (e.g., Ubuntu): 
```
sudo apt-get update
sudo apt-get install python3-tk
```

- **pytube module**: https://pytube.io/en/latest/user/install.html

## How to use

- First clone this repository: `git clone https://github.com/Iaskasan/YouTube_Downloader.git`
- Go to your cloned repository's path and simply start the `main` file.

## Creating an executable file of the YouTube_Downloader

You can create a standalone executable file of the `YouTube_Downloader` by following those steps:
- Install the module `PyInstaller`. It will allows you to convert a `.py` module into an `.exe` file: `pip install pyinstaller`.

- Run the command-line `pyinstaller --onefile main.py`, optionnaly you can add the argument `--noconsole` to hide the console window when running the executable file: `pyinstaller --onefile --noconsole main.py` (Only works for Windows).
The standalone executable will be located in the dist directory within your current working directory: 

`dist/main.exe`  # On Windows

`dist/main`      # On Linux or macOS

## Features

- You can choose between videos or audio only.
- You can download entire playlist with the above conditions too.
- You can choose the destination path.
- The quality will be defaulted as the one present on the video when you give the URL (e.g., if the youtube's video is on 1080p, then the downloaded one will be of the same quality)

## Known issues

- Downloading a playlist creates a "Programm not responding" error but the programm is still doing its work so don't worry about that.
- (Windows) When creating a `.exe` file using the `PyInstaller` module, winbdows will treat it as a malware/virus. To avoid that you will have to disable the `Real-time protection` before using the command-line `pyinstaller --onefile main.py`. Don't forget to reacivate the `Real-time protection` right after the `.exe` has been created.
## Author

- [@Iaskasan](https://github.com/Iaskasan/)

