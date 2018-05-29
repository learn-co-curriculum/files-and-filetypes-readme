# Files, Extensions, and File Types

## Problem Statement

According to the influential [paper][seven] "The Magical Number Seven, Plus or
Minus Two," published in 1956 by George A. Miller, the number of objects that
an average person can hold in _working memory_ is about seven. Recall the last
time you tried to memorize a phone number, URL, or address "for a second" as
you tried to type it in. After you keyed in that information, you probably
experienced relief because it has been _safely_ stored and, 20 minutes later,
you could not have recalled the number. This information was temporarily, and
riskily, stored merely in _working memory_.

Sometimes, when doing computation, we need to be able to store our results or
processes for re-use or review.  Humans preserve temporary information (phone
numbers, our share of the dinner cheque) on Post-It Notes, the arrangement of
beads on an abacus, in the counting knots of Inca _quipu_, or a note-taking
app on their smartphone.

Similarly, computers have a limited (although presently it's quite large!)
amount of working memory (called RAM) which they can access and use very
quickly.  However, sometimes they, too, need to write results somewhere safe
either because the data is so big that their working memory is exhausted **or**
because the data is useful and might need to be reviewed at some later point.

Computers write data that needs to be durable into **files**.  As
technologists, we're going to be creating _lots_ of files. We need to
understand the vocabulary that the craft uses to describe files so that we're
able to follow documentation and communicate with one another. That's what
we'll learn more about in this lesson.

## Objectives

1. Define what a file is
2. Contrast the function of _text files_ and _binary files_
3. Identify the function of file extensions

## Define What a File Is

While you may have used these computers for years, you might not have ever
considered what a "file" is. You've certainly downloaded them, saved them, and
deleted them. A file is a thing computers use to store data or processes
(programs) for later use.

## Contrast The Function Of Text Files And Binary Files

In the earliest days of computing, the users of the ancestors of modern
computers recognized two primary types of files: **text** files and **binary**
files. Stored data tended to live in **text** files while stored processes,
also known as "programs" tended to live in executable files written in the
**binary** language that computers use internally. This created the primary
division in file types: **text** and **binary**.

### An Unnecessary Adjective? "Plain"

Perhaps as an unnecessary adjective, computer users put the adjective "plain"
in front of "text" to emphasize _just how utter plain and human-oriented_ the
contents were. For this reason, these files are occasionally called "[plain
text][plaintext]" or "[plaintext][plaintext]." These all refer to the same
thing, though, files full of things that humans can type on their keyboards.

### Experiencing File Types

**(Plain) Text** files are designed for _humans_ to read and write with editors
like LearnIDE, Atom, Sublime Text, vim, or emacs (notably, **not** Microsoft
Word or TextEdit - more on those in a moment!).

**Binary** files are designed for _computers_ to read and run (or "execute").
These files contain instructions, written in binary (the format computers think
in) that describe how to do something. In general, if a computer is doing much
of anything that involves processing and transforming data, it's working with a
binary file.  Every video game, every DVD, every CD is effectively _one large
file_ written on a disc (or downloaded) in the _binary_ format.

### The Curious Case of Word Processing Files

Word processing programs (for example: Microsoft Word on your computer, MacOS'
"TextEdit" program), provide a confusing case. While you're _seeming_ to edit
text, Word stores your text _as well as information_ about the text (which font
to use, which words are in bold, whether these next five lines are part of a
bullet-list, etc.) in the file. Most word processing document files, therefore,
are _actually_ stored in binary files.

As additional context, since word processing programs emit _binary_ files,
they're unfit to be used to create HTML documents (and indeed, unfit to write
source code for use by programs like `python` or `ruby`). Technologists write
their computer-friendly documents in a "text editor" but tend to write business
documents, letters to grandmothers, and Southern Reach trilogy fan fiction in
word processors. Text Editor programs differ from Word Processor programs
because they emit their save files as **text** files.

## Identify the Function of File Extensions

Many file names have an "extension" that comes after a `.` which suggests what
type of program works with the file or what kind of data lies inside the file.
For example `LetterToGrandma.docx` has a *docx* _extension_ which suggests the
Word word processing program by Microsoft. The file `groceries.txt` has a *txt*
extension which suggests a plaintext text editor like Notepad or Atom. The
`CarltonDance.gif` file's extension of `.gif` suggests an image, possibly
animated. When people say they "I went to giphy.com to find a GIF" they're
really saying: "I used the giphy.com search engine to find files that have the
`.gif` extension."

**BUT** be careful. A text file called `groceries.txt` could be renamed
`groceries.mp3` **but it would still be a text file**. Just because you put a
Mercedes-Benz medallion on the front of your Toyota _does not mean_ that you're
driving a Benz. A look at the internals would quickly reveal that the label did
not match the manufacture.

Operating systems use these extensions to help decide what sort of tool ought
be used to read and process the file. Some operating systems, like MacOS, even
_hide_ the extension on the theory that that most "no longer care about it."
This is probably a reasonable conclusion, but as technologists we're going to
frequently dig below the "end-user" layer. Since the LearnIDE environment we're
going to be working on is based on Linux, we _will_ see the extensions on
files.

Here's a table to help train your instincts in seeing text- files versus
binary-files:

|File | Plaintext or Binary | Extension | Use |
|-----|---------------------|-----|------|
| `beethoven_09_01_.mp3` | Binary | `.mp3` | Music influenced by German Idealist poetry|
| `CarletonDance.gif` | Binary | `.gif` | Image of the dance genius Alphonso Ribiero |
| `fibonacci_printer.py` | Plaintext | `.txt`| A Python program written in text; executable by the `python` _binary_ file |
| `index.html` | Plaintext | `.html`| An HTML File designed for sharing information on the web|
| `LetterToGrandma.docx` | Binary | `.docx` | A binary file for Microsoft Word |
| `minaswan.rb` | Plaintext | `.rb` | A Ruby program file written in text; executable by the `ruby` _binary_ file |
| `cannonball.mov` | Binary | `.mov` | A Quicktime movie showing someone jumping into a swimming pool **Splash!**|

## Conclusion

In this lesson we have taken some time to get to know files, things in which
computers store data that needs to last a while or which their users might want
to refer to again later. We've noted a primary distinction between (plain-)
text files and binary files and noted that many files also bear an extension
which provides hints (_but does not authoritatively decide_) whether a file
contains binary or textual data.

This lesson has described files in a way that's intuitive and has analogs to
daily life. If you want to puzzle on a more technical definition here's a
starting point: "A file is a sequential arrangement of bytes persisted to a
durable medium." See if you can make that definition work for both _binary_ and
_text_ files in your own understanding!

[seven]: http://www.musanim.com/miller1956/
[plaintext]: https://en.wikipedia.org/wiki/Plain_text
