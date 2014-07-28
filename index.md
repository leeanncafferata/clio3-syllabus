---
layout: page
title: About 
order: 1
...

## Course description

This class will teach you how to use computer programming for research
in history. This class is not organized around the features of a
particular programming language or the theoretical concepts of
programming, as a class in a computer science department might be.
Rather it is organized around three of the common practices (and four of
the common programming languages) that digital historians use to do
their work.

We will begin by learning the principles of the Unix operating system
which undergirds almost all research programming. Our first major
section will be on data analysis, in which you will use the R
language to analyze historical data both quantitatively and
geographically. You will also learn how researchers structure,
manipulate, and clean their data. At the end of this section you will
translate one of your visualizations into an interactive, online version
using Javascript, the lingua franca for interacting with users over
the web. Our next major section will be on scripting for research,
using the elegant and expressive language Ruby. We will begin by
using Ruby to access APIs and scrape web documents for research. Then we
will use Ruby to create our own simple web applications and to
interact with relational databases. Finally we will move on from Ruby to
PHP, a commonly used language for web applications like Omeka and
WordPress. We will use Omeka as our example of a large-scale digital
humanities tool. You will learn how Omeka plugins work and make your own
plugin as your final project.

This course emphasizes breadth for three reasons. First, digital
humanists tend to be polyglot when it comes to tools and programming
languages. Second, often the best way to gain a deeper understanding of
one language is to learn a second language. By comparing multiple
languages you will gain a knowledge of the basic structures of computer
programming. Third, picking up several languages will teach you how to
learn a computer language. In my experience, once you've learned three
or four programming languages it becomes much easier to pick up the next
language.

Since this is a research class, students are expected to come to the
course with an active research agenda and to know of or soon find a body
of primary sources susceptible to computational methods. As much as
possible, you should try to use the assignments in this course to
advance your research, especially for your dissertation. You should
expect to come out of this course a better-equipped historian. While
this course alone will likely not be sufficient to turn you into a
digital humanities software developer (for that you'll need a deep
immersion in a particular language or two) you will gain a familiarity
with the basics of computer programming as applied for humanities
research. Using this base, you can go on to become more fluent as a
digital humanities developer should you wish.

This course does not presume any prior experience with computer
programming. However the course does assume that you have taken Clio 1
and Clio 2, and thus possess the skills taught in those courses. Make no
mistake, this is an advanced digital history course and you will likely
find the material very difficult, even alien at first. Nevertheless, I
will make the commitment to get or give you all the help that you need,
and (contrary to a common discourse about computer programming) there is
no intrinsic reason why you should not do well in this course.

## Learning goals

After taking this course, you will

-   be familiar with R, Javascript, Ruby, and PHP, along with some of
    their most useful libraries, such as ggplot2, dplyr, jQuery, D3,
    Sinatra, and Nokogiri;
-   understand the common concepts of computer programming across
    computer languages;
-   be able to read documentation and navigate online aids such as Stack
    Overflow in order to learn programming languages for yourself;
-   perform reproducible data analysis both quantitatively and
    geographically;
-   programmatically access APIs and data for your research;
-   understand the basics of how web applications are built; and
-   contribute code back to digital humanities projects.

## A few notes

This course assumes that you are programming in a Unix-like environment,
namely some Linux distribution or the Unix underpinnings of Mac OS X.
You're free to use Windows if you like, but I won't support you in
figuring out the differences, and your code will have to run on my
machine.

Configuration is the bane of all computer projects, and to that end all
code must run on a standard machine. This machine image will be
available to you using [Vagrant][], and you'll be able to run it as a
virtual machine on your own computer. You should test all code in the
virtual machine before submitting it.

To submit your code, you will need a [GitHub][] account, and must let me
know your user name. (Your account can be anonymous/pseudonymous to the
world, if you wish, just not to the people in this course.) Each
assignment for the course should have its own repository, and each
repository should have a tag, `submitted`, for the version of the
assignment you wish me to grade.

This course will not teach you the tips and tricks of the innumerable
tools that surround programming, such as IDEs (Integrated Development
Environments), text editors, syntax checkers, environment managers and
so on, though I can provide suggestions if you need them. Use whatever
you want. If you don't have a preferred text editor, you could do worse
than [Sublime Text][] or [TextWrangler][]. I prefer [Vim][].

The culture around programming can be extraordinarily generous, with
many people sharing their work and expertise for free. It can also be
extraordinarily toxic, especially for women and minorities. Part of this
course will be learning to help yourself in the culture of programming,
including indispensable sites such as [Stack Overflow][]. If you get
stuck in the more nefarious parts of the culture, come ask for help.

In any case, come talk with me early and often!

  [The Programming Historian 2]: http://programminghistorian.org/
  [Vagrant]: http://www.vagrantup.com/
  [GitHub]: https://github.com/
  [Sublime Text]: http://www.sublimetext.com/
  [TextWrangler]: http://www.barebones.com/products/textwrangler/
  [Vim]: http://www.vim.org/
  [Stack Overflow]: http://stackoverflow.com/
