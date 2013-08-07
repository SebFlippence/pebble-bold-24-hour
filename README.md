# bold-24-hour

This is a [pebble](http://getpebble.com) watchface which displays a large, watch-face-sized, bold hour and a smaller minute number in the center of the hour. Works in 12 and 24 hour modes (use pebble settings to change).

This is a 24 hour fork of the 12 hour version by [yanatan16](https://github.com/yanatan16/pebble-bold-hour).

_Note_: Last built with version 1.12

## My Pebble Faces

Get and Vote for this face on mypebblefaces.com:
- [white numbers](http://www.mypebblefaces.com/view?fID=5426&aName=seb&pageTitle=Bold+24+Hour+%28White%29&auID=6482)
- [black numbers](http://www.mypebblefaces.com/view?fID=5426&aName=seb&pageTitle=Bold+24+Hour+%28White%29&auID=6482)

## How to build

This watchface was compiled with Android SDK release 1.12. Make sure you setup the SDK according to [pebble's instructions](http://developer.getpebble.com). Then clone this repo (or your fork) into the watches directory. Then add the symlinks.

```
cd ~/pebble-dev/PebbleSDK-1.12/Pebble/watches
git clone http://github.com/sebflipper/pebble-bold-24-hour bold-24-hour
../tools/create_pebble_project.py --symlink-only ../sdk bold-24-hour
```

To set it up for white numbers make sure the `#define LIGHT_WATCHFACE` is _not_ commented, and make sure all the images in the resoure map have the `-inv.png` on the end, as in `bold-hour-5-inv.png`. For black numbers, do the opposite.

## License

Copyright (c) 2013 Seb Flippence, Jon Eisen

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
