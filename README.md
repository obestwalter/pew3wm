# pew3wm

A [py3status](https://github.com/ultrabug/py3status) module using the PewPew hardware.

[![Travis CI status](https://api.travis-ci.org/obestwalter/pew3wm.png)](https://travis-ci.org/obestwalter/pew3wm)

## aims

* read button presses from a PewPew and use it to control i3wm
* display workspace on PewPew display

## install

We wish:

    $ pip install py3status-pewpew

But at the moment, clone repo and `tox -e deploy` :)


# testing

run the tests with tox:

```console
$ cd </path/to/this/repo>
$ tox
```

## development

install a development environment:

```console
$ cd </path/to/this/repo>
$ tox -e dev
```

... and activate it e.g via `source .tox/dev/bin/activate`. Then run tests with `pytest`.

# random

[python-evdev](https://python-evdev.readthedocs.io/en/latest/index.html)

experimenting with controlling i3wm with pewpew and creating a py3status module for it.

Starting from [this gist](https://gist.github.com/hbrylkowski/3ea9c65b672748b4f6a85074dd6ee311) to get the button events

This works when setting the pewpew to the gamepad mode (doing this directly on the pewpew).

Debugging hints:

    $ screen /dev/ttyACM0   # open a screen session. May need to reboot and/or hit Ctrl+C if are not greeted by a welcome message

