# "Blog"

This page is a log of thoughts that I am yet to organize into pages. Maybe I'll discover that I should have a proper
 blog, but for now this is a lightweight approximation that seems fine.

## 2019-11-06 10:32

Let's write about my second day at RC. In the morning, I did a pair programming workshop. After a cute intro, we split
into teams to pair on implementing a version of [Mastermind](https://en.wikipedia.org/wiki/Mastermind_(board_game )). My
partner and I swapped driving and navigating roles every 20 minutes with a timer, and we chose to program in Python
using VSCode. Although we didn't finish an implementation before we decided to break for lunch, I enjoyed the
back-and-forth. I'd definitely like to pair with a variety of people while at RC.

In the afternoon, pairing happened again! :) I had signed up for auto-pairing Tue-Thu via RC's pairing bot on Zulip ,
and I was matched with someone for the afternoon. I had been continuing my self-intro to Julia, and my partner noticed
that I had open both the Julia manual and Jupyter notebook running a Julia kernel. He suggested we do something in
Julia. Yay! However, I wasn't in the middle of some project for which we could implement a piece. I suggested that we
tackle a problem on [Project Euler](https://projecteuler.net/). He hadn't heard of this site , but was supportive after
I introduced it. We ended up solving one problem with me driving and then another with him driving. It was a fun way to
scramble about mapping ideas we both had about how to solve things to how to do so in Julia. I had never written a
function in Julia before, so "How do we write a function?" happened, as well as "Can we do a list comprehension in
Julia?" (we were both familiar with so-called list comprehensions in Python). One of the problems seemed to have a
straightforward solution if only we could do arithmetic involving giant (like 100^100) numbers, and I had just read
about the `BigInt` type in Julia; it was a joy to apply something so immediately.

After pairing, I went for a chat with someone new at RC. We were auto-connected via another bot on RC's Zulip, the "chat
bot", formerly known as the coffee bot, but since the crux is for two people to chat and not necessarily to drink a cup
of coffee in concert, it was renamed. We got some boba ("bubble milk tea"), which I love as part of a walk. I learned a
bit about dependent types, and spoke a bit about my interest in Julia. I had signed up for matchings Tue-Thu; I look
forward to this organized yet low-commitment way of just getting to know a variety of people during my time here.

## 2019-11-04 16:44

My first day at RC was a whirlwind. I enjoyed it, but definitely high-energy. Met a lot of folks in a well-organized way
(a handful of three-minute pairings with others), and then had lunch in a group of eight. When I got back to RC around
2:15, the Big Open hit me. What now? I went on Zulip, signed up for pairing and coffee chats with the respective bots,
and went through email. I poured a cup of coffee for myself and decided to browse the book jackets of RC's tiny
 library in anticipation of a moment during my batch when I'm puzzled and then have a "wait -- there's a book here on
  that!" realization. Time will tell.
  
My idea for a first project is to (1) get familiar with the [Julia](https://julialang.org/) language and then (2) write
a toy [density functional theory (DFT) code](https://en.wikipedia.org/wiki/Density_functional_theory ) in it
Specifically, I want to (2a) review Mikael Kuisma's [DFT code in one hour with
MATLAB](https://www.youtube.com/playlist?list=PLyifek164UUJk8PplzS56VvWZM8KgFqbk) and Tomas Arias' [Practical
DFT](http://jdftx.org/PracticalDFT.html) six-lecture mini-course (taught in Octave, an open-source MATLAB equivalent),
and then (2b) adapt the given code to Julia. These sources in particular seem useful because Julia is often marketed as
an "upgrade" to MATLAB (offering familiar syntax) for people. Thus, I should have some room to think about code
organization/design and not need to dwell much on low-level details that that be surmised from the MATLAB/Octave code
. I am hoping that I can accomplish all of the above in two weeks, one week for (1) and then another week for (2a-b).