# Video Conversor
Converts video files to MP4 and WEBM with 2 passes variable bitrate using FFmpeg
- MP4 conversion is H264 QuickTime compatible
- docs: https://trac.ffmpeg.org/wiki/Encode/VP9 / https://trac.ffmpeg.org/wiki/Encode/H.264

# Installation
Run the following command on Terminal:
```bash
$ source <(curl -s https://raw.githubusercontent.com/ma77os/video-conversor/master/install)
```

# Usage
- Without parameters, converts all MOV files located in the current folder to MP4 and WEBM with variable bitrate of 3MB:
```
$ video-conversor
```
- Specify desired bitrate using parameter "-b 0000k". In the following example, converts all MOV files to MP4 and WEBM using bitrate of 2MB:
```
$ video-conversor -b 2000k
```
- Specify an input format using "-i format" and output format using "-o format". Here, converts all MP4 files to WEBM:
```
$ video-conversor -i mp4 -o webm
```
- If you want to remove audio, pass parameter "-a". Here, converts all MP4 files to MP4 **without audio**:
```
$ video-conversor -a -i mp4 -o mp4
```


# Dependencies
- [Homebrew](https://brew.sh/)
- [FFmpeg](https://www.ffmpeg.org/)
