# rav1e_gui [![Travis Build Status](https://travis-ci.org/moisesmcardona/rav1e_gui.svg?branch=master)](https://travis-ci.org/moisesmcardona/rav1e_gui) [![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/github/moisesmcardona/rav1e_gui?branch=master&svg=true)](https://ci.appveyor.com/project/moisesmcardona/rav1e-gui)
A GUI to convert video files to AV1 using rav1e

![Main Window Screenshot](https://moisescardona.me/wp-content/uploads/2019/04/rav1e-GUI-v1.12-Main-Window.png)

![Advanced Encoder Options Window Screenshot](https://moisescardona.me/wp-content/uploads/2019/04/rav1e-GUI-v1.11-Advanced-Options.png)

I wrote this software to test the rav1e software. Unfortunately, at the current state, rav1e is single-threaded. This GUI solves the issue and enable multithreading by converting and splitting the input video file into segments of the length specified by the user in y4m format and encoding the audio to Opus ffmpeg. It then encodes each file using a CPU thread. After the encoding is finished, the .ivf files are concatenated. Lastly, the .ivf and .opus files are merged into a .webm or .mkv container.

Written in Visual Basic .NET using Visual Studio 2017.
## Dependencies:

* You need ffmpeg as found here: https://ffmpeg.zeranoe.com/builds/. Use the nightly builds. [Instructions here.](https://moisescardona.me/downloading-ffmpeg-rav1e-gui/)
* You also need rav1e. The software comes bundled with it already, but newer builds can be found here: [https://moisescardona.me/rav1e-builds/](https://moisescardona.me/rav1e-builds/)

Builds comes with opusenc and rav1e bundled, but not ffmpeg due to licensing restrictions.

# Updated components builds:

Ocasionally, rav1e and opusenc gets updated. You can download the latest version of rav1e_gui with these updated tools included here: [https://moisescardona.me/rav1e-gui](https://moisescardona.me/rav1e-gui)

Enjoy!
