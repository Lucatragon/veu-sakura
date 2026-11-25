# Update History
#### Marked with 
<ol>🟢 is completed. This means no future iterations of this will be included in this current version.</ol>
<ol>🔵 is current. This means it is in the Stable branch.</ol>
<ol>🟠 is not released yet or unstable. This means it is normally in the Unstable branch. You may see the Unstable version number go up repeatedly, even rapidly. This is normal.</ol>
<ol>🔴 is not worked on. This means you cannot access versions that are labeled red.</ol>

<ol>! Versions are NOT sequential. 00000 is before 00005, but there are not [normally] 6 updates (0, 1, 2, 3, 4, 5) in between. There are cases where there ARE indeed 6 updates, typically typo fixes and management. Actual architectural changes typically change the version number to a higher amount than typo fixes or most minor bug fixes.</ol>

<ol>? Why not use actual version numbers? While it is easier to write and comprehend strings such as <strong>0.14.29</strong> or <strong>2.6.126</strong>, the versioning method used for Anya is more linear on the roadmap, and any bumps along the way cannot be mistaken for actual planned updates if logged correctly. Otherwise without proper logging, there is no way to porperly tell the difference between 0.69.420 and 0.69.421 when the roadmap was set to begin itterating say, another feature. </ol>

### Current Version: ``Alpha Mars 0.8``
#### Version Code: ``-00001 (Pre-Beta Pre-Release)`` <br><br><br>

## 🔵 Alpha (Mars)
#### 🔵 Alpha 0 (pending update confirmation)
* Introduced commands. Learn more [here](https://github.com/Lucatragon/veu-anya/wiki/Commands).
* Introduced license VFL2 and deprecated license AZGLv1. Learn more [here](./LICENSE).
* Made a wiki for organization. Learn more [here](https://github.com/Lucatragon/veu-anya/wiki/Home).
* Renamed Artzenith Sound to Veu Demeteria. Closed issue [#1](https://github.com/Lucatragon/veu-anya/issues/1).
* (0.2) Renamed Veu Demeteria to Veu Kiri. Closed issue [#2](https://github.com/Lucatragon/veu-anya/issues/2).
* (0.8) Renamed Veu Kiri to Veu Anya. Closed issue [#4](https://github.com/Lucatragon/veu-anya/issues/4).
* (0.8) Added a logo in PNG form. See [this image](/ext-source/logo.png).
#### 🔴 Alpha 1 (Mars 1) (pending update initialization)
* (1.0) Prototyping in Turbowarp
  * This involves getting the ``.aso`` and ``.asn`` files put in place for first initialization
  * Will utilize PCM WAV Audio and a MIDI-like file format system to host audio files to try to make a song
  * (1.2) Watchdog needs developing
    * Will attempt to complete in a later update
    * Watchdog does not need developing yet until I can confirm ``.aso`` and ``.asn`` file initialization.
  * (1.4 - 1.7) Idea:
    * ``.asp`` (Anya Sound Pack) could be a file format that allows ``!Instrument`` labels to be hosted separately, and the ASP code could be in a function call (e.g. soon, there would be a way to go inside of ``.aso`` and ``.asn`` files and make the ``!Instrument`` label call a ``.asp`` file with a specific ``.asp`` code, and then ``Factors`` (``F0``, ``F1``, etc, inside of ``!Chart``) could be any number possible because instruments could just require an ID, the ID could get called, and if the ID cannot be found, a fallback ``Factor`` could be implemented.
    * Example given in Figure 1.
  * Any bugs must be at least looked at and graded in ``Issues`` before continuing to Saturn 0000, actual release.
  * Most if not all function-related bugs must be solved before continuing to Saturn 0000, actual release.
* (1.9) Most if not all generalized bugs must be at least looked at and graded in ``Issues`` before continuing to Saturn 0000, actual release.
* (00000) Actual release of Saturn v0 (Core) must be functional in both Windows 10, Windows 11 environments, and Debian Linux, with planned support for further operating systems, distributions and kernels later down the line.
   
Figure 1: Tadashii (C/Ruby hybrid) code that could be an example function for calling an ``.asp`` file.
```tadashii
!Instrument
    Instrument Flute fn[a](require asp flute.e359) : iF
    Instrument Drums fn[a](require asp drums_synth.e359): dS
```
<br>

### Naming convention for Non-Alpha, such as Beta, Centuri, Fault, and Ignis
```
00           000
Major        Minor
Release      Release

Example: 0010 = Saturn (0, 1) + Minor Release Code 0010 (Beginning of
repo, bug fixes are similar in number but major releases involve higher
number jumps, so 6225 to 6331 is a bigger jump in changes than 6225 to
6278).

0   1        Saturn (Beta)
2   3        Jupiter (Post-Beta Pre-Official Release)
4   5        Neptune (Release)
6            Pluto
7   8        Luna
9            Eclipse
10           Sol
11           New Eclipse
12           Ignis
...          ...

* some of these version names might not be used, or may be used early, or
late.

* if it is apparent not every feature has been added to the roadmap but the
versioning number is close to moving to a new major release, updates may be
halted, slowed or less common until new major release.

* versions can be referred as a 5 digit decimal number or a 4 digit decimal
number, both are the same, until Sol 000 releases, in which case it will be
referred as a 5 digit number, in this case, 10000.
```

## 🔴 Beta (Saturn)
#### 🔴 Beta 0010 (Pending completion of tasks instructed by Mars 1.0; requires Watchdog completion for Windows or Linux systems {WSL might have support, research further})
* Referring to 00000 as a reference, promote to 00010 if Watchdog has been completed for Windows (10 and 11, potential support for 8 and older) and Linux (Debian/Mint, Arch, Fedora), with potentially looking at BSD and other systems alike.
* If supported, allow Android and iOS to recieve development (Mobile device development will be introduced with an M next to the update name, example, ``00015M``, which is not related to update ``00015`` unless stated otherwise.
* If supported, consider compatibility with Sony Interactive Entertainment's PlayStation, and Microsoft's XBox consoles, alongside potential Nintendo Switch (1 and 2) support if not older hardware in general, such as the Nintendo DS, XBox 360 or SIE PlayStation 3.
