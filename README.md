# nms-desktop
## Install

* Open a terminal

* git clone https://github.com/nextsigner/nms-desktop.git

* cd nms-desktop

* npm install

## Init Desktop Stream

* Open other terminal
* ffmpeg -y -re -video_size 1280x720 -framerate 25 -f x11grab -i :0.0 -f pulse -i alsa_output.pci-0000_00_1f.3.analog-stereo.monitor -c:v libx264 -preset veryfast -f flv rtmp://localhost/live/stream

Note: Set screen resolution with your screen width and height.
