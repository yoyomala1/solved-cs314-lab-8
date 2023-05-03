Download Link: https://assignmentchef.com/product/solved-cs314-lab-8
<br>
<span class="kksr-muted">Rate this product</span>

In this assignment you will explore some of the page frame reclaiming algorithms that you have read about.

1 Pick one by random

To set a standard and to see if we actually do something useful we first implement the algorithm where we select a frame by random. If we later

experiment with very complicated algorithms we hope that they behave better than the random, or why would we else bother to implement something

complicated.

Create a file random. c and open up your favorite editor. Don’t use an IDE that hide all the complicated things, use a regular text editor and do the compilation by hand from a command shell.

1.1 a random sequence

The first thing we shall do is to generate a random sequence of page identifiers. This sequence is the sequence of page references that we are going to

use in our benchmark of the algorithm. We could have generated these references on the fly but we need them when we implement the optimal strategy so we might as well do it now.

Below is you first go at the random. c program. It will only write out a sequence of random numbers but it’s only a start. Compile the code and do

a test run to see that it works.

*include &lt;stdlib

#include &lt;math.h&gt;

#include &lt;assert .

void init (int * sequence ,

for (int i

— 0; i&lt;refs;

sequence lil

rand ( )

int refs ,

%pages ;

int

pages)