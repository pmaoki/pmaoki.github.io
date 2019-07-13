---
title: personal
layout: main
---
# Some facts about me

## Trivia

* I'm a [**Navy veteran**](USN/navy.html).
  That gets me [employment
  preference](https://www.opm.gov/policy-data-oversight/veterans-services/vet-guide-for-hr-professionals)
  at the Post Office.
* I've been &ldquo;[**mentally contaminated**](930108.oppose.html)&rdquo; since '85.
* [**Hidamari no tami are strangely soothing**](https://web.archive.org/web/20180705140229/http://tinkerville.cutthatout.com/hidamari/).
* **Go Bears!** Golden Bears in my immediate family include my dad's
  dad (business), my dad (electrical engineering), my sister (French
  literature) and countless cousins.  The &ldquo;all-Cal&rdquo;
  experience is one I have in common with [Jim
  Gray](http://research.microsoft.com/~gray/) (B.S. '66, Ph.D. '69),
  [Marti Hearst](http://sims.berkeley.edu/~hearst/) (B.A. '86,
  Ph.D. '94), among others.
* Prototypes have a life of their own. Some [**University POSTGRES
  applications that gave us pause**](pgapps.html).
* Sometimes, so do class projects.  I was surprised to find that one
  of mine had been used for [**course readings**](web.html) at several
  universities.
* Sadly, my
  [**Erd&ouml;s number**](erdos.html)
  is no longer smaller than 
  [Dourish](https://www.ics.uci.edu/~jpd/misc/erdos.html)'s.
* **Yes, the  &ldquo;M&rdquo; is there for a reason.**
  You wouldn't think this would be a problem, but it turns out that
  there are other people named &ldquo;Paul Aoki&rdquo; doing
  computer-related research, notably [Paul
  K. Aoki](http://depts.washington.edu/llc/People_Admin.php) at UW.

## Software experience

I've worked on several different medium-large software systems
(<em>i.e.</em>, systems in the ballpark of 100-1000 KLOC - that's
total size, not how much I wrote!). Outside of the companies for which
I've worked full-time post-Ph.D., I've written software for:

* **Illustra Information Technologies**<br/>
  The first commercialization of POSTGRES.  Formerly known as
  Mir&oacute; Systems and Montage Software; acquired by Informix
  Software, which is now part
  of <a href="http://www.software.ibm.com/data/informix/">IBM</a>.
* [**Garlic**](https://web.archive.org/web/20181117140139/http://www.almaden.ibm.com/cs/garlic/)<br/>.
  A heterogeneous multimedia object management project at
  IBM [Almaden Research
  Center](http://research.ibm.com/labs/almaden/), which became part of DB2 DataJoiner.
* [**Mariposa**](http://mariposa.CS.Berkeley.EDU/)<br/>
  A distributed DBMS project that formed the basis for Cohera;
  acquired by [PeopleSoft](http://www.peoplesoft.com/), which is now
  part of [Oracle](http://www.oracle.com/).
* [**Sequoia 2000**](https://web.archive.org/web/19990125091755/http://s2k-ftp.cs.berkeley.edu/)<br>
  A global change research project that included a large geospatial
  database component.
* [**POSTGRES**](http://db.cs.berkeley.edu/postgres.html)<br/>
  One of the original
  &ldquo;[object-relational](http://en.wikipedia.org/wiki/Object-relational_database)&rdquo;
  DBMS systems, and the basis for Illustra, Cohera,
  [PostgreSQL](http://www.postgresql.org/),
  [EnterpriseDB](http://www.enterprisedb.com/), etc.
* **General Electric**<br/> 
  I worked briefly at Ilex Systems, a company that did contract work
  on a nuclear reactor core monitoring system written by GE's
  [commercial nuclear reactors](http://www.gepower.com/nuclear/)
  (3D-MONICORE).  This was actually more fun than it sounds like when
  I describe it (largely thanks to the utterly crazy [John
  Plevyak](http://www.plevyak.com/), but don't tell him I called him
  that...), but it also convinced me that writing new software is a
  lot more fun than maintaining old software.

## Hacks 'n' patches

Most of my open source code has to do with research projects -- these
are basically gists, from the days before GitHub. Grab what you like,
but be warned that I'll probably trash any email I get about this
stuff.

* [<tt>hilbert.shar</tt>](../software/hilbert.shar)<br/>
  This is a hacked-up version of the Hilbert code generator from the
  [Utah Raster Toolkit](https://github.com/sarnold/urt/).  Through the
  use of the GNU Integer class, it has been extended to support up to
  32 dimensions and 32 bits of resolution (though CPU and space
  requirements are unlikely to allow both at the same time).
* [<tt>sphere.patch.amd64</tt>](../software/sphere.patch.amd64)<br/>
  Some fixes for the NIST SPHERE 2.6a distribution of speech audio
  tools.  (The base distribution from 1997 can be
  found [here](ftp://svr-ftp.eng.cam.ac.uk/pub/comp.speech/tools/).)
  The patch enables the distribution to compile and pass its
  regression test suite under Ubuntu 10.04 amd64.  However, before
  bothering with this, you should really look
  at [LDC's page](http://www.ldc.upenn.edu/Using/) on
  dealing with SPHERE-formatted data, and make sure that you can't
  just use [SPHERE 2.7](https://www.nist.gov/itl/iad/mig/tools) from
  2012 :-).
* [<tt>ich4-rh73.patch</tt>](../software/ich4-rh73.patch)<br/>
  A context-diff patch for Linux kernel 2.4.18-5 to make it recognize
  the IDE controller in the Intel ICH4 chipset (as used in, e.g., the
  Dell Optiplex GX260 and Dell Precision Workstation 650 series).  You
  can install RH 7.3 fine without the patch, but the IDE controller
  will be operating in PIO mode...reading a DVD can drive CPU
  utilization to 100%.
