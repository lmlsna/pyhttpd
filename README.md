# pyhttpd
A small, portable, python HTTP server utility for displaying static text, doing redirects, or listing a directory.

# Usage
```
Usage: pyhttpd [options]

Options:
  -h, --help            show this help message and exit
  -b HOST, --bind=HOST  bind server to this ip address
  -p PORT, --port=PORT  listen for connection on this port
  -t TEXT, --text=TEXT  text to return as page
  -r REDIRECT,
  --redirect=REDIRECT   location to redirect to
  -f FILE, --file=FILE  print the contents of this file
  -d DIR, --dir=DIR     serve the contents of this directory 
  -D, --daemon          fork process to the background
```
