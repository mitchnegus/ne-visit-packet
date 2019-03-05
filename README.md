# UC Berkeley Nuclear Engineering Visit Packet

This repository contains the LaTeX source files for the UC Berkeley Department of Nuclear Engineering prospective graduate student visit packet.
The packet is a document assembled by current UC Berkeley NE graduate students to represent the individuals who make up the department.
The packet features short bios of students, activities and extracurriculars, and ends with photos of Berkeley students living life to the fullest.

<div align='center'>
<img src='fig/ne_logo.png' width='25%'>
</div>

## Editing & Updating

To edit this packet for future years, feel free to clone this repository and edit any of the files as needed.
The repository is also linked to Overleaf, so you should be able to get access there. Contact me (@mitchnegus) for more info. 


#### Structure

The packet is based in the `visit-packet.tex` file, which is what you should compile. 
This will generate the `visit-packet.pdf` file for distribution. 
The `visit-packet.tex` file will pull all preamble information from the `preamble.tex` file, before processing all of the individual body elements. 

These body elements are (in order):

* `cover_page.tex`: The cover page with dates and logo
* `contents.tex`: The table of contents page, with a welcome letter from UCB NE graduate students
* `cal.tex`: A page describing UC Berkeley
* `ne_department.tex`: A page describing the UCB NE department
* `faculty.tex`: A section with photos and research descriptions of the department's faculty
* `research_groups.tex`: A section with descriptions of the research groups, along with bios of (some of) the groups research members
* `nssc.tex`: A page on the Nuclear Science and Security Consortium
* `activities.tex`: A section on extracurricular activities of Berkeley students
* `berkeley_life.tex`: A section with photos of UC Berkeley students in action

All figures used in the document should be stored in the `fig` directory.


#### Templates

The files are designed to be fairly easy to work with, so that you (hopefully) shouldn't need a ton of TeX expertise to update them.
Whenever possible, I've added `\newcommand` templates so that things can be adjusted easily as students graduate and professors are hired/retire—no need to dig around too much in the LaTeX code.
As an example, for the faculty and student tiles, a user just needs to specify fields in the corresponding `\facultytile`/`\studenttile` commands.
More details can be found at the tops of those respective files (`faculty.tex` and `research_groups.tex`).
Still, despite my best attempts, configuring image locations is still a bit tricky. 
Finagling those to show up well may require a bit of effort, especially for images of different sizes.
My suggestion is that you get familiar with the `minipage` and `wrapfigure` environments, and then you can play around with getting the dimensions and spacing just right. 

One last note: the document uses a non-standard LaTeX font (OpenSans, described in the file `OpenSans-Regular.ttf`), and so it must be compiled using LuaLaTeX, not the standard pdflatex compiler. 

Good luck and go bears!
