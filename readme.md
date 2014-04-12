# Examples of open source work

All examples of work are Java and Android based. .  I have been building up the underlying code required by my own project of producing a game, which is an isometric simulation world.  This has introduced me more advanced UI work with Android (such as Fragments), using a game framework, introducing LOG4J for logging purposes, ANT to build projects and also creating custom tools. 

The following links are to my branch of a popular Android 2D game engine, the code I have added or modified can be viewed in the second link.

[https://github.com/Niffy/AndEngine/tree/niffy-AnchorCenter](https://github.com/Niffy/AndEngine/tree/niffy-AnchorCenter "AndEngine Niffy branch")

[https://github.com/Niffy/AndEngine/commits/niffy-AnchorCenter](https://github.com/Niffy/AndEngine/commits/niffy-AnchorCenter "AndEngine Niffy Branch commits")

I have also implemented an isometric view to a popular extension allowing a pseudo 3D (also called 2.5D) view to be made out of 2D sprites.  There is a wiki page describing some of the features implemented as well, these contain some pictures explaining how a feature works or a bug to watch out for. 


[https://github.com/Niffy/AndEngineTMXTiledMapExtension/tree/GLES2-AnchorCenter_isometric](https://github.com/Niffy/AndEngineTMXTiledMapExtension/tree/GLES2-AnchorCenter_isometric "AndEngine Niffy Isometric branch")
[https://github.com/Niffy/AndEngineTMXTiledMapExtension/commits/GLES2-AnchorCenter_isometric](https://github.com/Niffy/AndEngineTMXTiledMapExtension/commits/GLES2-AnchorCenter_isometric "AndEngine Niffy isometric branch commits")
[https://github.com/Niffy/AndEngineTMXTiledMapExtension/wiki](https://github.com/Niffy/AndEngineTMXTiledMapExtension/wiki "Isometric branch wiki page")

The above additions can be demonstrated with the following example code which also includes a wiki on calculating certain values required for moving entities in a game scene.  There is also a YouTube video of a similar example demonstrating my work in action.

[https://github.com/Niffy/IsometricWorldExample/tree/dev](https://github.com/Niffy/IsometricWorldExample/tree/dev "Isometric World Example")

[https://github.com/Niffy/IsometricWorldExample/wiki](https://github.com/Niffy/IsometricWorldExample/wiki "Isometric World Wiki")

[http://www.youtube.com/watch?v=O6AToQHRJw8](http://www.youtube.com/watch?v=O6AToQHRJw8 "You Tube")

What is interesting about my AndEngine work is I had to reimplement Layout Fragments into the engine, the original version of framework had support for Android Fragments, but when the version changed this feature was skipped. Therefore in order for me to use Android native UI with the framework I had to reintroduce it, this can be seen with the following commit. 

[https://github.com/Niffy/AndEngine/commit/116e45655845fa052e13b240bc8bebce8ef257c9](https://github.com/Niffy/AndEngine/commit/116e45655845fa052e13b240bc8bebce8ef257c9 "Andengine Fragment Support")

This feature can be seen in action in the YouTube Video link. The buttons and menus are all native android UI controls overlaid on the framework.

I have also produced a cross platform library which aids me in log file collection from Android devices.  This solution solved the problem of having to collect a log file from multiple devices in a local development environment. I now just have to produce an XML file of devices and details of the log to collect for a windows client. This requires a Windows client to run the collection commands while running an Android service on the devices.  Interestingly I use LOG4J as a logging framework and using Apache Commons CLI library for the windows client. The logs collected can be consumed in `otroslogviewer`, this offers great help in the ability to understand the flow of execution when working in a multi threaded environment and networked applications.


[https://github.com/Niffy/LogForwardLib](https://github.com/Niffy/LogForwardLib "LogForwardLib")

[https://github.com/Niffy/LogForwardClient](https://github.com/Niffy/LogForwardClient "LogForwardClient")

[https://github.com/Niffy/LogForwardAndroid](https://github.com/Niffy/LogForwardAndroid "LogForwardAndroid")


I had created another Java tool to aid in my Android development work.  The tool, called Versioner, is called from an ANT build file to modify a properties file in an Android project, allowing for build and version numbers to increase when required.

[https://github.com/Niffy/Versioner](https://github.com/Niffy/Versioner "Versioner")

I had also started work on a p2p network library, but this was later stopped as Google had released Google Play Game Services. This service allowed networked games with friends and features such as a lobby, it provided the underlying network communication which made this library redundant. I had started to demonstrate the use of Google Play Game Services with Andengine in the IsometricWorld example.  

[https://github.com/Niffy/AndEngineLockStepEngine](https://github.com/Niffy/AndEngineLockStepEngine "LockStepEngine")