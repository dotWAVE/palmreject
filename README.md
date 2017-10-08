# Palm rejection for bash and xinput

The code is tested on Ubuntu 17.04 with Gnome 3.

Depends only on bash and xinput.

Turns off touchscreen input when stylus is near screen.

Stylus status is checked every 100 ms, a timeout is by
default set to 2 seconds for re-enabling the touchscreen
after stylus input.

Additionally, if no pen device is found, it will check again every 2 seconds before starting palm rejection.

You need to check the ids for your devices.
Run "xinput list" on your system and edit the
first lines in palmreject.sh.
Then run the script every time you login.

