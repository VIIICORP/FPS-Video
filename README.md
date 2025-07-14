# Future Production Studio Video Editor

Future Production Studio Video Editor is an award-winning free and open-source video editor 
for Linux, Mac, and Windows, and is dedicated to delivering high quality 
video editing and animation solutions to the world.

## Build Status

<!-- TODO: Update badges to Future Production Studio repositories when available -->
[![fps-video CI Build](https://github.com/FutureProductionStudio/fps-video/actions/workflows/ci.yml/badge.svg)](https://github.com/FutureProductionStudio/fps-video/actions/workflows/ci.yml) 
[![libfps CI Build](https://github.com/FutureProductionStudio/libfps/actions/workflows/ci.yml/badge.svg)](https://github.com/FutureProductionStudio/libfps/actions/workflows/ci.yml) 
[![libfps-audio CI Build](https://github.com/FutureProductionStudio/libfps-audio/actions/workflows/ci.yml/badge.svg)](https://github.com/FutureProductionStudio/libfps-audio/actions/workflows/ci.yml)
<!-- TODO: Update Discord server ID for Future Production Studio Discord -->
![Discord](https://img.shields.io/discord/1143390791507644496?style=flat)

## Features

* Cross-platform (Linux, Mac, and Windows)
* Support for many video, audio, and image formats (based on FFmpeg)
* Powerful curve-based Key frame animations
* Desktop integration (drag and drop support)
* Unlimited tracks / layers
* Clip resizing, scaling, trimming, snapping, rotation, and cutting
* Video transitions with real-time previews
* Compositing, image overlays, watermarks
* Title templates, title creation, sub-titles
* 2D animation support (image sequences)
* 3D animated titles (and effects)
* SVG friendly, to create and include vector titles and credits
* Scrolling motion picture credits
* Advanced Timeline (including Drag & drop, scrolling, panning, zooming, and snapping)
* Frame accuracy (step through each frame of video)
* Time-mapping and speed changes on clips (slow/fast, forward/backward, etc...)
* Audio mixing and editing
* Digital video effects, including brightness, gamma, hue, greyscale, chroma key, and many more!
* Experimental hardware encoding and decoding (VA-API, NVDEC, D3D9, D3D11, VTB)
* Import & Export widely supported formats (EDL, XML)
* Render videos in many codecs and formats (based on FFmpeg)

## Getting Started

The quickest way to get started using Future Production Studio is to download one of 
our pre-built installers. On our download page, click the **Daily Builds** 
button to view the latest, experimental builds, which are created for each 
new commit to this repo.

https://www.futureproduction.com/download/

## Tutorial

Watch the official [step-by-step video tutorial](https://www.youtube.com/watch?list=PLymupH2aoNQNezYzv2lhSwvoyZgLp1Q0T&v=1k-ISfd-YBE), or read the official [user-guide](https://www.futureproduction.com/user-guide/):

## Developers

Are you interested in becoming more involved in the development of 
Future Production Studio? Build exciting new features, fix bugs, make friends, and become a hero! 
Please read the [step-by-step](https://github.com/FutureProductionStudio/fps-video/wiki/Become-a-Developer) 
instructions for getting source code, configuring dependencies, and building Future Production Studio.

## Documentation

Beautiful HTML documentation can be generated using Sphinx.

```sh
cd doc
make html
```

The documentation for the most recent release can be viewed online at [futureproduction.com/user-guide](https://www.futureproduction.com/user-guide/).

## Report a bug

Please report bugs using the official [Report a Bug](https://www.futureproduction.com/issues/new/) 
feature on our website. This walks you through the bug reporting process, and helps 
to create a high-quality bug report for the Future Production Studio community.

Or you can report a new issue directly on GitHub:

https://github.com/FutureProductionStudio/fps-video/issues

## Translations

Translating Future Production Studio into other languages is very easy! Please read the [step-by-step](https://github.com/FutureProductionStudio/fps-video/wiki/Become-a-Translator) instructions or login to LaunchPad and get started.
All you need is a web browser.

<!-- TODO: Update LaunchPad URLs to Future Production Studio project -->
* Application Translations: https://translations.launchpad.net/futureproductionstudio/2.0/+translations
* Website Translations: https://translations.launchpad.net/futureproductionstudio/website/+pots/django

## Dependencies

Although installers are much easier to use, if you must build from 
source, here are some tips: 

Future Production Studio is programmed in Python (version 3+), and thus does not need
to be compiled to run. However, be sure you have the following 
dependencies in order to run Future Production Studio successfully: 

*  Python 3.0+ (http://www.python.org)
*  PyQt5 (http://www.riverbankcomputing.co.uk/software/pyqt/download5)
*  libfps: Future Production Studio Library (https://github.com/FutureProductionStudio/libfps)
*  libfps-audio: Future Production Studio Audio Library (https://github.com/FutureProductionStudio/libfps-audio)
*  FFmpeg or Libav (http://www.ffmpeg.org/ or http://libav.org/)
*  GCC build tools (or MinGW on Windows)

## Launch

To run Future Production Studio from the command line with an installed `libfps`,
use the following syntax:
(be sure the change the path to match the install or repo location 
of fps-video)

```sh
cd [fps-video folder]
python3 src/launch.py
```
    
To run with a version of `libfps` built from source but not installed,
set `PYTHONPATH` to the location of the compiled Python bindings. e.g.:

```sh
cd [libfps folder]
cmake -B build -S . [options]
cmake --build build
    
cd [fps-video folder]
PYTHONPATH=[libfps folder]/build/bindings/python \
python3 src/launch.py
```

## Websites

- https://www.futureproduction.com/  (Official website and blog)
- https://github.com/FutureProductionStudio/fps-video (source code and issue tracker)
- https://github.com/FutureProductionStudio/libfps-audio (source code for audio library)
- https://github.com/FutureProductionStudio/libfps (source code for video library)
<!-- TODO: Update LaunchPad URL to Future Production Studio project when available -->
- https://launchpad.net/futureproductionstudio/

### Copyright & License

Copyright (c) 2008-2022 Future Production Studio. This file is part of
Future Production Studio Video Editor (https://www.futureproduction.com), an open-source project
dedicated to delivering high quality video editing and animation solutions
to the world.

Future Production Studio Video Editor is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

Future Production Studio Video Editor is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with Future Production Studio Library.  If not, see <http://www.gnu.org/licenses/>.
