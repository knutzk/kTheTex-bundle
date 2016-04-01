# kTheTex-bundle

This bundle will include both templates for reports and theses written
in LaTeX. The intention is to provide a comprehensive and
out-of-the-box template that is easy to use. Most of the templates out
there focus take convenience and technical aspects over an elaborate
design, this template will try to include everything.

Please feel free to suggest anything you would consider to be useful
for a thesis template as well. Or even start contributing yourself.


## Is there a stable release?

Right now, there is no stable release of this package. There are still
some points to be crossed from the to do list, before the first
official (or even preliminary) release can be published. If you are
still interested to try the current code, simply download it! The
bundle is based on the docstrip utility, combing both documentation
and code in the same files. The class and package files can be
generated with the included script `kTheTex-bundle.ins` by calling

```
$ latex kTheThex-bundle.ins
```

The writing of a documentation is still in progress, but it can be
generated via

```
$ latex kTheTex-bundle.dtx
```


## But how do those templates look like?

Although still on a very early stage, there is a showcase file for the
class `ktxreprt` that has already been created. A compiled version can
be created by calling

```
$ pdflatex showcase-report.tex
$ biber showcase-report
$ pdflatex showcase-report.tex
```

The program `biber` is needed since the generation of the bibliography
is done with the package Biblatex instead of the old BibTeX. Biblatex
and `biber` are part of every major TeX distribution and are available
as stable releases 2.0 and 1.0 since summer 2012, respectively. If you
haven't switched to Biblatex in your projects, you should consider it!
The main reason for this package to use Biblatex is the fact that its
style files are written in LaTeX code and are therefore much easier
to read, to understand and to adjust than files based on BibTeX code.


## To Do List

1. Write a more appropriate README that actually includes more useful
information about the contents of this bundle.
2. Remove the to do list from the showcase, this should be part of the
documentation instead
3. Write another showcase for a thesis.
4. Inclusion of various packages to the whole bundle, saved in aux/
right now. Those include
  * `kPrakt.sty`
  * `kBibstyle.sty`
  * `kLinenumbers.sty`
5. Support for different types of classes, such as report and
thesis. This should also be extended to *minimal* versions of those,
without the whole bunch of options the classes usually contain.
6. Inclusion of Uni Goettingen specific parts, such as the thesis
cover and the declaration in the end.
