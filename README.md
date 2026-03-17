# Contents
- [Peace Equalizer APO Extension - source sync](#peace-equalizer-apo-extension---source-sync)
- [Peace/ReadmePeace.txt](#peacereadmepeacetxt)
- [Peace/Readme How to compile.txt](#peacereadme-how-to-compiletxt)

---

# Peace Equalizer APO Extension - source sync

This repo is an automated mirror that synchronizes the source code of [Peace Equalizer APO extension](https://sourceforge.net/projects/peace-equalizer-apo-extension/) from SourceForge to GitHub.

## How it works

A GitHub Action runs daily:

1. Calculates the MD5 hash of the latest source code archive on SourceForge
2. If a new version is detected, it downloads and extracts it into the `upstream/` directory.
3. It creates a new branch and opens a Pull Request with the updated source code.

## Setup Requirements

For the automation to function correctly, you must enable Pull Request permissions for GitHub Actions:

1.  Go to your repository **Settings**.
2.  Navigate to **Actions** > **General**.
3.  Under **Workflow permissions**, ensure **Allow GitHub Actions to create and approve pull requests** is checked.
4.  Click **Save**.

---

# Peace/ReadmePeace.txt
## v1.6.9.11

### Peter's Equalizer APO Configuration Extension (Peace)

An equalizer and effects interface for Equalizer APO by Peter Verbeek

- Peace http://sourceforge.net/projects/peace-equalizer-apo-extension
- Equalizer APO http://sourceforge.net/projects/equalizerapo

### Installation:
Run `PeaceSetup.exe` to install. Or move a downloaded executable `Peace.exe` to `Program files\EqualizerAPO\config` and run it.

When you start Peace for the first time, you may get a popup question `Overwrite config.txt?`. Saying `Yes` will activate Peace.

---

# Peace/Readme How to compile.txt
## v1.6.9.11

How to compile:

- Install AutoIt version 3.3.14.5
- Install the AutoIt IDE SciTE4AutoIt3
- Create an AutoIt development folder for instance `c:\users\Peter\Documents\AutoIt`
- Download `Source code.zip` from the Peace website (Files -> Source code) (**or clone this GitHub repo with source already in it**)
- Unzip it to your Autoit development folder extracting the folder tree

You should at least have this folder tree and files:

```
c:\users\Peter\Documents\AutoIt
  AutoIt Library
    Dialogue.au3
    NumberBox.au3
    String and File String.au3
  Knobs
    Images  (containing .png files)
    Knobs.au3
  Midi
    API  (containing MIDI library files)
    UDF  (containing MIDI library files)
  Peace
    7z  (containing 7za.exe)
    AutoEQ  (containing AutoEQ data files)
    Configurations  (containing .peace files and a zip file)
    DevicePeakValues  (containing DevicePeakValues32.dll and DevicePeakValues64.dll)
    DirectSound  (containing DirectSound.au3 and DirectSoundConstants.au3)
    Help  (containing peace.chm)
    Images  (containing .png and .ico files)
    Include  (containing some files to include)
    Languages  (containing .plf language files and EqualizeAPOcommands file)
    Sounds  (containing sound files, this folder is needed from Peace 1.5.3.2)

    Peace.au3
    _inputmask.au3  (only needed for version 1.6.1.2 and lower)
    GUIScrollbars_Ex.au3
    midiImproved.au3
    ReadmePeace.txt
```

Now start up the AutoIt IDE and open Peace.au3 and hit F5 to run.

When using another older Peace version download it a rename it to Peace.au3.

---

## License

This project is licensed under the GNU General Public License v2.0 (GPL-2.0).
