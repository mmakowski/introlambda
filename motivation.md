Hi, my name is MM and this is not going to be a talk about Scala. Given that
this is Scala user group meetup, you might feel cheated, so let me remediate
that by trying to explain why you might care anyway.

In engineering disciplines the designers of a given machine or structure can
usually say something about its properties: this engine will generate 300 Watts
of power, this building can withstand earthquake of magnitude 4 in Richter
scale. I write software for a living -- mostly in Scala, nowadays. These are
business applications that pump data from one place to the other, sometimes
reshaping and recombining it on the way. In my experience, in this domain
any absolute guarantees about the behaviour of the system are very uncommon. 
We use acceptance tests to check what the system *will* do, but as is the 
case with all example-based tests, it cannot provide guarantees as to what the 
system *will not*, under any circumstances, do.

Many of us have heard of scalaz and shapeless projects, and perhaps even about
the principles of functional programming and dependently-typed programming those
projects are based on. Those techniques purport to provide some guarantees about
the software that we write: "this piece of code will never perform any IO" (not 
really possible in Scala), "this function will always yield a sorted list" and
so on. However, for many run-of-the-mill programmers such as myself there is
all this intimidating terminology that might be off-putting and stop
us from taking advantage of those powerful tools.

The bad news is, there is no easy way to enlightenment. Proper understanding of 
advanced functional and type-level techniques requires a lot of learning. 
The good news is that first steps in this learning are very easy. The fundamental 
formalism that underpins all of this, the lambda calculus, is really easy to get 
to grips with. This talk is meant to show you the lay of the lambda-land and 
give some pointers where to look next if you wanted to learn more. To be clear:
there won't be any practice in it, you won't go away and think: "right, let's
put it to use now". But hopefully, it will pique your interest in the subject
and give some ideas where to go next.

-- plan of the talk

I do not assume any theoretical background, just programming experience. The
concepts we will discuss should be really straightforward, so if anything is 
unclear then please ask questions immediately.
