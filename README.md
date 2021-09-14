# Steganography

Tools:
---------------

1.Steghide
-------------------

Steghide is a steganography program that hides data in various kinds of image and audio files , only supports these file formats : JPEG, BMP, WAV and AU. but it’s also useful for extracting embedded and encrypted data from other files.

>>> Installing

    sudo apt-get install steghide
    
>>> Useful commands:

<i><b> steghide --help </i></b>  : It will show all available commands. 





<br><br>
2.Foremost
-----------------

Foremost is a program that recovers files based on their headers , footers and internal data structures , I find it useful when dealing with png images.

>>> Install Command           

    sudo apt-get install foremost

>>> Useful commands:

<i><b>foremost -i file_name </b></i>: extracts data from the given file.

<br><br>
3.Stegsolve
----------------
Sometimes there is a message or a text hidden in the image itself and in order to view it you need to apply some color filters or play with the color levels. You can do it with GIMP or Photoshop or any other image editing software but stegsolve made it easier. it’s a small java tool that applies many color filters on images. Personally i find it very useful. You can get it from <a href="https://github.com/eugenekolo/sec-tools/tree/master/stego/stegsolve/stegsolve"> GITHUB </a>.

<br><br>
4.Strings
------------
Strings is a linux tool that displays printable strings in a file. That simple tool can be very helpful when solving stego challenges. Usually the embedded data is password protected or encrypted and sometimes the password is actaully in the file itself and can be easily viewed by using strings
It’s a default linux tool so you don’t need to install anything.

>>> Useful commands:    
         
<i><b>strings file_name </b></i>: displays printable strings in the given file.


<br><br>

5.Exiftool
----------------
Sometimes important stuff is hidden in the metadata of the image or the file , exiftool can be very helpful to view the metadata of the file.You can download it in windows. You can get it from <a href="https://exiftool.org/"> here </a>.

>>> Install in linux:

    sudo apt-get install exiftool

>>>Useful commands:

<i><b>exiftool file </b></i>: shows the metadata of the given file

<br><br>
6.Exiv2
-----------
A tool similar to exiftool.

>>>Linux Install:

    sudo apt-get install exiv2

>>>Useful commands:


<i><b>exiv2 file </b></i>: shows the metadata of the given file


<br><br>
7.Binwalk
-------------

Binwalk is a tool for searching binary files like images and audio files for embedded files and data.

>>> Install in Linux:

    sudo apt-get install binwalk

>>>Useful commands:

<i><b>binwalk file </i></b>: Displays the embedded data in the given file
<i><b>binwalk -e file </i></b>: Displays and extracts the data from the given file

<br><br>

8.Zsteg
--------------

zsteg is a tool that can detect hidden data in png and bmp files. The source can be found on <a href="https://github.com/zed-0xff/zsteg">github</a>

>>>Install in Linux:

    gem install zsteg

>>>Useful commands:

<i><b>zsteg -a file </i></b>: Runs all the methods on the given file
<i><b>zsteg -E file </i></b>: Extracts data from the given payload (example : zsteg -E b4,bgr,msb,xy name.png)

<br><br>

9.Wavsteg
---------------
WavSteg is a python3 tool that can hide data and files in wav files and can also extract data from wav files.
You can get it from <a href="https://github.com/ragibson/Steganography#WavSteg"> here </a>

>>> Useful commands:

<i><b> stegolsb wavsteg --help </i></b>: extracts data from a wav sound file and outputs the data into a new file


<br><br>
10.Sonic visualizer
---------------------
Sonic visualizer is a tool for viewing and analyzing the contents of audio files, however it can be helpful when dealing with audio steganography. You can reveal hidden shapes in audio files.It is a GUI based tool. <br>
<a href="https://www.sonicvisualiser.org/">Official Website</a>

 
<br><br>

11.file
-----------------------
file command is used to determine the type of a file. .file type may be of human-readable(e.g. ‘ASCII text’) or MIME type(e.g. ‘text/plain; charset=us-ascii’). This command tests each argument in an attempt to categorize it.

12.cmp
----------
cmp command in Linux/UNIX is used to compare the two files byte by byte and helps you to find out whether the two files are identical or not.

>When cmp is used for comparison between two files, it reports the location of the first mismatch to the screen if difference is found and if no difference is found i.e the files compared are identical.
>cmp displays no message and simply returns the prompt if the the files compared are identical.

    cmp --help

<br><br>
13.diff
-----------------
diff stands for difference. This command is used to display the differences in the files by comparing the files line by line.

>>>Usage:

<i><b> diff a.txt b.txt </i></b> : it will compare a.txt and b.txt .




BRUTEFORCERS
------------------
<br><br>
1.Fcrackzip
---------------
Sometimes the extracted data is a password protected zip , this tool bruteforces zip archives.

>>>Install

    sudo apt-get install fcrackzip 

>>>Useful commands:

<i><b> fcrackzip -v -u -D -p /usr/share/wordlists/rockyou.txt Impossible.zip </i></b>: bruteforces the given zip file with passwords from the given wordlist .



<br><br>

2.Stegcracker
---------------------
A tool that bruteforces passwords using steghide.

>>>Usage

<i><b> stegcraker image.png wordlists.txt</i></b> : It will crack password of image.png which is password protected and it will use wordlist.txt as a wordlist.



<br><br><br>

Web Tools
---------------------
<br><br>
1.<a href="https://www.irongeek.com/i.php?page=security/unicode-steganography-homoglyph-encoder">Unicode Text Steganography</a>  
-----------------------------------------------------------------------------------------------------------------------------------
A web tool for unicode steganography , it can encode and decode text.

<br><br>
2.<a href="https://www.bertnase.de/npiet/npiet-execute.php">  Npiet Online</a>
--------------------------------------------------------------------------------------
an online interpreter for piet. piet is an esoteric language , programs in piet are images. Read more about it <a href="https://www.dangermouse.net/esoteric/piet.html"> here </a>.


<br><br>

3.<a href="https://www.dcode.fr/en"> dcode.fr </a>
--------------------------------------------------------
Sometimes when solving steganography challenges you will need to decode some text. dcode.fr has many decoders for a lot of ciphers and can be really helpful.


















<b><i>Source</b></i>
-----------------------
<i><u> 1. https://0xrick.github.io/lists/stego/</i></u>
<i><u> 2. https://www.geeksforgeeks.org </i></u>














