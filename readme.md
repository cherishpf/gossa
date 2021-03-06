gossa
=============

![e](https://user-images.githubusercontent.com/760637/52522293-942fa880-2c83-11e9-9f79-0a5b922bcc7f.gif)

[![Build Status](https://travis-ci.org/pldubouilh/gossa.svg?branch=master)](https://travis-ci.org/pldubouilh/gossa)

🎶 A fast and simple webserver for your files, that's dependency-free and with under 210 lines for the server code, easily code-reviewable.

### features
  * 🔍 files/directories browser
  * 📩 drag-and-drop file/directory uploader
  * 🗺️ files handling - move/rename/delete
  * 📸 picture browser
  * 📽️ video streaming from the browser
  * ✍️ simple text editor
  * ⌨️ keyboard shortcuts
  * 🥂 speed - showed rates above 100MB/s

### built blobs
built blobs are available on the [release page](https://github.com/pldubouilh/gossa/releases).

### run
```sh
# build (or download release from github)
make

# run
./gossa -h 192.168.100.33 ~/storage
```

### ui shortcuts
|shortcut | action|
| ------------- |-------------|
|click new folder icon | create new folder|
|click pad icon | open file editor|
|click file icon  | rename item|
|double click file icon | delete item|
|drag-and-drop item on UI | move item|
|drag-and-drop external item | upload file/folders|

### keyboard shortcuts
|shortcut | action|
|-------------|-------------|
|Arrows/Enter | browse through files/directories and pictures|
|Ctrl/Meta + C | copy URL to clipboard|
|Ctrl/Meta + E | rename file/folder|
|Ctrl/Meta + Del | delete file/folder|
|Ctrl/Meta + U | upload new file/folder|
|Ctrl/Meta + D | create a new directory|
|Ctrl/Meta + X | cut selected path|
|Ctrl/Meta + V | paste previously selected paths to directory|
|\<any letter\> | search|

### using with docker
a few docker/docker-compose files are provided in the [docker folder](https://github.com/pldubouilh/gossa/tree/master/docker). release images are also pushed to [dockerhub](https://hub.docker.com/r/pldubouilh/gossa), e.g. :

```sh
# pull from dockerhub and run
sudo docker run -v ~/LocalDirToShare:/shared -p 8001:8001 pldubouilh/gossa
```
