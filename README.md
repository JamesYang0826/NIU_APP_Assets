# NIU_APP_Assets


-----
ffmpeg -i 03.mp4 -vf "fps=15,scale=1080:-1:flags=lanczos,palettegen" -y palette.png  
ffmpeg -i 03.mp4 -i palette.png -lavfi "fps=15,scale=1080:-1:flags=lanczos [x]; [x][1:v] paletteuse" 03.gif

