---
layout: page
order: 3
permalink: '/schedule/'
title: Schedule
...

## Aug. 27: Unix as a Way of Life

How to interact with your computer and to run programs through the
command-line interface. You will also learn a philosophy for writing
programs.

### Reading

-   Mike Gancarz, *[Linux and the Unix Philosophy][]*, chs. 1--8,
    focusing on the ten tenets.
-   William E. Shotts Jr., *[The Linux Command Line: A Complete
    Introduction][]*. Most of this book is a reference source, but
    familiarize yourself at a minimum with chapters 2 (navigation), 4
    (file manipulation), 5 (commands), 6 (redirection), 10 (processes),
    11 (environment). Nearly all of what Shotts writes about Linux will
    apply to the Unix terminal in Mac OS X.

### Exercises

Try out all the Unix style commands in your terminal.

Before class, do your best to get the following installed:

-   A text editor of your choice: [Sublime Text][], [TextWrangler][],
    [Atom][], and [Vim][] are all solid choices.
-   [Google Chrome][]
-   [VirtualBox][]
-   [Vagrant][]
-   [Homebrew][] (if you're on a Mac)
-   [Git][] (through Homebrew on a Mac; through the package manager on
    Linux)
-   [Node.js][] (through Homebrew on a Mac; through a package manager on
    Linux)
-   [R language][]
-   [R Studio Desktop][]

If you are on a Mac, you should install [Homebrew][] and any necessary
dependencies as you go along. If you are on some kind of Linux machine,
then probably everything you need is in your package manager. If you are
on a Windows PC, you should install [Ubuntu 14.04 LTS][] inside Virtual
Box using [Vagrant][]. Follow [this tutorial on Vagrant][], substituting
`ubuntu/trusty64` for `hashicorp/precise32`.

## Sept. 3: Version Control and Reproducible Research

Version control lets you contribute to projects and distribute your
code. [GNU Make][] helps automate and reproduce your results.

### Reading

-   Work through [GitHub's interactive tutorial][] for Git.
-   GitRef on [basics][] and [branching and merging][]; GitHub's
    tutorial on [pull requests][] ([video][]).
-   Look at Scott Chacon, *[Pro Git][]*, especially chs. 1--3, 5, for
    reference.
-   Read Karl Broman's [lectures about reproducible research][]:
    [introduction][]; [command line][]; [version control][].
-   Read Mike Bostock, "[Why Use Make][]".
-   Read the documentation for [GNU Make][].

### Exercises

-   At least one day before class, submit a pull request to the
    [repository for this syllabus][]. The pull request should modify the
    list of participants (`source/participants.md`) to add your name
    with a link to your personal website, as well as your GitHub user
    name and a link to your GitHub user profile. Feel free to include
    your Twitter user name and link if you like. (A guide to
    [Markdown][] if you need it.) Also add your name and the topic of
    your tutorial to the schedule (`source/schedule.md`).
-   Create a minimal Makefile. This Makefile should take a text file
    (provided by you) and find and replace words of your choosing to a
    new text file. (Hint:
    `sed 's/foo/bar/g' input-file.txt > output-file.txt` replaces all
    instances of `foo` with `bar` and redirects standard out to a file.)
    The Makefile should also put the time stamp for when the output file
    was generated at the bottom of the file. (Hint: in your shell the
    `>>` operator appends to a file; there is also a command to get the
    current time.) Can you rewrite the Makefile so that it uses rules?
    So that it uses special targets? So that it works on several text
    files at once? On an arbitrary number of files? So that it uses a
    default rule? Post your Makefile and input text files to GitHub.

## Sept. 10: Flow Control and Functions in JavaScript

The basics of JavaScript, as well as some foundational principles like
loops, conditionals, functions, closure, and recursion.

### Reading

-   Read Marijn Haverbeke, *[Eloquent JavaScript: A Modern Introduction
    to Programming][]* (hereafter EJ), [introduction][1], [ch. 1][],
    [ch. 2][], [ch. 3][].
-   Browse the [JavaScript documentation][], paying special attention to
    [strings][]. ([DevDocs][] is also useful for language and API
    documentation.)

### Exercises

-   Create separate `.js` files with the solutions for each exercise in
    these chapters, and post them to GitHub.

## Sept. 17: Data Structures in JavaScript

An introduction to how data is structured, and an introduction to the
object-oriented style of programming for modeling data.

### Reading

-   Read EJ, [ch. 4][], [ch. 6][].
-   Browse the [documentation for the DPLA's API][] and sign up for [an
    API key][].
-   Browse the [API for the American Converts Database][], especially
    the [items page][], as well as the [Omeka REST API documentation][].

### Exercises

-   Create separate `.js` files with the solutions for each exercise in
    these chapters, and post them to GitHub.
-   Think of a historical source, event, or life that could be modeled
    as data, and create a data model for it in JavaScript. Can you write
    a constructor function to create new objects? Can you create at
    least five objects? How can you store an arbitrary number of
    objects? Now that you've stored those objects, what can you do with
    them that is interesting? How can you display, represent, filter,
    and link them? Post your code to GitHub.

## Sept. 24: Functional Programming in JavaScript; DOM Manipulation

An introduction to manipulating data with pure functions, and to
creating elements on a web page.

### Reading

-   Read EJ, [ch. 5][], [ch. 12][], Skim [ch. 13][], but we have much
    better ways for manipulating the DOM in D3.js.
-   Read Scott Murray, *[Interactive Data Visualization for the Web][]*
    (O'Reilly, 2013), [ch. 4][2], [ch. 5][3].
-   If it's helpful, read Mike Bostock, "[Thinking with Joins][]."

### Exercises

-   Create separate `.js` files with the solutions for each exercise in
    chapter 5 only.
-   Last week we looked at historical data available through APIs.
    Rewrite our code using functional programming. How can you do this
    with functions that you write yourself? How can D3's functions for
    manipulating data help you? How can you use D3's functions for
    manipulating the DOM to display the data? Can you build in
    interactivity? What can you make that is usefuL? Post your code to
    GitHub (if suitable, as a [bl.ocks][] too).

## Oct. 1: Introduction to R / Grammar of Graphics in R

We learn our second programming language and begin to make real
visualizations.

### Reading

-   Watch the [Google Developers' introduction to R][]. You might also
    like [R Twotorials][].
-   For a more thorough introduction to R, read the opening chapters of
    Norman Matloff, *The Art of R Programming: A Tour of Statistical
    Software Design* (No Starch Press, 2011) or of Hadley Wickham,
    *[Advanced R][]*.
-   Read Hadley Wickham, *ggplot2: Elegant Graphics for Data Analysis*,
    chs. 1--5. For the theory behind ggplot, look at Leland Wilkinson,
    *The Grammar of Graphics*, 2nd ed. (Springer, 2005). You may find
    Winston Chang, *[R Graphics Cookbook][]*, appendix A, chs. 1--4, a
    useful introduction to ggplot.
-   Browse the [ggplot2 documentation][].

### Exercises

-   Experiment with ggplot2 in R Studio as you read the assigned books.
-   Find a historical data set and make as many different kinds of
    charts with it as you can. (Some of them should be bad charts or
    unhelpful charts.) Annotate the charts in RMarkdown and Knitr
    ([guide here][]). Post the code to GitHub and the document to
    [RPubs][].

## Oct. 8: Manipulating Data in R

Data seldom comes in the format we need it: this is how to munge it into
a useful form.

### Reading

-   Watch Hadley Wickham, "[Tidy Data and Tidy Tools][]," NYC Open
    Statistical Computing Meetup, Dec. 2011.
-   Read Hadley Wickham, "[Tidy Data][]," *Journal of Statistical
    Software* (forthcoming).
-   Read Hadley Wickham, "[Reshaping Data in R][]," *Statistical
    Computing and Graphics* 16, no. 2 (Dec. 2005): 5--8.
-   Read Hadley Wickham, "[The Split-Combine-Apply Strategy for Data
    Analysis][]," *Journal of Statistical Software* 40, no. 1 (Apr.
    2011): 1--29.
-   Browse documentation for [tidyr][] and [dplyr][]. Be aware of the
    more full-featured packages [reshape2][] and [plyr][].
-   You may find Seth van Hooland, Ruben Verborgh, and Max De Wilde,
    "[Cleaning Data with OpenRefine][]," to be helpful.

### Exercises

You will be provided with a messy, untidy data set. Without editing any
file by hand, create a pipeline that cleans and tidies the data. Create
some sample data visualizations to demonstrate that the data has been
tidied. Can you also apply this technique to some data you have gathered
for your research? Publish your input, output, and code files on GitHub
and your explanation of the process as an Rpubs document.

## Oct. 15: Sp in R

How to make maps and perform other kinds of spatial analysis.

### Reading

-   Read Roger S. Bivand, Edzer Pebesma, and Virgilio Gómez-Rubio,
    *Applied Spatial Data Analysis with R* (Springer, 2013).

-   Read Robin Lovelace and James Cheshire, "[Introduction to Spatial
    Data and ggplot2][]," Spatial.ly, Dec. 9, 2013.

-   Read Steven Brey, "[Working with Geospatial Data][]" and Bethany
    Yollin, "[Working with Geospatial Data (and ggplot2)][]."

-   Browse documentation for [sp][], [rgdal][], [rgeos][], [geonames][],
    and [ggmap][] R packages, as well as for the [GDAL/OGR][]
    command-line tools.

### Exercises

Select from the spatial data sets available to you, or find your own.
Make maps. Publish your code to GitHub and your results to Rpubs. Hint:
If you use ggplot2 with a projected shapefile (i.e., a shapefile whose
coordinates are stored in some coordinate reference system other than
latitude and longitude) it will probably blow up. First convert the
shapefile to [EPSG 4326/WGS 84][].

## Oct. 22: Text Mining in R

How to do "distant reading," document similarity, and other kinds of
textual analysis.

### Reading

-   Read Matthew Jockers, *Text Analysis with R for Students of
    Literature* (Springer, 2014). You may also wish to consult Matthew
    Jockers, *[Macroanalysis][]* (University of Illinois Press, 2013).
-   Read Fred Gibbs, "[Document Similarity with R][],"
-   Read the text mining and topic modeling sections sections of Shawn
    Graham, Ian Milligan, and Scott Weingart, *[The Historian's
    Macroscope][]*.
-   Read the [topic-modeling issue][] of the *Journal of Digital
    Humanities* 2, no. 1 (2012).
-   Browse the documentation for [MALLET][] and the [mallet][MALLET] and
    [tm][] R package.

### Exercises

Chose one (or both) of the following, in either case posting your code
to GitHub and your results to RPubs:

-   In the nineteenth-century United States, there was a fierce debate
    over whether to codify laws. New York created several codes of civil
    procedure, which other states then borrowed. You will be given a
    handful of codes. Which codes borrowed from one another? What did
    they borrow? How can you visualize this? How can you browse the
    borrowings? What interpretations do you draw from this?
-   You will be given a cleaned up set of texts from the Oxford
    Movement's *Tracts for the Times*. What does text mining and topic
    modeling these texts tell you? You may substitute another corpus if
    you wish.

## Oct. 29: Network Analysis in R

How to measure and visualize networks of people, events, ideas, sources,
you name it.

### Reading

-   Read Eric D. Kolaczyk and Gábor Csárdi, *Statistical Analysis of
    Network Data with R* (Springer, 2014).
-   Read the networks sections of Shawn Graham, Ian Milligan, and Scott
    Weingart, *[The Historian's Macroscope][]*.
-   Read Elijah Meeks, "[More Networks in the Humanities][]."
-   Read Scott Weingart, "[Demystifying Networks, Parts I & II][],"
    *Journal of Digital Humanities* 1, no. 1 (2011).
-   Browse the documentation for the [statnet][], [sna][], and
    [network][] R packages.

### Exercises

You will be provided with some historical data suitable for network
analysis, or you may bring your own. Do some network analysis with
visualizations and interpretations.

## Nov. 5: D3.js Concepts

The basics of a powerful visualization library for the web.

### Reading

-   Read Scott Murray, *[Interactive Data Visualization for the Web][3]*
    (O'Reilly, 2013).
-   Read Mike Bostock, "[Let's Make a Bar Chart][]" parts 1--3, "[Let's
    Make a Map][]," "[Let's Make a Bubble Map][]," and "[Thinking with
    Joins][]."
-   Browse the [D3 documentation][].
-   Experiment with the examples in the [D3 gallery][].

### Exercises

-   Using some suitable data set(s), create as many different kinds of
    D3 visualizations as you can manage. (These need not be complicated
    visualizations.) Can you add interactivity to them? What does
    interactivity add to the graphics? What does it take away?

## Nov. 12: D3.js Applications

From D3 basics to D3 for history.

### Exercises

Over the course of the semester we have written programs to do many
kinds of analysis. Take one of the kinds of analysis that seems most
promising for your work, and translate it to the web using D3. Create
the most sophisticated (not flashy) visualization that you can, and
embed it in an interpretation or narrative. Use the principles of
reproducible research as appropriate.

## Nov. 19: Workshop day / TBD

This week we will work collaboratively on the projects for the course.
We may also cover additional topics such as web applications and
frameworks ([Ruby on Rails][], [Sinatra][], [Node.js][]); programming
practices such as debugging, refactoring, and testing; other programming
languages ([Python][], [Ruby][], [PHP][]); basic statistics of use to
historians; or other topics relevant to your research.

## Nov. 26: No class

Thanksgiving break.

## Dec. 3: Project Presentations

You will present your final projects, with an emphasis on both their
code and historical interpretations. **Final projects are due by 6 p.m.
on December 10.**

  [Linux and the Unix Philosophy]: http://magik.gmu.edu/cgi-bin/Pwebrecon.cgi?BBID=3366870
  [The Linux Command Line: A Complete Introduction]: http://linuxcommand.org/tlcl.php
  [Sublime Text]: http://www.sublimetext.com/
  [TextWrangler]: http://www.barebones.com/products/textwrangler/
  [Atom]: https://atom.io/
  [Vim]: http://www.vim.org/
  [Google Chrome]: https://www.google.com/intl/en-US/chrome/browser/
  [VirtualBox]: https://www.virtualbox.org/
  [Vagrant]: http://www.vagrantup.com/
  [Homebrew]: http://brew.sh/
  [Git]: http://git-scm.com/
  [Node.js]: http://nodejs.org/
  [R language]: http://www.r-project.org/
  [R Studio Desktop]: http://www.rstudio.com/products/rstudio/
  [Ubuntu 14.04 LTS]: http://www.ubuntu.com/download/desktop
  [this tutorial on Vagrant]: https://docs.vagrantup.com/v2/getting-started/index.html
  [GNU Make]: http://www.gnu.org/software/make/
  [GitHub's interactive tutorial]: http://try.github.io/
  [basics]: http://gitref.org/basic/
  [branching and merging]: http://gitref.org/branching/
  [pull requests]: https://help.github.com/articles/using-pull-requests
  [video]: http://vimeo.com/41045197
  [Pro Git]: http://git-scm.com/book
  [lectures about reproducible research]: http://kbroman.org/Tools4RR/pages/schedule.html
  [introduction]: http://kbroman.org/Tools4RR/assets/lectures/01_intro_withnotes.pdf
  [command line]: http://kbroman.org/Tools4RR/assets/lectures/02_unix_withnotes.pdf
  [version control]: http://kbroman.org/Tools4RR/assets/lectures/04_git_withnotes.pdf
  [Why Use Make]: http://bost.ocks.org/mike/make/
  [repository for this syllabus]: https://github.com/lmullen/clio3-syllabus
  [Markdown]: https://help.github.com/articles/markdown-basics
  [Eloquent JavaScript: A Modern Introduction to Programming]: http://eloquentjavascript.net/
  [1]: http://eloquentjavascript.net/00_intro.html
  [ch. 1]: http://eloquentjavascript.net/01_values.html
  [ch. 2]: http://eloquentjavascript.net/02_program_structure.html
  [ch. 3]: http://eloquentjavascript.net/03_functions.html
  [JavaScript documentation]: http://www.w3schools.com/jsref/
  [strings]: http://www.w3schools.com/jsref/jsref_obj_string.asp
  [DevDocs]: http://devdocs.io/
  [ch. 4]: http://eloquentjavascript.net/04_data.html
  [ch. 6]: http://eloquentjavascript.net/06_object.html
  [documentation for the DPLA's API]: http://dp.la/info/developers/codex/
  [an API key]: http://dp.la/info/developers/codex/policies/#get-a-key
  [API for the American Converts Database]: http://americanconverts.org/api
  [items page]: http://americanconverts.org/api/items?pretty_print
  [Omeka REST API documentation]: http://omeka.readthedocs.org/en/latest/Reference/api/
  [ch. 5]: http://eloquentjavascript.net/05_higher_order.html
  [ch. 12]: http://eloquentjavascript.net/12_browser.html
  [ch. 13]: http://eloquentjavascript.net/13_dom.html
  [Interactive Data Visualization for the Web]: http://chimera.labs.oreilly.com/books/1230000000345
  [2]: http://chimera.labs.oreilly.com/books/1230000000345/ch04.html
  [3]: http://chimera.labs.oreilly.com/books/1230000000345/ch05.html
  [Thinking with Joins]: http://bost.ocks.org/mike/join/
  [bl.ocks]: http://bl.ocks.org/
  [Google Developers' introduction to R]: https://www.youtube.com/playlist?list=PLOU2XLYxmsIK9qQfztXeybpHvru-TrqAP
  [R Twotorials]: http://www.twotorials.com/
  [Advanced R]: http://adv-r.had.co.nz/
  [R Graphics Cookbook]: http://www.cookbook-r.com/Graphs/
  [ggplot2 documentation]: http://docs.ggplot2.org/current/
  [guide here]: http://rmarkdown.rstudio.com/
  [RPubs]: http://rpubs.com/
  [Tidy Data and Tidy Tools]: http://vimeo.com/33727555
  [Tidy Data]: http://vita.had.co.nz/papers/tidy-data.pdf
  [Reshaping Data in R]: http://vita.had.co.nz/papers/reshape-scgn.html
  [The Split-Combine-Apply Strategy for Data Analysis]: http://www.jstatsoft.org/v40/i01/
  [tidyr]: http://cran.r-project.org/web/packages/tidyr/index.html
  [dplyr]: http://cran.r-project.org/web/packages/dplyr/index.html
  [reshape2]: http://cran.r-project.org/web/packages/reshape2/index.html
  [plyr]: http://cran.r-project.org/web/packages/plyr/index.html
  [Cleaning Data with OpenRefine]: http://programminghistorian.org/lessons/cleaning-data-with-openrefine
  [Introduction to Spatial Data and ggplot2]: http://spatial.ly/2013/12/introduction-spatial-data-ggplot2/
  [Working with Geospatial Data]: http://mazamascience.com/WorkingWithData/?p=1277
  [Working with Geospatial Data (and ggplot2)]: http://mazamascience.com/WorkingWithData/?p=1494
  [sp]: http://cran.r-project.org/web/packages/sp/index.html
  [rgdal]: http://cran.r-project.org/web/packages/rgdal/index.html
  [rgeos]: http://cran.r-project.org/web/packages/rgeos/index.html
  [geonames]: http://cran.r-project.org/web/packages/geonames/
  [ggmap]: http://cran.r-project.org/web/packages/ggmap/index.html
  [GDAL/OGR]: http://www.gdal.org/
  [EPSG 4326/WGS 84]: http://spatialreference.org/ref/epsg/wgs-84/
  [Macroanalysis]: http://magik.gmu.edu/cgi-bin/Pwebrecon.cgi?BBID=3547073
  [Document Similarity with R]: http://fredgibbs.net/tutorials/tutorial/document-similarity-with-r/
  [The Historian's Macroscope]: http://www.themacroscope.org/
  [topic-modeling issue]: http://journalofdigitalhumanities.org/2-1/
  [MALLET]: http://cran.r-project.org/web/packages/mallet/index.html
  [tm]: http://cran.r-project.org/web/packages/tm/index.html
  [More Networks in the Humanities]: https://dhs.stanford.edu/visualization/more-networks/
  [Demystifying Networks, Parts I & II]: http://journalofdigitalhumanities.org/1-1/demystifying-networks-by-scott-weingart/
  [statnet]: http://cran.r-project.org/web/packages/statnet/index.html
  [sna]: http://cran.r-project.org/web/packages/sna/index.html
  [network]: http://cran.r-project.org/web/packages/network/index.html
  [Let's Make a Bar Chart]: http://bost.ocks.org/mike/bar/
  [Let's Make a Map]: http://bost.ocks.org/mike/map/
  [Let's Make a Bubble Map]: http://bost.ocks.org/mike/bubble-map/
  [D3 documentation]: https://github.com/mbostock/d3/wiki
  [D3 gallery]: https://github.com/mbostock/d3/wiki/Gallery
  [Ruby on Rails]: http://rubyonrails.org/
  [Sinatra]: http://www.sinatrarb.com/
  [Python]: https://www.python.org/
  [Ruby]: https://www.ruby-lang.org/en/
  [PHP]: http://php.net/
