FROM homeassistant/raspberrypi3-homeassistant
MAINTAINER Khanh Cao <khanhncao@gmail.com>
VOLUME /media

RUN apt-get update
RUN apt-get install apt-transport-https ca-certificates apt-utils -y
RUN apt-get upgrade -y
RUN apt-get remove pulseaudio -y
RUN apt-get install vlc alsa-utils -y
