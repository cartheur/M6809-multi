# M6809-multi

---
DOCUMENTATION: For instructions and other documentation for these files, refer to the Wiki (use the link at the top of the page). You might not see the link if you are using a mobile device -- you may need to select "desktop version"
---

I always wanted a 6809 machine. I still have the A4 notebook where I sketched out design ideas. However, I never simultaneously had the time and money to build one from scratch (even though I have accumulated all of the parts in my junk box over the years).

When I saw this http://searle.hostei.com/grant/Multicomp/index.html I realised I could satisfy my yearning without too much soldering.

I decided that I would run Brad Rodriguez's Camelforth on it. Before I did that I resussitated a 6809 emulator and added crude support first for Brad's "scroungmaster" machine and then for the 6809 multicomp machine. That emulator is https://github.com/nealcrook/exec09.

Camelforth is currently running on real hardware. Using a hardware bank-switching unit on multicomp Camelforth can also act as boot loader for Grant's port of Microsoft ROM BASIC and for the N8VEM port of Dave Dunfield's CUBIX and for my ports of FLEX, NitrOS-9, BUGGY and FUZIX. All of this also runs on exec09.

This repository is a venue for sharing the hardware and software that I have used on my multicomp.

For detail on how to use any of this stuff, click on the "wiki" button on the right.

More on CamelForth here:
https://launchpad.net/camelforth
http://www.camelforth.com/
http://www.bradrodriguez.com/papers/index.html

Approximate WIKI Change Log:

03Feb2016 Rework FLEX stuff to add more detail and make it clearer

05Feb2016 Rework CUBIX stuff to describe new single-step boot. Remove references to obsolete SDINIT.

12Feb2016 New BUGGY source code - single step now works. Expanded WIKI pages on CamelForth to add some links on tutorials. New versions of TERMINAL and UART VHDL to add functional reset of input FIFOs to avoid some start-up problems.

09Aug2018 Tidy-up pass - adding a few misisng files and scripts and generally tidying things up. In particular, clean up the build process for the 6809 ROM BASIC and add some images for simulation debug.

06Mar2019 Reorganisation to try to provided consistent descriptions for each operating environment: the original material  evolved over time as I ported successive bits of code and it shows (too much) in places.

24May2020 WIKI was a mix of creole and markdown. I am gradually migrating all the pages to markdown, making various small updates on the way. Expand the pages on camelforth to describe how to build it at a different start address.
