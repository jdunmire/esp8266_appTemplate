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

      __DO NOT MODIFY THIS FILE__ Copy it to `paths.env` and make your
      changes there. `paths.env` is listed in `.gitignore` so that it
      will not get committed. This both protects you from
      inadvertentely sharing information about your environment when
      you share your git archive and prevents _dualing commits_.

  * user/ - The top level code for your app goes here.

  * driver/ - auxillary code used by your app

  * include/ - header files

Instructions
------------
  * Clone this template to start a project
  * Update the README.md files
  * Start writing code


Project README Template
=======================
This template project prints "Hello, World".


Build and Installation
----------------------
  * Copy `paths.tmpl` to `paths.inv`.
  * Adjust the paths in `paths.inv` for your setup.
  * Build:

        $ make

  * Install (put your target system in bootloader mode first):

        $ make flash


Copyright and License
---------------------
