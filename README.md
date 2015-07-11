# Getting Started Guides

To view these docs offline, download a zip of the 'html' branch by clicking on the "Download zip" button to the left.

Unzip the downloadeded file and run a simple webserver in the root of the extracted files.

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
