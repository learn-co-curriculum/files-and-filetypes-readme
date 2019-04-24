# Files, Extensions, and File Types

## Problem Statement

Have you tried to memorize a phone number "for a second" as you tried to write
it down? Maybe you kept repeating it over and over?  Have you ever felt a little
overwhelmed when someone was giving you too much information at once and you were
trying to keep up--but felt relief when you finally "got it"? As humans we can
only hold a few things in our heads before they start to, well, vanish or get 
mixed up. Our _working memory_ is not too reliable!

Computers also have a limited working memory. Just like us, they keep things in
working memory that they're, well, working with.

When computers or people run out of space, they write down information stored
in their _working memory_. Humans sometimes use a napkin, Post-It Notes or the back of their
hands. Computers use _files_.  The stuff computers write into their files fits
into two main categories:

1.  information humans can read ("text files")
2.  information only computers can read ("binary files")

Developers create _lots_ of files. This README will help us all get on the same
page with how to talk about them.

## Objectives

1. Define what a file is
2. Contrast _text files_ versus _binary files_
3. Identify the function of file extensions

## Define What a File Is

A file is a thing computers use to store facts ("data") or processes
("programs") for later use.

## Contrast _Text Files_ Versus _Binary Files_

Computers think in electricity.

Whoa!

Computers' thoughts are usually shown as 1's and 0's. This is called _binary
code_.  When computers write things down, they often write them down in files in
_their_ language, _binary_.  These files are _binary files_.

Types of _binary_ files are images, music, and software programs. We can create
these files with Adobe Photoshop, the C programming language, or Ableton.

Nobody is exactly sure how humans think. That's a question for science or
philosophy. When we write our ideas down, we write them in files in _our_
language, _text_. These files are _text files_.

Types of _text_ files are HTML, letters to grandma, a list of student
grades for a gradebook program, directions to Carnegie Hall, etc.  We create
these _text_ files with _text editors_ like the LearnIDE editor, Atom, Sublime
Text, vim, or emacs.

> **ASIDE:** You might hear some developers call text files
> "[plaintext][plaintext]" or "[plain text][plaintext] files" They all mean the
> same thing.

#### The Curious Case of Word Processing Files

What about files made by word processors Microsoft Word or MacOSX's TextEdit?
While you're typing text, those programs store the text _as well as
information_ about the text (which font to use, which words are in bold,
whether these next five lines are part of a bullet-list, etc.) in the _same_
file.  To make the loading and saving fast, these programs save the file in
_binary_.

#### Word Processors and HTML, Code

Since word processing programs store their output in _binary_ files and
programs that read HTML (like browsers) or run code (like Ruby, Python,
JavaScript, or Java) need _text_, **Word Processors should not be used to
create HTML or code.  Developers do their work in _text editors_, not _word
processors_.**

## Identify the Function of File Extensions

Many file names have an "extension" that comes after a `.`. It is not a
requirement, but it's a best practice. The extension is a "hint" to the
operating system of which program should be used to work with the file.  For
example, `LetterToGrandma.docx` has a *docx* _extension_ which _hints_ to the
OS that it should open the file with the Word word processing program by
Microsoft. The file `job_offer.pdf` _hints_ to the OS that it could open the
file with either Acrobat or MacOSX's Preview application. When the OS finds
many good options, it will ask for the user's help in selecting the right program.

Changing an extension **does not** change the type of file you have.  A text
file called `groceries.txt` could be renamed `groceries.mp3` **but it would
still be a text file**. A Toyota with a BMW medallion does not suddenly become
a BMW. Our `groceries` did not suddenly become music because we changed the
extension.

Some operating systems, like MacOSX _hide_ the file extension by default.  They reckon
that most users "no longer care about it." Since we're
developers, though, we will frequently dig below the "end-user" layer. When in
a terminal, we will see full file names - including extensions.

Here's a table to help train your instincts in seeing text- files versus
binary-files:

|File | Text or Binary | Extension | Use |
|-----|---------------------|-----|------|
| `beethoven_09_04_.mp3` | Binary | `.mp3` | Recording of the "Ode to Joy"|
| `CarletonDance.gif` | Binary | `.gif` | Image of a dancer from "The Fresh Prince of Bel-Air"|
| `fibonacci_printer.py` | Text | `.txt`| A Python program written in text; executable by the `python` _binary_ file |
| `index.html` | Text | `.html`| An HTML File designed for sharing information on the web|
| `LetterToGrandma.docx` | Binary | `.docx` | A binary file for Microsoft Word |
| `minaswan.rb` | Text | `.rb` | A Ruby program file written in text; executable by the `ruby` _binary_ file |
| `cannonball.mov` | Binary | `.mov` | A movie showing someone jumping into a swimming pool **Splash!**|

## Conclusion

In this lesson we have taken some time to get to know files. Files are things
in which computers store data that needs to last a while or which their users
might want to refer to again later. We've noted that files generally come in
binary and text formats.  And we saw that many files also have an extension
which provides hints about which program should be used to work with the file.

[plaintext]: https://en.wikipedia.org/wiki/Plain_text
