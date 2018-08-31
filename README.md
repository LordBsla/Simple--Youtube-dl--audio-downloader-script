# Simple--Youtube-dl--audio-downloader-script
<hr>

A simple shell script that automates the usage of 'youtube-dl' for downloading audio from youtube<br>
# Information<br>
-embeds the video stream thumbnail to the downloaded file(via ffmpeg)<br><br>
-downloads audio at at 127kbps(won't work if the video is at a lower audio quality)<br>
<br>
# Requirements:<br>

 - A 'Linux' shell (can work on Windows via the 'Windows subsystem for Linux ')
 - The packages ```youtube-dl``` & ```ffmeg``` should be installed

 
 # Setup:
- First install the necessary programs in your Linux environment:
```
sudo apt install youtube-dl ffmpeg
```
- then put the script in your shell's home/default directory <br>
```
cd <download dir>/<script version>
mv audio-downloader ~
```
# Usage
Issue ```sh audio-downloader``` in the directory of which the script is located. In our case it's the home directory ```~``` it will ask you for the video URL

# Notes:
- The Linux version would download the the mp3 files to your current ```pwd```
- The WSL version would always download the mp3 files to ```C:\youtube-dl```

# Food for though
- Modifiying the flag ``` -f``` within the script can allow you to download files from other online media sources(such as sound cloud)
- Modifying the flag ```-o``` within in the script will allow you to change the download location, download naming scheme(including creating new folder on download for playlists for example)
- With more modifications it can work on android(using 'Termux')<hr>However if you can do any of this however you're better off creating your own shell scripts as you see fit this is inteanded for absolute beginners :)
