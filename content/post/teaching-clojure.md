+++
title = "Teaching clojure"
author = ["Alain Picard"]
date = 2020-09-02T00:00:00+10:00
tags = ["clojure", "peopleware"]
draft = false
+++

## The Setup {#the-setup}

I had the opportunity recently to teach the [clojure](https://clojure.org) programming language
to a group of interns.  I was consulting for a client who wanted
to build a team of clojure developers to maintain and extend an
application he had commissioned earlier from a small consultancy.
I agreed to train and lead a team until we felt they were "safe
without the training wheels".

This was during the start of the COVID pandemic,
so the entire course was held remotely, via Zoom meetings, during six
weeks, with two classes of two hours each per week.  Thus 12 lessons,
totalling 24 hours of classes.  I expected the students to spend about two
hours for each hour of course work, so they ended up having to work at
least 12 hours per week.  (I was told later that they had, in fact,
had to work quite a bit more than what I had anticipated).

The students (there were four of them) were highly motivated;
this training was part of a recruitment effort, and two of them
would most likely be hired at the end of the training; so the
classes doubled as an extended evaluation period.  I felt comfortable
with this as this was all explained up front to the students, who
got a chance to get "free training from an expert", during a period
where they could not be employed anyhow.


## What **they** learned {#what-they-learned}

I rushed madly trying to prepare
[training materials](https://github.com/alain-picard/clojure-training), which were heavily based on the
excellent online book [Clojure for the Brave and True](https://www.braveclojure.com/clojure-for-the-brave-and-true/)
and the [clojure Koans](https://github.com/functional-koans/clojure-koans).  I had already had a chance to
review the application they would be maintaining, and so
knew that they would also to know clojurescript and the
most excellent [re-frame](https://github.com/day8/re-frame/) front end framework.  This meant
a _lot_ of material to cover, and I knew that just simple,
abstract exercises would not provide sufficient complexity
to get a flavour for "real" clojure programming, so I resolved
quite early on that the final outcome of the classes would
be the delivery of a small, but complete, web based application
which would be a clone of the [New York Times Spelling Bee](https://www.nytimes.com/puzzles/spelling-bee) word game.


## What **I** learned {#what-i-learned}

Teaching is _hard work_.  I guess I knew this; having run away from a
potential teaching career early on[^fn:1] but I ended up mentoring
quite a number of young colleagues throughout my career, and found
great satisfaction in seeing them grow.  I guess the distinction is
the degree of motivation of the student, and the intensity of focus.

Teaching clojure (and lisps in general) is deceptive: on the one hand,
the basic syntax of the language is so simple and easy to learn that
the student gets a sense of false confidence in their progress; on the
other hand, the tooling is unfamiliar (and somewhat unpolished) adding
a degree of unnecessary complexity.

Once the initial hurdle was over,
and we were able to dive into code and exercises, the next sticking
point was definitely trying to understand _functional idioms_.  None
of my students had been exposed to the ideas behind functional
programming at University.[^fn:2]  This did not greatly improve my
opinion of current CS and software engineering programs...
The students had familiarity with the following languages: Python,
Java, C# and a little C++.  These are all language from the same
"family", and follow largely an object oriented, mutable in place
approach to software design.  Getting the students to think outside of
this particular box was challenging, but rewarding.

One aspect which surprised me, though it perhaps shouldn't have, is
that one of the most valuable teaching aspect was the detailed code
review and criticism I gave back the students to all of their
exercises.  One student wrote, giving feedback at the end of the course:

> The biggest thing I found helpful in this course would definitely be
> the code review.  It really helps us improve our mindset and as
> programmers.

Where I was basically taking them through a process analogous to what
I normally follow with junior colleagues; _i.e._ extensive coding review
emphasising not only correctness, but style, layout, design, and, what
for lack of a better word I call _good taste_, my students had never had
such feedback on their code.  Their previous experience was submitting
software to some automated test runner which ran their code, and
getting a passing grade as soon as the code ran as specified in the
assignment.  So the greatest missing piece for them was probably the
realisation that having the code simply working was by no means
enough; the aim was to write _understandable_ code.

So, whereas universities are trying to "teach what industry wants" by
using what they think are "popular" languages, they actually fail to
instil some of the more important lessons about maintainability and
good taste.

In the end, this was most clearly exemplified by another
comment from one of my students, who said:

> I think I've learnt more about programming through this 45 day course
> than in my degree.


## Outcome {#outcome}

I was pleasantly surprised that all of my students succeeded in
delivering a fully working clone of the spelling bee puzzle (albeit
with hard-coded data, so no automatic puzzle generation)

The students actually became very collegial and helpful towards
one another, even though they were effectively in competition with
one another.  Don't believe the garbage that the millenials are
lazy entitled brats; these guys were hardworking and friendly, and
a pleasure to interact with.

The best thing to come of of this for me was that one of the
students who was "cut" from the group eventually managed to
convince my client to hire him anyway, so we ended up with a team
of three instead of two, and he ended up being an _excellent_ hire,
so I think we really lucked out.

I am, as of this writing, still engaged with this client and continue
to teach them, now as temporary acting CTO and tech lead, and will
have truly succeeded when I have managed to make myself redundant, and
they can fully take over the maintenance and future development of
the application!

[^fn:1]: I did teach an _Astronomy for Poets_ (_i.e._ introductory astronomy for non-scientists) at UCLA right after completing my doctorate. This episode convinced me that teaching was _not_ my vocation.
[^fn:2]: And they were all graduates, or soon to be graduates, of some of the best universities in Australia.
