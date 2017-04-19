FROM zorbash/kitto-rpi:latest

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && apt-get install -y \
  iceweasel xserver-xorg-core xserver-xorg-video-fbdev x11-xserver-utils \
  libgl1-mesa-dri matchbox-window-manager xautomation feh

ADD kiosk /bin/kiosk
ADD wallpaper.png /etc/wallpaper.png
ADD dot-mozilla /root/.mozilla

CMD ["/bin/kiosk"]
