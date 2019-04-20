---
layout: default
permalink: /engine
name: Engine
---

# Quiver Engine

The Quiver Engine is a modified version of the 2007 leak of Valve's Source Engine.
Among the improvements are upgraded shaders, better POSIX support (WIP), modernized
API, and better GUI via Ultralight (WIP).

## Building

It is not yet possible to build on OSX or Linux systems.

On windows, you will need Visual Studio with VC++ and [Perl](http://strawberryperl.com/)
installed. Then follow these steps to build Quiver:

- Open Perl Command Line and enter cpan String::CRC32
- Run createcoreprojects.bat and build the solution in Release.
- Run src/materialsystem/stdshaders/buildallshaders.bat.
- Run src/createallprojects.bat or src/createbinprojects.bat and build the solution in Release.
- Edit game/make_dir_junction.bat with your HL2 install directory if needed and Run

Then run the engine with run_mod_hl2.bat, run_mod_episodic.bat, or run_hl2r.bat.
