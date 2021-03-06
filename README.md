# Jumpcutter Tkinter GUI

Carykh's jumpcutter but with a homemade tkinter interface.

Adjust the speeds of the sounded and silent parts of the video without manual editing. Original explanation by carykh [here](https://www.youtube.com/watch?v=DQ8orIurGxw).


### Some heads-up:

It uses Python 3.

It works on Ubuntu 16.04 and Windows 10. (It might work on other OSs too, we just haven't tested it yet.)

This program relies heavily on ffmpeg. It will start subprocesses that call ffmpeg, so be aware of that!
As the program runs, it saves every frame of the video as an image file in a
temporary folder. If your video is long, this could take a LOT of space. I have processed 17-minute videos completely fine, but be wary if you're gonna go longer.

You can download a zip file that includes ffmpeg [here](https://www.dropbox.com/s/5anbg3x9og3bz82/JumpcutterGUI.zip?dl=1).

### Pyinstaller
Pyinstaller doesn't work when the script is creating temp files. I tried cxfreeze, but doesn't work with scipy. :/

---

# Getting Started

Download and install the latest version of Python for Windows from https://www.python.org/.
When installing, make sure you add Python to PATH.

Next, open up cmd any type the following command to install the required libraries:
```
pip install Pillow audiotsm scipy numpy pytube3 easygui
```

Next, download [this zip](https://www.dropbox.com/s/5anbg3x9og3bz82/JumpcutterGUI.zip?dl=1) and extract it.

Run 'jumpcutter.pyw' in the SAME FOLDER as 'ffmpeg.exe'. The program will now start.

---


## View the UI:

![View the Interface](https://github.com/BatchSource/Jumpcutter-GUI/blob/master/example.gif)
