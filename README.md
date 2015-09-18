# Halide-Binaries

These are Windows builds of Halide.dll.

Why not use the standard Windows binary downloads that the Halide team produces?

The reason is because they only publish a Release build, which links Halide.dll to MSVCRT120.dll and MSVCP120.dll.
When experimenting, we want to use our Debug build configuration, and this causes heap incompatibilities between MSVCRT120.dll and MSVCRT120d.dll.

I expect the Release mode binaries in here to be very similar to those produced by the Halide team.

NOTE: The only .dll inside here that was produced by us is vs2013/x64/Debug/Halide.dll
The others are from the Halide team.
I'll eventually compile them all consistently, if we're using this in production.