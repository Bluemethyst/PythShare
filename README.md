# PythShare
A minimal ShareX custom uploader that fits neatly into one python file using Flask.
## Installation
Create a docker-compose.yml file with the contents from [here](/docker-compose.yml) or below.
```yml
services:
  pythshare:
    container_name: pythshare
    image: bluemethyst/pythshare:1.0.0
    restart: always
    environment:
      - FLASK_ENV=development
    ports:
      - "5000:5000"
    volumes:
      - /srv/docker/pythshare/uploads:/app/uploads
```
## ShareX Setup
The setup for a custom ShareX uploader is below. You can set the name to whatever you'd like!

![ShareX Setup](https://raw.githubusercontent.com/Bluemethyst/PythShare/refs/heads/main/01_19_25_12-38.png)
