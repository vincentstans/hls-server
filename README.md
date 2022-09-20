# hls-server
create hls streams and serve them
requires python3, ffmpeg, pv, sed.
source file must be greater than 1280x720

chmod +x bin/hls
bin/./hls VIDEO-source-FILE.mkv
Will create a Directory VIDEO-source-FILE ( as Title )
In there it creates 3 streams v0 ( source ) v1 ( 1280x720 ) v2 ( 640x380 )
It creates a VIDEO-source-FILE.html that will stream this video
It creates a index.html with links to all VIDEO-source-FILE.html files.
