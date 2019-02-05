# Spotify Music Downloader (SMD) 
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<img align="center" src="https://i.ibb.co/j84F6HJ/image5.png">

## **Download your music in high quality**

<img align="center" src="https://i.ibb.co/BwgvL5R/result.png">

## Usage

```
./main.py [without any parameters] - normal startup

./main.py [parameter][argument] - startup with parameter

Parameters

  -h, --help       Print a help message and exit.

  -s, --song       Spotify song URI.

  -p, --playlist   Spotify playlist URI.

  -f, --file       File with song URIs.

```
## Installation

```
git clone https://github.com/artyshko/smd.git
```

### First you need to install all dependencies
```
pip3 install -r requirements.txt
```

### Make file executable
```
chmod +x main.py
./main.py
```
### Or use
```
python3 main.py
```
### How to get song URI

<img align="center" src="https://i.ibb.co/BzM7ZKp/image4.png">

### Example of Spotify URI Code
```
spotify:track:4tmwiN9YU7xMjh2hoqcVuI
```

### Song mode
Example:
```
./main.py -s spotify:track:7ARveOiD31w2Nq0n5FsSf8
```

### File mode
#### Create file with songs
<img align="center" src="https://i.ibb.co/JQsMCYV/image3.png">

Example:
```
./main.py -f songs.txt
```

### Playlist mode
#### Create playlist and make it secret
<img align="center" src="https://i.ibb.co/kBKtDys/image1.png">

#### Then copy playlist URI
<img align="center" src="https://i.ibb.co/yWHHBDX/image2.png">

Example:
```
./main.py -p spotify:user:spotify:playlist:37i9dQZF1DXcRXFNfZr7Tp

```


## **In case of `pytube.exceptions.regexmatcherror: regex pattern ("signature",\s?([a-za-z0-9$]+)\() had zero matches` try:**

```
pip3 install git+https://github.com/nficano/pytube.git
```