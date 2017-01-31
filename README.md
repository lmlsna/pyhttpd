# pyhttpd
A small, portable, python HTTP server utility for displaying static text, doing redirects, or listing a directory.
Usage: pyhttpd [options]

Options:
  -h, --help            show this help message and exit
  -b HOST, --bind=HOST  Bind server to this ip address
  -p PORT, --port=PORT  Listen for connection on this port
  -t TEXT, --text=TEXT  Text to return in "text" mode
  -r REDIRECT, --redirect=REDIRECT
                        Location to redirect to when in "redirect" mode
  -f FILE, --file=FILE  Print the contents of this file when in "file" mode
  -d DIR, --dir=DIR     Serve the contents of this directory when in "dir"
                        mode
  -D, --daemon          Fork process to the background
