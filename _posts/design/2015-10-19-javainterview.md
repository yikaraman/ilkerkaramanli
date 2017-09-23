---
layout: page
subheadline: "Java Interview Questions"
title: "General Questions about Java"
teaser: "Basic Questions about Java Job Interview..."
header:
    image_fullwidth: "java.jpg"
    caption:
    caption_url: ""
image:
    thumb:  java-thumb.jpg
    homepage: business.jpg
categories:
    - Interview
comments: true
sidebar: left
show_meta: true
---

1. What does the “static” keyword mean? Can you override private or static method in Java?
- Static keyword denotes that a member variable or method can be accessed, without instantiation of the class.
- User cannot override static methods in Java, because method overriding based upon dynamic binding at run time and static methods are statically binded at compile time.
- A static method is not associated with any distance of a class so the concept is not applicable.

2. What is Auto-boxing and Unboxing?
- Auto-boxing  is the automatic conversion made by compiler between primitive types and their corresponding object wrapper classes.
               Ex: int to Integer, double to Double
- Unboxing: if conversion goes other way, it is called unboxing
               Ex: Integer to int

3. What are pass by Reference and Pass by Value?
- Pass by Value: this means that a copy of the object is passed.
- Pass By reference: this means that the actual object is not passed, rather a reference of the object is passed.

4. Explain different ways of creating thread. Which one would you prefer and why?
- A class may extends the Thread Class
- A class may implement the Runnable interface, it does not require a object to inherit the thread Class.
- An application can use the Executer Framework, in order to create a thread pool.

5. Thread States in a high-level.
- NEW
- RUNNABLE
- BLOCKED
- WAITING
- TERMINATED

6. What is the difference between Synchronized Block and Synchronized Method?
- each object has a lock. Thread sets object Lock.
- Synchronized Block —> fine grained lock
- Synchronized Method —> coarse Grained lock
