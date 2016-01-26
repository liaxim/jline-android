# jline-android
New JLine for Android 4.4+ with Telnet support based on new NVT4J

This project is based on jline, a Java implementation of the line editing library (libreadline).
See Jline project: http://jline.sourceforge.net. The source code is based on https://github.com/jline/jline2.
jline2 supports Windows and Mac arrow keys without the need of external keymap files.

The source code is cleaned up to allow it to compile on Android 4.4+ (API 19+).

To use jline in a debug shell for Android framework / applications, a Telnet layer is needed to negotiate
capabilities of the virtual terminal. NVT4J is used as the Telnet layer because it has a cleaner interface
to integrate with general Java I/O interfaces (InputStream, OutputStream and Socket).
