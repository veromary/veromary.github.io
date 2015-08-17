---
author: Veronica Brandt
comments: true
date: 2012-09-17
layout: post
slug: diy-handwriting-worksheets-with-latex
title: DIY handwriting worksheets with LaTeX
category: Education
tags: handwriting
---

There are several [handwriting fonts](http://www.tug.dk/FontCatalogue/calligraphicalfonts.html) already designed in METAFONT - the native font engine for TeX and family.  Most of these are German, one Austrian, one French - that's just the ones I know of.

[handwriting-samples]({{ site.url }}/pdf/handwriting-samples.pdf)

So there you have Lateinische Ausgangsschrift, French Cursive, Vereinfachten Ausgangsschrift, Österreichische Scholschrift and TW Cal 14.  Makes a change from all the US based handwriting worksheet generators which provide variations on Zaner-Bloser, D'Nealian and Getty Dubay.  It's still a far cry from the Australian Foundation Handwriting that I grew up with (italic, but taller ascenders and descenders than Getty).  

That's part of the fun of DIY homeschooling - so many options.

And how I made the sample sheet:

~~~latex
\documentclass{article}

\usepackage{la}
\usepackage{frcursive}
\usepackage[cm]{fullpage}
\usepackage{xcolor}
\usepackage{va}
\usepackage{oesch}
\usepackage{twcal14}

\begin{document}

\renewcommand{\seyesDefault}{\color{gray}}
\setlength{\parindent}{0mm}
%\setlength{\baselineskip}{12pt}
\setlength{\parskip}{10pt}

\huge

\lahuge

Lateinische Aushangsschrift:

\seyes{The quick brown fox jumps over the lazy dog \quad}

\seyes{\phantom{The quick brown fox jumps over the lazy dog \quad}}


\begin{cursive}
\acadshape

French Cursive

\seyes{The quick brown fox jumps over the lazy dog \quad}

\seyes{\phantom{The quick brown fox jumps over the lazy dog \quad}}

\end{cursive}

\vacalfont

Vereinfachten Ausgangsschrift

\seyes{The quick brown fox jumps over the lazy dog \quad}


\seyes{\phantom{The quick brown fox jumps over the lazy dog \quad}}

\oeschfamily

\"Osterreichische Scholschrift


\seyes{The quick brown fox jumps over the lazy dog \quad}

\seyes{\phantom{The quick brown fox jumps over the lazy dog \quad}}

TW Cal 14

\twcal

\seyes{The quick brown fox jumps over the lazy dog \quad}

\seyes{\phantom{The quick brown fox jumps over the lazy dog \quad}}

\end{document}
~~~

Theoretically it should work for any fonts - maybe next thing is to try using it with [Christopher Jarman](http://quilljar.users.btopenworld.com/) [Handwriting Fonts](http://quilljar.users.btopenworld.com/fonts.html) (make sure you download the PC truetype fonts - unless you have a RISC/Acorn computer and know what you're doing).

**Update**: [Briem Handwriting](http://briem.net) includes an italic font which has a lined variant.
