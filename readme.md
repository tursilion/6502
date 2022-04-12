20070922

This is an experimental 6502 emulation core for the TMS9900. I got as far as stepping through the sample program included in 6502_9900.a99, and that was all the testing it got. It's slow, as might be expected.

It does not support decimal mode, but it does appear to run, at least for the embedded test program. I didn't take it any further than that and this is therefore presented mostly as a curiousity.

To run, load Editor/Assembler and use option #3 to load 6502_9900 (which is an uncompressed TI object file). Then run program START.

All it will display is a count of 6502 cycles per frame, in hex. Real time would be about >2080. This won't get even close, around >0120. ;)

Building it can be tricky - it builds into low RAM and so overwrites the Editor/Assembler #3 loader if you try to load it that way. I use my external tiobj2bin tool to convert it into a PROGRAM image first (and that image is what is provided.)

