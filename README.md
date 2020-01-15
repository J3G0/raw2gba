# raw2gba

Converts raw files into an array of C bytes (can be used for loading sound files
into the Game Boy Advance).

This program only relies on gcc.  To compile, run make. However in this repo, I included a compiled .exe for windows users.

## Usage
First of all you need to convert the audio file (.mp3, .wav,...) to a .raw file.
The program I used is [Switch Sound File Converter](https://www.nch.com.au/switch/).
<br/>
<img src="https://github.com/J3G0/raw2gba/blob/master/misc/switch.png">
<br/>
Select the .raw file extention and use the signed 8-bit mode when converting your audio. 
Otherwise you'll find yourself with distorted audio on the GBA.
<br/>
<img src="https://github.com/J3G0/raw2gba/blob/master/misc/settings.png">
<br/>
To convert a raw file to a .h file for usage in programming for a GBA you use the following command:

```
raw2gba sound.raw
```
(Path variables might need to be added if an error occurs)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

* [Ian Finlayson](https://github.com/IanFinlayson) started this.
* Used in [The Unfair Game](https://github.com/J3G0/gba-sprite-engine).
* Thanks to the people who made the music and sound effects that are used. Links are in the
respectable .h files in the [Sounds](https://github.com/J3G0/raw2gba/tree/master/Sounds) folder. These are left in there to act as an example.
