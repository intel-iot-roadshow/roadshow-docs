# Getting Started Guides

If you're viewing this README from Github and not a supplied Roadshow USB thumb drive, go to https://github.com/ssg-drd-iot/getting-started-guides/releases to download the latest zip package.

Unzip the contents of the downloaded file to your **local** harddrive (not a USB drive).

## To view these docs offline

**Launch docs start page by viewing the local `index.html` from the zip in your web browser.**

## Alternative ways of viewing html docs

If you're running into issues viewing the docs, you can run a simple webserver in the root of the extracted files.

### Python web server

The simplest probably is to use Python's built-in http server. 

If you have [Python](http://python.org/) installed (it's built into Mac OS), it should be enough to `cd` into your unzipped folder and run this from a command line:

```bash
# Python 2.x
python -m SimpleHTTPServer
```

```bash
# Python 3.x
python -m http.server
```

This will serve files from the current directory at localhost under port 8000:

http://localhost:8000/

### Options for Windows

If you're on Windows and don't have Python installed, download and use [mongoose](https://cesanta.com/mongoose.shtml).
