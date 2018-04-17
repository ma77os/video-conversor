# Video Conversor
Converts video files to MP4 and WEBM with 2 passes variable bitrate using FFmpeg

*MP4 conversion is H264 quicktime compatible*
- docs: https://trac.ffmpeg.org/wiki/Encode/VP9 / https://trac.ffmpeg.org/wiki/Encode/H.264
- author: @ma77os - André Mattos

# Installation
Run the following command on Terminal:
```bash
$ source <(curl -s https://raw.githubusercontent.com/ma77os/video-conversor/master/install)
```

# Usage
```
Usage: video-conversor <[-a -b <value> -i <format> -o <format> -h ]>
Options:
        -a              Converts video without audio.
        -b <value>      Sets the desired bitrate. Default is 3000k
        -i <format>     Specify the input video extension. Default is .mov
        -o <format>     Specity the output video format, use mp4, webm or both. Default is both.
        -h              Show this message
```

# Examples
- Without parameters, converts all MOV files located in the current folder to MP4 and WEBM with variable bitrate of 3MB
```
$ video-conversor
```
- Converts all MOV files to MP4 and WEBM with bitrate of 2MB
```
$ video-conversor -b 2000k
```
- Converts all MP4 files to WEBM only
```
$ video-conversor -i mp4 -o webm
```
- Converts all MP4 files to MP4 only **without audio**
```
$ video-conversor -a -i mp4 -o mp4
```


# Dependencies
- [Homebrew](https://brew.sh/)
- [FFmpeg](https://www.ffmpeg.org/)
