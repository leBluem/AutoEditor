# AutoEditor

download: https://github.com/leBluem/AutoEditor/releases

Poor mans line/text editor. Freeware program for automatic text manipulation via masks and counters. INI manipulation, search and replace, filter, open save, browse ... usefull for fast generating of a lot of text. Uses custom SynEdit Component from http://synedit.sourceforge.net and ShellControls. Bugs - there are a lot, save or copy often! Check results! No guaranties! Use at your own risk!

Some special use case for kn5/fbx files, it tries to open them too, it uses included "Kn5Unpack.exe" and "fbxConvert.exe" : if kn5: unpack, if binary fbx, convert to ascii, then it scan's the resulting ascii fbx and you get a list of Meshes and Materials + existing dds filenames (leaving behind the unpacked stuff, if kn5 ;) ).

doc - This program was coded fast und dirty and comes with no doc, read history in relase archive for feature overview.

source - its a mess, i you really want it contact me - its in delphi with lots of custom components...

command line parameters:

- this will load "file.bin" into AutoEditor, like with normal programs:
```
AutoEditor.exe file.bin
```
- this will insert a line "ACTIVE=1" in matching sections and exits AutoEditor after file was written:
```
AutoEditor.exe file.ini /iniadd sectionname* ACTIVE 1
```
- this will change only existing values in matching sections and exits AutoEditor after file was written:
```
AutoEditor.exe file.ini /inichange sectionname* RENDERABLE 0
```
- hint:
```
AutoEditor.exe file.ini /iniadd LIGHT*,MATERIAL* ACTIVE 1
is the same as:
AutoEditor.exe file.ini /iniadd "LIGHT*, MATERIAL*" ACTIVE 1
```

Advanced INI-change dialog, you can use wildcards like ? and * everywhere in this dialog (except "Value" of course):
![Imgur Image](https://i.imgur.com/QkPoZCN.png)

Section Generation with a mask:
![Imgur Image](https://i.imgur.com/yIIwrdw.png)

v2.6: added list to ini-change dialog
usefull for a list of meshes and mass-adjusting i.E. LOD_OUT values in existing ".fbx.ini" persistence files
![Imgur Image](https://i.imgur.com/49yb0QS.png)

