MicroDVD to SRT converter
=========================

There is still MicroDVD formatted subtitles around (usually with ``.sub``
extension) although they are frames based, which makes them useless for same
movies with different frame rate. This is an converter for such subtitles to
widely used SRT format.

Requirements
============

Only Python interpreter is required.

Installation
============

No installation is required, although ``microdvd2srt.py`` might be placed in
one of ``$PATH`` locations for convenience.

Usage
=====

This script simply accepts subtitle file as an argument, so it is enough to:

.. code:: shell-session

   microdvd2srt.py file.sub

Converted subtitles will be write up on the stdout output in terminal. To write
it to destination file:

.. code:: shell-session

   microdvd2srt.py file.sub > file.srt

To change default frame rate, which is ``25``, use the ``-f`` option:

.. code:: shell-session

   microdvd2srt.py -f 23.976 file.sub > file.srt

License
=======

This software is licensed under 3-clause BSD license. See LICENSE file for
details.
