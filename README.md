# Upslug2

**Note:** this repository is a fork from [wspringer](https://github.com/wspringer/upslug2)

I made only a _very_ [little fix](https://github.com/carlesso/upslug2/commit/e3d1163d130e588f91c863b2719018cab7470e38)
to be able to compile nowdays.

**ALL** credit goes to
* John Bowler <jbowler at users.sourceforge.net>
* Roger Nilsson [macosx support]

Thanks for your work. This Repository is also used as source for the [HomeBrew](http://mxcl.github.com/homebrew/) Formula to build it.

To install upslug2 with homebrew simply write:

```
  $ brew install https://raw.github.com/carlesso/upslug2/master/brew_formula/upslug2.rb
```


-----------------------------------

##This is upslug2.

upslug2 is a command line program intended to allow the upgrade of a LinkSys
NSLU2 firmware to new or different versions.  Unlike upslug and the LinkSys
(Sercomm) upgrade utilities upslug2 will synthesise a complete 'image'
from a kernel and a root file system, as such it duplicates part of the
functionality of 'slugimage'.

upslug2 also optimises the upload to avoid transmitted parts of the image which
need not be written or are 'blank' (set to the erased flash value of all 1's).

upslug2 is functionally similar to upslug, however it is not derived from
upslug.  It is a rewrite ab initio based on the following information:

1) Observation of the behaviour of upslug and of the problems upslug has
with the NSLU2 upgrade protocol.

2) Reverse engineering of that protocol for the purpose of writing a better
upslug.

3) Examination (but not copying or direct use) of the GPL
source code released by LinkSys and to be currently found at
ftp://ftp.linksys.com/opensourcecode/nslu2/
