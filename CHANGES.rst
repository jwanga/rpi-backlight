Changes
=======

2.7.0
-----

- Drop ``microsoft-surface-rt`` board type in favor of ``generic`` with support for Chromebooks (`#65 <https://github.com/linusg/rpi-backlight/pull/65>`_, `@archisman-panigrahi <https://github.com/archisman-panigrahi>`_)
- Add Raspberry Pi 5 support (`#66 <https://github.com/linusg/rpi-backlight/pull/66>`_, `@jamesecc <https://github.com/jamesecc>`_)

2.6.0
-----

- Add Python 3.11 as supported version, drop 3.6
- Add support for Microsoft Surface RT (`#54 <https://github.com/linusg/rpi-backlight/pull/54>`_, `@apandada1 <https://github.com/apandada1>`_)

2.5.0
-----

- Add Python 3.10 as supported version
- Support alternate backlight sysfs path (`#50 <https://github.com/linusg/rpi-backlight/pull/50>`_, `@j-coopz <https://github.com/j-coopz>`_)

2.4.1
-----

- Fix board type detection

2.4.0
-----

- Drop support for Python 3.5, which reached end-of-life in late 2020. Supported versions as of this release are 3.6 - 3.9
- Implement automatic board type detection (`#32 <https://github.com/linusg/rpi-backlight/pull/32>`_, `@p1r473 <https://github.com/p1r473>`_),
  passing a ``board_type`` to the constructor is no longer necessary in most cases, even when using an ASUS Tinker Board
- Fix setting brightness to max value and brightness fading loop condition (`#35 <https://github.com/linusg/rpi-backlight/pull/35>`_, `@Martin-HiPi <https://github.com/Martin-HiPi>`_)

2.3.0
-----

- Add support for ASUS Tinker Board 2 (`#29 <https://github.com/linusg/rpi-backlight/pull/29>`_, `@p1r473 <https://github.com/p1r473>`_)

2.2.0
-----

- Add toggle functionality to CLI (`#21 <https://github.com/linusg/rpi-backlight/pull/21>`_, `@p1r473 <https://github.com/p1r473>`_)
- Replace Travis CI with GitHub actions (`#20 <https://github.com/linusg/rpi-backlight/pull/20>`_, `@linusg <https://github.com/linusg>`_)
- Improve tests

2.1.0
-----

- Add support for ASUS Tinker Board (`#19 <https://github.com/linusg/rpi-backlight/pull/19>`_, `@p1r473 <https://github.com/p1r473>`_)

2.0.1
-----

- Add mypy type checking
- Add Python 3.8 to Travis CI config
- Fix documentation readthedocs build
- Fix typo in docs
- Improve README.md
- Mark project as stable on PyPI

2.0.0
-----

- New, more pythonic API
- Update CLI and GUI
- Support emulator
- Add tests

1.8.1
-----

- Fix float division issue with Python 2

1.8.0
-----

- Fix permission error inconsistency across Python versions
- Update link to PyPI

1.7.1
-----

- Fixed typo in ``CHANGES.rst``
- Fixed rendering of parameters and return types in the documentation

1.7.0
-----

- Fixed bug in ``get_power``, which would eventually always return False
- Added parameters and return types in docstrings

1.6.0
-----

- Added ``duration`` parameter to ``set_brightness``
- ``smooth`` now defaults to ``False``
- Huge improvements on CLI
- Fixed renamed function in examples
- Minor code and readme improvements

1.5.0
-----

- PR #3 by Scouttp: Fixed permission errors
- Added documentation
- Code improvements
- Fixed typos

1.4.0
-----

- Check for ``pygobject`` being installed
- Code cleanup
- README improvements

  - Added external links
  - Added badges
  - Fixed typos

- Moved to Travis CI and Landscape.io for builds and code health testing
- Prepared docs hosting at readthedocs.org

1.3.1
-----

- Fixed type conversion

1.3.0
-----

- Added experimental GUI (start with ``rpi-backlight-gui``)

1.2.1
-----

- Fixed CLI and typo

1.2.0
-----

- Added command line interface (``rpi-backlight`` and ``rpi-backlight-gui``)
- Code improvements - thanks to deets

1.1.0
-----

- Fixed ``set_power(on)`` function
- Added function to get the current power state of the LCD
- Added docstrings
- Code cleanup and improvements

1.0.0
-----

Initial release. Added necessary files and basic features:

- Change the display brightness smoothly or abrupt
- Set the display power on or off
- Get the current brightness
- Get the maximum brightness
