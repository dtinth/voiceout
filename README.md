
# Voice Out - an HTML5 Web Audio API Demo

This web application lets you play a song and filter out voice
(and some other instruments) in real time.

  * Only tested on __Google Chrome__.
  * The file must be __stereo__.
  * The file must have __resonable quality__.

This application works by subtracting the wave of the right channel
from the left channel.
Most songs have the vocal track on the center,
so the waveform of these sounds are the same in both left and right channel.
When we subtract one from another, they interfere destructively,
thus removing the sound.

In addition to vocals, I found out that these instruments are usually
center-panned (meaning they too will be filtered out):

  * Bass
  * Kick Drum
  * Lead Guitar

On the other hand, these sounds are usually NOT center-panned, and remains
in the song (some even stand out):

  * Piano
  * Crash Cymbals
  * Some Hihats
  * Synthesizers
  * Strings
  * Rhythm Guitar

