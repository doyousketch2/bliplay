bliplay
=======

**bliplay** is a plaintext-based chiptune sound player. See the interactive player at <https://play.blipkit.audio> for examples and syntax description. Some example files also are located in [examples](examples).

1. Install SDL
--------------

For simplyfing the audio output on a wide range of systems the program uses SDL (<https://www.libsdl.org>). If not already, you have to install it to be able to
run the program.

2. Checkout BlipKit
-------------------

[BlipKit](https://github.com/detomon/BlipKit) is the core library which generates the sound. It is added as a submodule. To fetch its source, use the following command when cloning the **bliplay** repository:

```sh
git clone --recursive https://github.com/detomon/bliplay.git
```

or afterwards with:

```sh
git submodule update --init
```

3. Building
-----------

First execute `autogen.sh` in the base directory to generate the build system:

```sh
sh ./autogen.sh
```

Next execute `configure` in the base directory:

```sh
./configure
```

Then execute `make` to build the program in the `bliplay` directory:

```sh
make
```

4. Playing files
----------------

Some example files are located in `examples`. Use the following command to play them:

```Shell
bliplay/bliplay examples/hyperion-star-racer.blip
```


License
-------

This program is distributed under the MIT license. See `LICENSE`.
