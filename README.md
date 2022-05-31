# Blowup: a script for making giant posters

`blowup.tex` is a small script for plain pdfTeX (*not* pdfLaTeX, which uses a
strict document structure) that blows up PDF, JPEG or PNG documents
pixel-perfectly across multiple pages, with a tunable overlap at the edges. PDF
documents even stay completely vectorized, retaining the tack-sharp fonts and
vector artwork. I wrote this script to create giant multiple-page posters of my
photos, which it does flawlessly.

If you stumbled on this page through Google and are not familiar with TeX, I
should explain that it's a free, open source, high quality, ultra-stable
typesetting engine used primarily by academia and book publishers. To use this
script, you first need to install a so-called TeX distribution.
[MikTeX](http://www.miktex.org) is a good one for Windows. Do yourself a
favour, learn how to write LaTeX (it's sort of like HTML) and never bother with
Microsoft Word again.

If you're looking for something quick and easy,
[pdfposter](http://pdfposter.origo.ethz.ch/) does something similar and does
not require TeX. There are tons of other alternatives too. This one is just my
donation.

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

There are no output size limits in this script; knock yourself out. Use this
script in whatever way you see fit. Maybe some day I'll write an online
interface, but if you need your posterized file *right now* (but uglier), I
suggest the [Rasterbator](http://homokaassu.org/rasterbator/).
