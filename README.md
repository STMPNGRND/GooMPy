# GooMPy
Google Maps for Python

GooMPy provide a Python interface to the Google Static Maps API, automatically ownloading and stitching together map tiles into a single image that you can zoom and pan.  To support using maps when you don't have an internet connection, GooMPY provides a pre-fetching function that stores the tiles in a caching folder. 

You'll need the Python Image Library (PIL) or equivalent (Pillow for Windows and OS X) installed on your computer equivalent to run GooMPy.  The repository includes an example using Tkinter, though you should be able to use GooMPy with other toolkits like wx and Qt.

Because Google limits the number of tiles that you can download during a given time period, we recommend setting up an API key as described here:
  
  https://developers.google.com/maps/documentation/staticmaps/#api_key
  
Once you have your key, put it in the file goompy/key.py, and GooMPy will use it in fetching map tiles.  If you run out of downloads, the tiles will be black with a "capacity exceeded" image in them.

