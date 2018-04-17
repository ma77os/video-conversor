# Video Conversor
Convert movies to MP4 and WEBM with FFmpeg

# Installation
Run the following command on Terminal:
```bash
source <(curl -s https://raw.githubusercontent.com/ma77os/video-conversor/master/install)
```

# Usage
```
Usage: video-conversor <[-a -b:<value> -i:<format> -o:<format> -h ]>
Options:
        -a              Converts video without audio.
        -b:<value>      Sets the desired bitrate. Default is 3000k
        -i:<format>     Specify the input video extension. Default is .mov
        -o:<format>     Specity the output video format, use mp4, webm or both. Default is both.
        -h              Show this message
```

# Dependencies
- [Homebrew](https://brew.sh/)
- [FFmpeg](https://www.ffmpeg.org/)
