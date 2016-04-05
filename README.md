# `mimac` (Mum, I made a computer.)

Welcome!  You're either here because you got lost while surfing the internet, or because like me - you're fascinated by *stuff*.

`mimac` is a super tiny, incredibly simple computer.  It's not a physical one, it's emulated.  And it's free for anyone to make a copy to play with.  The only condition is you keep *your* copy free too.

# Why?

As I already said, I'm fascinated by stuff.  Computers fascinate me as much as anything else.  One thing that never ceases to amaze me is that the very same ideas which means you can turn a light on and off in your living room - allows you to surf the internet on your iPad.  The simplest of principles have been extrapolated to such a point that we begin forgetting what those simplest principles are, and just talk about the "more abstract" things instead.

So for example we talk about "processors" (or CPUs - "central processing units") rather than transistors and clocks.  When it gets to iPads, we don't even really talk about processors - rather we just talk about "apps" and stuff.

Therefore I've made `mimac`.  I took everything I know about computers - and boiled it down almost all the way to the simplest principles.  I didn't quite go all the way, because you can still do that by buying an good "learn electronics" kit from your local Radioshack or Maplin.

# Tell me more!

`mimac` is a tiny computer which runs in your browser.  It has a central processing unit (CPU), some memory (both volatile [lost when restarted] and non-volatile - all random access [RAM]) and some input/outputs (keyboard in, video out).

Theoretically you could *build* `mimac` in hardware.  I've made it run in your browser so it's costless and easy to get playing.

Like most computers, `mimac` has a bootloader or BIOS (basic input/output system) - a bit of software it always runs when you start it up.  For `mimac` - it simply checks if there is any instructions (software) already saved ("installed") in the non-volatile memory, and runs it - or asks you what to do otherwise.

The CPU understands 16 instructions - which are detailed further below.  You can tell the CPU what to do using those 8 instructions, and you can convert "human readable" instructions (written in a language called "C") into lists of those 8 instructions using an included compiler, which is an extension of another free project ([http://homepage.ntlworld.com/edmund.grimley-evans/cc500/]).

# Give me details of the CPU...

16 instructions.  I've listed their numbers in hex - `0x00` means `0`, `0x01` means `1`, `0x0A` means `10`, all the way up to `0x0F` (meaning `15`) which then goes to `0x10` (meaning `16`), etc.

They are:

***TBD - Probably just implement something like [https://en.wikipedia.org/wiki/Manchester_Small-Scale_Experimental_Machine] plus some useful shortcuts for common needs.
