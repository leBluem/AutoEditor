AutoEditor v2.3 (3. jul 2019) by leBluem

Poor mans buggy Line Editor. Freeware program for automatic text manipulation via masks and counters.
Features: various searches+replaces, filter/sort/columnize, open save, browse ...
usefull for fast generating of a lot of text. Still unstable, I mostly use it copy/paste and per commandline

Uses custom ShellControls and SynEdit-2_0_8.zip Component from http://synedit.sourceforge.net

bugs
----
  maybe a lot

docu
----
  AutoEditor.exe file.ini /inicheck
  AutoEditor.exe file.ini /iniadd sectionname* key value
  i.e: AutoEditor.exe file.ini /iniadd LIGHT*,MATERIAL* ACTIVE 1
    euqals:
    AutoEditor.exe file.ini /iniadd "LIGHT*, MATERIAL*" ACTIVE 1

  This program was coded fast und dirty and comes with no doc, read history for feature overview.

history
-------
  v1.1 (30. Mar 2012)
    - first public release

  v1.2 (27. Jan 2018)
    - added sorting and more colunm options

  v1.3 (6. Aug 2018)
    - added INI renaming for [LIGHT_SERIES_] and [MATERIAL_ADJUSTMENT_]
      + counting more than one use of meshes+materials

  v1.4 (7. Aug 2018)
    - bugfix, column-replacement was not working

  v1.5 (7. Aug 2018)
    - add/change line for INI sections

  v1.6 (17. Aug 2018)
    - ini functions now compatible with 'name = value' / 'name=value'
    - added commandline parameters for the two INI-functions:
      AutoEditor.exe file.ini /inicheck
      AutoEditor.exe file.ini /iniadd sectionname* key value
      i.e: AutoEditor.exe file.ini /iniadd LIGHT*,MATERIAL* ACTIVE 1
           euqals:
           AutoEditor.exe file.ini /iniadd "LIGHT*, MATERIAL*" ACTIVE 1
      now you can call autoeditor with autoeditor!
    - added (buggy) application skinning/themes (right click on title bar)

  v1.7 (18. apr 2019)
    - added "only if exists" and "invert section" options in ini dialog
    - removed application skinning/themes (right click on title bar)
    - added scanning KN5/FBX files: if kn5: unpack, if binary fbx, convert to ascii,
      scan fbx -> list of Meshes and Materials + dds filenames

  v1.8 (19. apr 2019)
    - fixed fbx scanning

  v1.9 (19. apr 2019)
    - fixed editor stuff
    - keeping selection after deleting is a feature not a bug

  v2.0 (2. may 2019)
    - fixed loading files
    - F7 with selection opens INI change-dialog, now scrolls to first found item on section change
    - F8 ini rename (only for somme keywords from assetto, not gernalized)
    - F9 scan fbx/kn5 (leaving behind trash from unpacking)

  v2.1 (5. may 2019)
    - finally fixed saving files, now its a real editor ;)
    - fixed other stuff + improved search and ini change dialog

  v2.2 (6. may 2019)
    - enabled that save button

  v2.3 (3. jul 2019)
    - ini-changer: added option to filter by section content; +fixes

  v2.5 (19. dec 2020)
    - sanity and performance update

  v2.8 (apr 2022)
    - more stable

  v3.0 (june 2022)
    - fixed line unify feature

  v3.1 (feb 2023)
    - finally fixed line unify feature
