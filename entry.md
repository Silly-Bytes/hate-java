Why do I hate Java
==================


Everything is an object...
--------------------------

... No, it's not!


Not everything is a object. Have you ever read Java code? It's full of actions
dressed like objects: Mutator, Traverser, Factory, Maker, Creator, Generator,
Mediator, Eliminator. So you don't *mutate*, *traverse* or *create* anything,
instead you **force** an **object** that can do that.

Ok, some of that stuff can be useful for *well used* design patterns and a good
design, but most of the time is not!

Don't force objects everywhere. Classes are good when they fit though, and a
good language has OOP as a **feature**.

As Steve Yegge puts it in his article: [Execution in kingdom of nouns](
http://steve-yegge.blogspot.com/2006/03/execution-in-kingdom-of-nouns.html),
verbs should not be second class citizens.

Java stupidity causes lots of [astonishment and improper behaviors that you are
forced to get used to.]( http://www.j-paine.org/objects/objects/objects.html)


S.O.S
-----

Ok, you hit a problem, *javac* is throwing a completely incomprehensible error
and of course you go to Google hoping you get some answers, and you do:

- Click that button
- A pop up widow appears
- Fill up those text fields
- Mark that check box
- Click the yellow icon
- Click "ok"
- Then restart your IDE

> Are you fucking kidding?


The freaking 99% of "solutions" you find are a sequence of clicks and actions in
a graphical user interface of an IDE, What if I'm not using that specific IDE?
What if I'm not using an IDE at all!!?? Are you people stupid? I'm probably not
even in a Xorg server session and writing the code comfortably in my preferred
text editor in a nice tmux or screen session, how I'm I supposed to "click" here
and there? I have no icons!

How is that an error produced because Java can't find a library of something
similar requires a sequence of GUI actions using a mouse? And worse, how is
that the ONLY way to fix it!?

You guys are aware that code is plain text right?... RIGHT??


Use and IDE!
------------

James Gosling (aka Java's father) says: [Don't use
Emacs](http://www.computerworld.com.au/article/207799/don_t_use_emacs_says_java_father/).

Yes, if you're writing Java and you're not using an IDE, but a good text editor
instead, you're going to have some tough moments, but for a good reason.

Java programming gets hard with Vim or Emacs because Java sucks very hard, and
this symptom tells more about the language than it says about de editors.

The language needs and is *dependent* on a huge, bloated and sometimes slow
tailored program to use the language. The IDE becomes a really big support to
hold everything where the language fails.

So the language is not aimed for humans, it requires an extra layer, an
interface (the IDE) for the user to actually use.

More on that in this post: [Why I hate
IDEs](http://silly-bytes.blogspot.com/2016/03/why-do-i-hate-ides.html)


IDE dependent projects
----------------------

If you project use, lets say, Eclipse, the other person will have to use it as
well if she doesn't want to die trying to maintain it in Netbeans for example.
Yes it is possible, but you get headaches too.

Found a nice example in the Internet about something you need? Great! Lets hope
it uses the exact same IDE you use though...

Have you tried to compile an IDE generated project without the IDE? If your not
feeling extremely adventurous or not willing to do it with lots of horrible
hacks, then you better go and install that stupid IDE.

IDE dependent projects is already too bad, but projects that are dependent on
the IDE specific **version**?? Yeah... You might go now and shoot yourself in
the head as well.


Why documentation when you have a mouse?
----------------------------------------

Real documentation is almost inexistent if the IDE has an *automagical* GUI
button for doing that, so if you have to do it, you must use the IDE so you can
press the goddammit button!

Trying to write a SOAP interface for a JSF application? No problem, just click
here and there!. But if you don't use the IDE you're pretty screwed because good
documentation about how to actually **write** the feature, it's stupid or non
existent.

Documentation becomes optional if the IDE has button for doing it.

Automation is good!, but if you **have** to use an IDE to implement a SOAP web
service in a stupid JSF application because there is no other way in which you
don't have to go through a traumatic process, then you are under lots of shit!

Note that I'm using SOAP as example just for the sake of the argument, there are
plenty of other examples, each of those with more or less documentation.


Conclusion
----------

- There are lots of stupid programmers, and Java is on of the things to
[blame](http://www.joelonsoftware.com/articles/ThePerilsofJavaSchools.html).

- If you can't easily write software in a language without an IDE, then the
language sucks.

- Because of the Java dependency on IDEs as (bad programming language
  enablers)[https://dzone.com/articles/ide-bad-programming-language], **lots of
  the problems with Java are just the intersection with IDE's problems.**
