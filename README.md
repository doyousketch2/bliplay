bliplay
=======

This program was build to play CSV like sound files to test the BlipKit library.
Some example files are located in `examples`.

1. Install SDL
--------------

For simplyfing the audio output on a wide range of systems the program uses SDL
(<http://www.libsdl.org>). If not already, you have to install it to be able to
run the program.

2. Checkout BlipKit
-------------------

BlipKit is the core library which generates the sound. It is added as a `git`
submodule. The source is fetched with this commands:

	$ git submodule init
	$ git submodule update

3. Building
-----------

First execute `autogen.sh` in the base directory to generate the build system:

	$ sh ./autogen.sh

Next execute `configure` in the base directory:

	$ ./configure

Then execute `make` to build the program in the `bliplay` directory:

	$ make

4. Playing files
----------------

Files can be played like this:

	bliplay$ ./bliplay -p examples/wysiwyg.blip
