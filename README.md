# pyhttpd
A small, portable, python HTTP server utility for displaying static text, doing redirects, or listing a directory.

## Usage
```
Usage: pyhttpd [options]

Options:
  -h, --help              show this help message and exit
  -D, --daemon            fork process to the background

Bind Options:  
  -b HOST, --bind=HOST    bind server to this ip address
  -p PORT, --port=PORT    listen for connection on this port

Server Mode Options:  
  -t TEXT, --text=TEXT    text to return as page
  -r URL, --redirect=URL  location to redirect to
  -f FILE, --file=FILE    print the contents of this file
  -d DIR, --dir=DIR       serve the contents of this directory
```

## Bind Options
With no bind options (-b|p) set, pyhttpd will bind to all interfaces and listen on port 80 (if run as root) or port 8080.

## Server Modes
There are 4 available server modes, only one server mode option can be given at a time.
  * ```--text "text or html code"``` Will serve a page with the give text or code.
  * ```--redirect "URL"``` Will return a 301 redirect for the given URL.
  * ```--file``` Will server the contents of the given FILE.
  * ```--dir``` Will give a directory listing and server files within the given DIR.
  
If no server mode option (-t|r|f|d) is set, pyhttpd defaults to displaying the text "Hi!" as an HTML page.


