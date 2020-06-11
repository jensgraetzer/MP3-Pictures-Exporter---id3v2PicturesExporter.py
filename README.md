# MP3-Pictures-Exporter

The python script __id3v2PicturesExporter.py__ exports the pictures contained in ID3v2 tag of a MP3
file. It exports the pure MP3 audio data as well. Only tag versions ID3v2.3 and ID3v2.4 are
supported.

# Audio and pictures export with Id3v2PicturesExporter

Nowadays MP3 audio files contain text and maybe pictures as well. These additional data is stored in the so called ID3v2 tag [1, 2, 3]. The text is such metadata as the album, artist, songname, and so on.  ID3v2 tags bay be contain subtitles as well, and many more information. There may be even one or more pictures stored. This way, MP3 files with a ID3v2 tag are examples of multimedia data stored in a single file [4].

This version of id3v2PicturesExporter.py assumes the ID3v2 tag to be at the beginning of the MP3 file. It does not support ID3v2 tags at the end oft the MP3 file.

Usage: Run the script id3v2PicturesExporter.py. A file picker opens. Pick a MP3 file an press the “open” button. The script shows all frame names in the output and writes audio and picture files. The file names of these files start with “PPP_”.
Try id3v2PicturesExporter.py with the sample data attached.

# Sample MP3 files

* sample01_Kiss_the_Sky.mp3
The ID3v2.4 contains a bigger picture, format 16:9.
* sample02_C_Major_Prelude.mp3
The ID3v2.4 contains six bigger pictures, format 16:9 and subtitle text in a SYLT frame.
* ![sample03_Presentation.mp3](https://github.com/jensgraetzer/MP3-Pictures-Exporter/blob/master/sample03_Presentation.mp3)
The ID3v2.4 contains four bigger pictures, format 16:9 and subtitle text in a SYLT frame.
* sample04_Karaoketext.mp3
The ID3v2.4 contains one little picture 600x600 pixel and a subtitle text in a SYLT frame. The subtitle contains a time stamp for every single word.

# References
1. M. Nilsson, Informal Standard: ID3 tag version 2.4.0 - Main Structure, 2000,
https://id3.org/id3v2.4.0-structure (last visited 2020-06-11)
2. M. Nilsson, Informal Standard: ID3 tag version 2.4.0 - Native Frames, 2000,
https://id3.org/id3v2.4.0-frames (last visited 2020-06-11) 
3. M. Nilsson, Informal Standard: ID3 tag version 2.3.0, 1999,
https://id3.org/id3v2.3.0 (last visited 2020-06-11) 
4. J. Grätzer, Multimedia Data Categories, 2020
https://github.com/jensgraetzer/MP3-Pictures-Exporter/blob/master/Multimedia-Data-Categories.pdf (last visited 2020-06-11)
