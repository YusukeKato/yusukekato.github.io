# FFmpeg
Official website: [ffmpeg.org](https://www.ffmpeg.org/)

## resize
```sh
# w=500, h=500
ffmpeg -i input.jpg -vf scale=500:500 output.jpg
# w=500
ffmpeg -i input.jpg -vf scale=500:-1 output.jpg
# h=500
ffmpeg -i input.jpg -vf scale=-1:500 output.jpg
```
