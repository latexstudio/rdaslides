The rdaslides class: Research Data Alliance presentations
=========================================================

The rdaslides LaTeX class is intended to produce slides for Research
Data Alliance (RDA) presentations, or an accompanying transcript, or
both.

Installation
------------

### Automated way ###

A makefile is provided which you can use with the Make utility:

  * Running `make` generates the derived files

      - README.md
      - rdaslides.pdf
      - rdaslides-slides.pdf
      - rdaslides.cls
      - rdamsdwg.sty

  * Running `make inst` installs the files (and images) in the user's
    TeX tree.
  * Running `make install` installs the files (and images) in the
    local TeX tree.

### Manual way ###

 1. Compile rdaslides.dtx just as you would a normal LaTeX file. As well
    as the usual PDF (or DVI) and auxiliary files, several others are
    generated.

 2. Compile rdaslides.dtx a second time with `-jobname=rdaslides-slides`
    as a command line option to generate the sample slides.

 3. Move the files to your TeX tree as follows:

      - `source/latex/rdaslides`: rdaslides.dtx, rdaslides.ins
      - `tex/latex/rdaslides`: rdaslides.cls, rdamsdwg.sty,
         rda-bg-normal.jpeg rda-bg-title1.jpeg rda-bg-title2.jpeg
      - `doc/latex/rdaslides`: rdaslides.pdf, rdaslides-slides.pdf,
         README.md

 4. You may then have to update your installation's file name database
    before TeX and friends can see the files.

Licence
-------

Copyright 2015 Alex Ball.

This work consists of three image files (rda-bg-normal.jpeg,
rda-bg-title1.jpeg, and rda-bg-title2.jpeg), the documented LaTeX file
rdaslides.dtx, and a Makefile.

The text files contained in this work may be distributed and/or modified
under the conditions of the [LaTeX Project Public License (LPPL)][lppl],
either version 1.3c of this license or (at your option) any later
version.

The rights to the image files distributed with this bundle are held by
the [Research Data Alliance][rda].

This work is "maintained" (as per LPPL maintenance status) by [Alex
Ball][me].

[lppl]: http://www.latex-project.org/lppl.txt
[rda]: https://rd-alliance.org/
[me]: http://alexball.me.uk/

