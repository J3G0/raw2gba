# raw2gba

Converts raw files into an array of C bytes (can be used for loading sound files
into the Game Boy Advance).

This program only relies on gcc.  To compile, run make.

## Usage
First of all you need to convert the audio file (.mp3, .wav,...) to a .raw file.
The program I used is (Switch Sound File Converter)[https://www.nch.com.au/switch/].
Select the .raw file extention  and use the signed 8-bit mode when converting your audio. 
Otherwise you'll ind yourself with  distorted audio on the GBA.

To convert a raw file to a .h file for usage in programming for a gba you use the following command:

```
raw2gba sound.raw
```
