joe-editor
==========

My fork of Joe's Own Editor

clone::

	hg clone http://joe-editor.hg.sourceforge.net:8000/hgroot/joe-editor/joe-editor

import::

	git init
	hg-fast-export


Compilation instructions
-------------------------

To compile joe::

	./autojoe

Then::

	./configure

And build it::

	make

And finally to install (optional)::

	make install

Description
--------------

From: http://joe-editor.sourceforge.net/

JOE is a full featured terminal-based screen editor which is distributed
under the GNU General Public License (GPL).  JOE has been around since 1988
and comes standard with many Linux distributions.

JOE is being maintained by its original author Joseph Allen, plus all of the
people who send bug reports, feature suggestions and patches to the project
web site.  JOE is hosted by SourceForge.net and its source code is
controlled under CVS.  Over the last few years there has been about one
major new release a year, usually in the April-May timeframe.

JOE is a blending of MicroPro's venerable microcomputer word processor
WordStar and Richard Stallman's famous LISP based text editor GNU-EMACS (but
it does not use code from either program): most of the basic editing keys
are the same as in WordStar as is the overall feel of the editor.  JOE also
has some of the key bindings and many of the powerful features of EMACS.

JOE is written in C and its only dependency is libc. This makes JOE very
easy to build (just "configure" and "make install"), making it feasible to
include on small systems and recovery disks.  The compiled binary is about
300K in x86.  Note that JOE can use either the termcap or terminfo terminal
capabilities databases (or a built-in termcap entry for ANSI terminals). 
The choice is controlled by a "configure" option.  If terminfo is used, a
library is required to access the database (on some systems this library is
ncurses, but JOE does not use curses to control the terminal- it has its own
code for this).

Much of the look and feel of JOE is determined by its simple configuration
file "joerc".  Several variants of the editor are installed by default in
addition to "joe": "jmacs" (emulate GNU-EMACS), "jstar" emulate WordStar,
"jpico" emulate the Pine mailer editor PICO and "rjoe"- a restricted version
of JOE which allows the used to only edit the file given on the command
line.  JOE is linked to several names.  The name which is used to invoke the
editor with "rc" tacked on the end gives the name of configuration file to
use.  It is thus easy for you to make your own variant if you want.  Also
you can customize the editor by copying the system "joerc" file to your home
directory.
