Template for esp8266 projects
=============================

Contents of the template
------------------------
  * README.md  - This should decribe the project. It should include:
    * A project summary, what it does and how it works.
    * Build and installation instructions
    * Copyright and license

    Keep this file short and clear. If it gets too long, move
    sections into other files and just refer to them from here.

  * Makefile - For simple, single file projects you don't need to
      modify this file. Just put your code in the `user/app.c`.

  * .gitignore - This is a list of files that should not be committed.

  * paths.tmpl - Environment variables that point the build tools.

      __DO NOT MODIFY paths.tmpl__ Copy it to `paths.inc` and make your
      changes there. `paths.inc` is listed in `.gitignore` so that it
      will not get committed. This both protects you from inadvertentely
      sharing information about your environment when you share your git
      archive and prevents _dualing commits_.

  * user/ - The top level code for your app goes here.

  * driver/ - auxillary code used by your app

  * include/ - header files

Instructions
------------
  * Clone this template to start a project
  * Delete the top port of this README.md file
  * Update this and the other README.md files, particularly the copyright
  * notices. 
  * Start writing code


Project README Template
=======================

Copyright 2015 Jerry Dunmire
This file is part of appTemplate

appTemplate is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or
(at your option) any later version.

appTemplate is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with appTemplate.  If not, see <http://www.gnu.org/licenses/>.

Files that are not part of appTemplate are clearly identified at the top
of each of the files. These files are distributed under terms noted in each
of the files.


Build and Installation
----------------------
  * Copy `paths.tmpl` to `paths.inv`.
  * Adjust the paths in `paths.inv` for your setup.
  * Build:

        $ make

  * Install (put your target system in bootloader mode first):

        $ make flash

