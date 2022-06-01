# Blowup: a script for making giant posters

`blowup.tex` is a small script for plain pdfTeX (*not* pdfLaTeX, which uses a
strict document structure) that blows up PDF, JPEG or PNG documents
pixel-perfectly across multiple pages, with a tunable overlap at the edges. PDF
documents even stay completely vectorized, retaining the tack-sharp fonts and
vector artwork. I wrote this script to create giant multiple-page posters of my
photos.

If you stumbled on this page through Google and are not familiar with TeX, I
should explain that it's a free, open source, high quality, ultra-stable
typesetting engine used primarily by academia and book publishers. To use this
script, you first need to install a so-called TeX distribution.
[MikTeX](http://www.miktex.org) is a good one for Windows. Do yourself a
favour, learn how to write LaTeX (it's sort of like HTML) and never bother with
Microsoft Word again.

![Original image and blown up version](blowup.svg "Original and blowup")

Above: the original image and the sliced-and-diced version.

## Usage

Download the script. Put the name of your file in the script where it says
`YOUR-FILE-HERE.png`. Choose how many pages wide you want your blowup to be.
(Height is calculated automatically.) In Linux, type `pdftex blowup.tex` to
generate a file named `blowup.pdf` in the current directory. In Windows, put
this script and your input file in the directory where pdftex.exe is located,
then open a command window, go to the directory, and type `pdftex blowup.tex`.
You'll find that a file called `blowup.pdf` has been created, which is your
poster.

# License

This repo is licensed under the [MIT License](https://opensource.org/licenses/MIT).
