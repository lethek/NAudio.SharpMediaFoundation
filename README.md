NAudio.SharpMediaFoundation
===========================

Alternative MediaFoundation support for NAudio using SharpDX for interop. Provides alternative implementations of the four main NAudio Media Foundation support classes/

 - SharpMediaFoundationReader
 - SharpMediaFoundationEncoder
 - SharpMediaFoundationResampler
 - SharpMediaFoundationTransform

A sample WPF application shows how they can be used in the same way that the standard .NET Media Foundation classes are used.

Benefits compared to using the standard NAudio classes:

 - Create a reader from a standard .NET stream
 - Encode to a standard .NET stream
 - Reader does not need to recreate its internal COM object when accessed from another thread
 - Probably performance is better (although see note below)




Installing
==========

Currently you'll need to do your own build. Download the source and build it. Then reference all the following DLLs:

 - NAudio.dll
 - SharpDX.dll
 - SharpDX.MediaFoundation.dll
 - NAudio.SharpMediaFoundation.dll
 
It is built against .NET 4, and should work just fine with .NET 4.5, 4.5.1, 4.7.1 etc.
