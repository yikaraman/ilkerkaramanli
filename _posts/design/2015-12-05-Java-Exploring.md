---
layout: page
subheadline: "Java keywords "
title: "Exploring java.lang"
teaser: "It is Java’s most widely used package..."
header:
    image_fullwidth: "java_banner_java_se_7_programming-1.png"
    caption: Image by Ticket Synergy
    caption_url: "http://ticketsynergy.com/2015/06/hello-world/"
image:
    thumb:  java-thumb.png
    homepage: java_home.jpg
categories:
    - Reading
comments: true
show_meta: false
---

Void
:  The Void class has one field, TYPE, which holds a reference to the Class object for type void. You do not create instances of this class.

Process
:  The abstract Process class encapsulates a process—that is, an executing program. It is used primarily as a superclass for the type of objects created by exec( ) in the Runtime class, or by start( ) in the ProcessBuilder class.

Runtime
:  The Runtime class encapsulates the run-time environment. You cannot instantiate a Runtime object. However, you can get a reference to the current Runtime object by calling the static method Runtime.getRuntime( ). Once you obtain a reference to the current Runtime object, you can call several methods that control the state and behavior of the Java Virtual Machine.

Memory Management
:   use the totalMemory( ) and freeMemory( ) methods.

ProcessBuilder
:   ProcessBuilder provides another way to start and manage processes (that is, programs). all processes are represented by the Process class, and a process can be started by Runtime.exec( ). ProcessBuilder offers more control over the processes.

ProcessBuilder defines these constructors:

~~~
ProcessBuilder(List<String> args)
ProccessBuilder(String ... args)
~~~

System
:  The System class holds a collection of static methods and variables. The standard input, output, and error output of the Java run time are stored in the in, out, and err variables.

Class
:  Class encapsulates the run-time state of a class or interface. Objects of type Class are created automatically, when classes are loaded. You cannot explicitly declare a Class object. Generally, you obtain a Class object by calling the getClass( ) method defined by Object.

Thread, ThreadGroup, and Runnable
:  The Runnable interface and the Thread and ThreadGroup classes support multithreaded programming.

~~~
Thread( )
Thread(Runnable threadOb)
Thread(Runnable threadOb, String threadName)
Thread(String threadName)
Thread(ThreadGroup groupOb, Runnable threadOb)
Thread(ThreadGroup groupOb, Runnable threadOb, String threadName)
Thread(ThreadGroup groupOb, String threadName)

NOTE: threadOb is an instance of a class that implements the Runnable interface and defines where execution of the thread will begin
~~~

<strong>ThreadGroup</strong> creates a group of threads. It defines these two constructors:

- ThreadGroup(String groupName)
- ThreadGroup(ThreadGroup parentOb, String groupName)

<strong>ThreadLocal and InheritableThreadLocal</strong>
Java defines two additional thread-related classes in java.lang:

- ThreadLocal: Used to create thread local variables. Each thread will have its own copy of a thread local variable.
- InheritableThreadLocal: Creates thread local variables that may be inherited.
