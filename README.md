# Steganography

Tools:
---------------
1.Steghide
-------------




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
