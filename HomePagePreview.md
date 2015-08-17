[![](http://piccolo2d.googlecode.com/svn/site/images/Piccolo2D-Logo.png)](http://piccolo2d.mro.name/)

If you're interested in _using_ the structured 2D graphics toolkit Piccolo2D, see the [Piccolo2D Homepage (current refuge)](http://piccolo2d.mro.name/). This page here is about the development of the toolkit itself.

# Welcome to Piccolo2D!
A revolutionary way to create robust, full-featured graphical applications in Java and C#, with striking visual effects such as _zooming_, _animation_ and _multiple representations_.

Piccolo2D is a toolkit that supports the development of 2D structured graphics programs, in general, and [Zoomable User Interfaces](http://en.wikipedia.org/wiki/Zooming_User_Interface) (ZUIs), in particular. A ZUI is a new kind of [user interface](http://en.wikipedia.org/wiki/User_interface) that presents a huge canvas of information on a traditional computer display by letting the user smoothly zoom in, to get more detailed information, and zoom out for an overview.

We use a [scene-graph](http://en.wikipedia.org/wiki/Scene_graph) model that is common to 3D environments. Basically, this means that Piccolo2D maintains a hierarchical structure of objects and cameras, allowing the application developer to orient, group and manipulate objects in meaningful ways.

# Why use Piccolo2D?
It will allow you to build structured graphical applications without worrying so much about the low level details. The infrastructure provides efficient repainting of the screen, bounds management, event handling and dispatch, picking (determining which visual object the mouse is over), animation, layout, and more. Normally, you would have to write all of this code from scratch. Additionally, if you want to build an application with zooming, that’s built right into the framework too.

# What exactly is it?
Piccolo2D is a layer built on top of a lower level graphics API. There are currently [three versions](http://www.piccolo2d.org/learn/comparison.html) of the toolkit:
  * Piccolo2D.Java,
  * Piccolo2D.NET and
  * PocketPiccolo2D.NET (for the .NET Compact Framework).

The java version is built on Java 2 and relies on the Java2D API to do its graphics rendering.

The .NET version is built on the .NET Framework and relies on the GDI+ API to do its graphics rendering. This makes it easy for Java and C# programmers, even those targeting PDAs, to build their own animated graphical applications.

And best of all, Piccolo2D is _free_ and _open source!_

# How do I get it?

Google Code hosting no longer allows new downloads to be created, so all recent Piccolo2D.Java versions are available only through the [Maven Central repository](http://search.maven.org/#search|ga|1|g%3A%22org.piccolo2d%22) or via release tag in the subversion repository.

The latest version of Piccolo2D.Java compatible with JDK versions 1.6 or newer is [3.0](http://search.maven.org/#search|ga|1|g%3A%22org.piccolo2d%22%20AND%20v%3A%223.0%22).  The svn release tag is [tags/piccolo2d-complete-3.0](http://code.google.com/p/piccolo2d/source/browse#svn%2Fpiccolo2d.java%2Ftags%2Fpiccolo2d-complete-3.0).

The latest version of Piccolo2D.Java compatible with JDK versions 1.5 or newer is [2.0](http://search.maven.org/#search|ga|1|g%3A%22org.piccolo2d%22%20AND%20v%3A%222.0%22).  The svn release tag is [tags/piccolo2d-complete-2.0](http://code.google.com/p/piccolo2d/source/browse#svn%2Fpiccolo2d.java%2Ftags%2Fpiccolo2d-complete-2.0).

The latest version of Piccolo2D.Java compatible with JDK versions 1.4 or newer is [1.3.2](http://search.maven.org/#search|ga|1|g%3A%22org.piccolo2d%22%20AND%20v%3A%221.3.2%22).  The svn release tag is [tags/piccolo2d-complete-1.3.2](http://code.google.com/p/piccolo2d/source/browse#svn%2Fpiccolo2d.java%2Ftags%2Fpiccolo2d-complete-1.3.2).

<br />

Learn more at the [Piccolo2D Homepage (current refuge)](http://piccolo2d.mro.name/).