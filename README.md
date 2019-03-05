# ne-visit-packet

This repository contains the LaTeX source files for the UC Berkeley Department of Nuclear Engineering prospective graduate student visit packet.
The packet is a document assembled by current UC Berkeley NE graduate students to represent the individuals who make up the department.
The packet features short bios of students, activities and extracurriculars, and ends with photos of Berkeley students living life to the fullest.

<div align='center'>
<img src='fig/ne_logo.png' width='25%'>
</div>

## Editing & Updating

To edit this packet for future years, feel free to clone this repository and edit any of the files as needed.
The repository is also linked to Overleaf, so you should be able to get access there. Contact me (@mitchnegus) for more info. 

The files are designed to be fairly easy to work with, so that you (hopefully) shouldn't need a ton of TeX expertise to update them.
Whenever possible, I've added `\newcommand` options so that template entries can be adjusted as students graduate or Professors are hired/retire.
As an example, for the faculty and student tiles, a user just needs to specify fields in the corresponding `\facultytile`/`\studenttile` commands.
More details can be found at the tops of those respective files (`faculty.tex` and `research_groups.tex`).
Still, despite my best attempts, configuring image locations is still a bit tricky. 
Finagling those to show up well may require a bit of effort, especially for images of different sizes.
My suggestion is that you get familiar with the `minipage` and `wrapfigure` environments, and then you can play around with getting the dimensions and spacing just right. 

One last note: the document uses a non-standard LaTeX font, and so it must be compiled using LuaLaTeX, not the standard pdflatex compiler. 

Good luck and go bears!
