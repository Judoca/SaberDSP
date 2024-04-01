# SaberDsp
Real Time Digital Signal Processing specialized for audio signals

Tools used:
- portaudio	( https://github/PortAudio/portaudio )

## Configuring and Compiling PortAudio

-To be executed in the directory containing the home PortAudio files

```./configure && make```

## Using PortAudio in a project

- To install PortAudio

```sudo make install```

- Copying ```libportaudio.a```:

```cp lib/.libs/libportaudio.a /YOUR/PROJECT/DIR```
OR
```cp /usr/local/lib/libportaudio.a /YOUR/PROJECT/DUR```

- It is necessary to copy *portaudio.h* located in ```include/```

```gcc main.c libportaudio.a -lrt -lm -lasound -ljack -pthread -o YOUR_BINARY```
