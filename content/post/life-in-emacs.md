+++
title = "My life in emacs"
author = ["Alain Picard"]
date = 2020-08-11T00:00:00+10:00
tags = ["emacs", "advice", "nostalgia", "tech"]
draft = false
+++

## In the beginning... {#in-the-beginning-dot-dot-dot}

I've been using [GNU Emacs](https://www.gnu.org/software/emacs/) pretty much daily since 1991, when I got
kicked off _deimos_, a VAX-780 in the astronomy department at Caltech.
Well, I didn't just get kicked off of it... it stopped existing, as
vaxen fell out of fashion for being cost ineffective, and the department
made the transition to a Convex, a now defunct super minicomputer.  But
that's a story for another day.

Finding myself with a brand new Sun Sparcstation, I then had to find
another editor (at the time, I was a wiz on VMS's `EDT` editor) to write
my thesis, the manuscript of which was going to be written in TeX.  My
choices seemed to be `vi` and `emacs`, as even then I (correctly) intuited
that sticking with an emulator for a defunct system was probably not a
good long term strategy.

Emacs had this nice mode called [AUCTeX](https://www.gnu.org/software/auctex/) to facilitate
authoring [TeX](http://www.tug.org/) documents.  I took the plunge, and have never looked back.
I of course totally fell for the tinkerer's malady which affects most
new emacs users, and spent more time exploring and configuring emacs
that writing my thesis (standard work avoidance tactics).

As I think back about my career in programming, it seems odd that such
an... _accidental_ choice ended up having such a deep impact on me.  Later,
I would come to appreciate emacs as a "programmable editor", learn lisp,
and eventually even build a company's technological core on [Common Lisp](https://common-lisp.net/);
I'm quite that would never have happened had I not had my eyes opened to
the existence of such deeply interactive and evolveable systems.


## Happy, productive years go by {#happy-productive-years-go-by}

The next two decades saw me _living_ in emacs.  From version 18.57,
emacs rapidly developed into an actual GUI application (whoa!  modern!)
with the 19.X release.  Then we were off the the races.
Working in `C++`, then `lisp`,
reading/writing mail and usenet (using `VM` and, later, [GNUS](http://www.gnus.org/)), various
folding modes (until the category killer, [org-mode](https://orgmode.org/) appeared in 2003),
version control (first with SVN, then [mercurial](https://www.mercurial-scm.org/), and, finally the
most wondrous [magit](https://magit.vc/), which rescues the horrible `git` from the pathetic
mess that is its UI); emacs gave me loyal service during countless
hours.

Cryptography, programming, editing remote files, diffing, rectangle
modes... my motto became "The Answer is Emacs.  Now, what was the
question?"  Even better, as computers got faster, emacs' reputation
for being slow and resource hungry began to fade, and now this appears
quaint, as single purpose applications like `slack`, a glorified IRC
system, dwarf emacs in terms of resource usage.

Startup time?  Not a problem if you never leave it; this
session is shorter than most...  I remember getting to over
a year of uptime once.

```lisp
(emacs-uptime)
"23 days, 7 hours, 41 minutes, 24 seconds"
```

I'm guessing I had to reboot my computer for some reason...


## Teaching emacs {#teaching-emacs}

I guess I sort of ended being the emacs guru and evangelist wherever
I went, so I ended up teaching emacs to quite a few people.  I discovered
an interesting phenomenon: many people took to emacs quite enthusiastically,
but usually for different reasons!  It seems emacs has many faces, and
people need to discover their own "killer app" to see the light.

Of course, today, many, many more special purpose tools and IDEs exist
which provide much of this functionality straight out of the box
(often better), it is difficult to justify the emacs way.  Add to this
that the emacs terminology is antiquated (a "window" in emacs doesn't mean
what you think, you want a "frame", you don't "cut and paste" in emacs,
you "kill and yank") it must feel like an alien and stubbornly archaic land
to a new user.  So why should they persevere?


## By their _tools_ shall ye know them {#by-their-tools-shall-ye-know-them}

_Expert_ tools are not designed like tools for beginners.  I watch
my younger colleagues, and many seem to be stuck in a form of arrested
development, paralyzed in a sort of "eternal beginner" state.  I think
it has to do with the idea of "user friendliness", which got (mis-)interpreted
as "beginner friendliness".  But a professional programmer isn't (or, at
least, shouldn't _stay)_ a beginner!  I watch them move the mouse, click,
drag, cut, scroll (again, with the mouse), click and finally paste... and
mentally calculate how long that took, how many times a day they do it,
how many days in their life they will do it for... and despair.  Not to mention
to mental interruption to the flow imposed by each of these tiny delays, each
of these additional bits of friction.

So let me be clear: I believe the young programmer should strive to make
their tool _disappear_ from their consciousness; the mechanical aspects of your
work should be as a musician playing his instrument: he thinks not of the
instrument but about the music.  The instrument "plays itself".

This is the realm in which emacs excels.  The reason for this is that it's
more a _meta tool_ than a tool.  The opening line of the emacs manual
is essentially unchanged to this day from my hardcopy version, sixth edition, 1987:

> Emacs is the extensible, customizable, self-documenting real-time
> display editor.

This emphasis on _extensibility_ and _customizability_ is the essence of emacs.
Emacs works the way _you_ do, not the way around.  That is why, unlike these
other "friendly" tools, it _never_ runs out of features, nor slows you down,
nor draws attention to itself.  The price you pay for this is climbing the
steep learning curve.  Did you think this was going to be easy?  Nothing
worthwhile ever is.


## Modern times {#modern-times}

These days I am deeply conflicted about whether or not to recommend to young
programmers that they follow this path; it's hard for me to gauge to what extent
the time I invested in learning this tool (and the rewards I got from it) are still
achievable today.  For me, the principal win has been that I could do just about
_all_ of my work from within emacs, thus compounding efficiencies as I switched
from one [mode](https://www.gnu.org/software/emacs/manual/html%5Fnode/emacs/Major-Modes.html) to another.  But the world has moved on, and working outside a
browser now becomes more and more difficult.  Even tools like the
[Edit with Emacs](https://chrome.google.com/webstore/detail/edit-with-emacs/ljobjlafonikaiipfkggjbhkghgicgoh) chrome browser extension only help marginally, because now
developers are made to use obnoxious tools like Jira, which (on purpose, I'm sure)
[prevent round tripping](https://www.atlassian.com/blog/archives/why-we-removed-wiki-markup-editor-in-confluence-4#comments) of their markup language to and from plain text (_i.e._ markdown).
Furthermore, even though I still read my mail from emacs, I have to pipe it
through the browser to properly view more than half of messages I now get.
I sure long for the days of plain ASCII email...

What advice would I give a young programmer choosing today?  I would
say you should still consider `emacs` if you are the type of person who
believes in expert tools.  Emacs is not flashy or pretty out of the
box.  Remember, think of emacs not as a finished product, but as a
_toolkit_ with which to create your own, custom work environment.  Emacs
is an _investment_: you'll have to _work_ at it.  You will either find
yourself falling down the rabbit hole, and enjoying the experience, or
totally bewildered and hating it.  Both are fine!

But if you think you'll still be doing this job in 20 years, if you want to
become ever more effective at it, if you want your work tool to become
an extension of your mind, then perhaps `emacs` _is_ for you, even now, in 2020.

You'll just have to find out for yourself, won't you?
