# ha-vlc
Homeassistant + VLC docker image

Docker compose example:
```yaml
  homeassistant:
    container_name: hass 
    image: kacao/ha-vlc
    volumes:   
      - /media:/media
      - ./ha/config:/config
      - /etc/localtime:/etc/localtime:ro
      - /dev/snd:/dev/snd
    restart: always
    networks:
      - local
    ports:
      - 8123:8123
    stdin_open: true
    privileged: true
    tty: true
```

For Raspiberry Pi, use `kacao/ha-vlc:rpi`
