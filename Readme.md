# Eartrainer
This project is being created as a programming project in Informatics class with Ms Vazquez in January 2018.


[Installation](#install)

  


## The Idea
A game based on the game of [set](https://en.wikipedia.org/wiki/Set_(game) "Wikipedia").

However, we do not want to create a clone of this game but rather convert it into something new.
Our idea is to use this notion of a set and apply it to music. 
Instead of having a 3x3 grid where one has to find a set, we will use a simpler version of the game.
In this version two 'cards' already lie on the table. By the rules of set, the third card is clearly determined.

In our version of the game the visual features of color, number, symbol and shading are replaced by auditive features.
These auditive features are:

[//]: # (@TODO: Fill in the gaps here.)

 - Interval size (Out of a predetermined list of three)
 - ...


## Setup
### Git and Github
Git is 'the' version management tool out there. It makes version management a breeze. Github makes distributed working easy.
To get an overview over this tool checkout:
 - [My Bash and Git Cheatsheet](https://github.com/stymphalide/git_bash_cheatsheet/blob/master/cheatsheet.md "git and bash cheatsheet")
 - [A really good git tutorial](http://gitimmersion.com/ "gitimmersion") (I really recommend checking this out)
 - [An introduction to Github's markdown](https://guides.github.com/features/mastering-markdown/ "mastering-markdown") (This file is written in this markdown.)
 - [A Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Markdown Cheatsheet")
 - [A Markdown Editor](https://jbt.github.io/markdown-editor/ "markdown editor")

Note: Since Windows and Linux handles line endings differently there has to be some set up in a .gitattributes file. (Also because of gradle)
[Dealing with line endings](https://help.github.com/articles/dealing-with-line-endings/)

### Gradle
A Build tool for our application. Takes the task of compiling the code and running tests away from us. Can also be used to create a `.jar` file. It also sets up a basic project, and most importantly can be used as a plugin in eclipse. This way we can make sure, that the setup of our application 'fits' for the IDE but can still be developed outside.
 - [Gradle Build Tool](https://gradle.org/ "gradle build tool") with tutorials on how to use it
 - [Eclipse Plugin Installation guide](http://www.vogella.com/tutorials/EclipseGradle/article.html "gradle plugin for eclipe") Remark: Make sure to install `gradle 4.4.1` or the corresponding version I don't know if there can be conflicts if we use different versions (Though I doubt that.)
 - [Github source code](https://github.com/gradle/gradle "gradle")
 - [Add dependencies](https://stackoverflow.com/questions/20700053/how-to-add-local-jar-file-dependency-to-build-gradle-file "gradle dependency stackoverflow")

### Testing
 - [JUnit on Github](https://github.com/junit-team/junit4 "source code") 
 - [Getting started with junit](https://github.com/junit-team/junit4/wiki/Getting-started "getting started with junit")
 - [junit dcoumentation](http://junit.org/junit4/javadoc/latest/ "junit documentation") (Don't get eye cancer!)
 - [Why Testing?](https://www.quora.com/Why-is-testing-code-important "why testing is important") (Note we are probably only going to do 	the first category of tests that he describes.)
 - [TDD](https://www.agilealliance.org/glossary/tdd/ "tdd") would be nice if we could actually implement some parts of the test-driven paradigm. (Note that under time pressure this is not going to work.)

### Front End
After the 'coding part' and the testing part we should decide on which libraries to use to accomplish out task. One thing that needs to be covered is the how to make the Graphical User Interface (Something that I consider highly overrated!!!). We are going to use Java's go-to tool, namely javafx
 - [JavaFx API](https://docs.oracle.com/javase/8/javafx/api/toc.htm "JavaFX API") (Don't get eye cancer here!!!)
 - [JavaFX Tutorial](http://code.makery.ch/library/javafx-8-tutorial/ "JavaFX Tutorial")
 - [Use JavaFX's WebView](https://docs.oracle.com/javafx/2/webview/jfxpub-webview.htm "JavaFX WebView") Could be used to just use html5 and css3 as well as js? to render the view. (This approach could be considered cheating)

### Further Libraries
Since we are going to produce sound in one way or another it is necessary to check out some midi/sound libraries for Java.

Java ships with some integrated libraries to accomplish these tasks:
 - `javax.sound.sampled`
 - `javax.sound.midi`

A higher level library could be jFugue:
 - [jFugueGithub](https://github.com/dmkoelle/jfugue "jfugue/github")
 - [jFugue](http://www.jfugue.org/ "jFugue") A high level midi parser, that take care of most of the dirty details, works out of the box.(?)
 - [Some basic examples](http://www.jfugue.org/examples.html "jfugue examples")
 - [jFugue API](http://www.jfugue.org/doc/index.html "jFugue API")

### License
To be determined

[//]: # (@TODO: License that important??)

### Time Schedule
List of important dates.

[//]: # (@TODO: Fill in the gaps here.)


### Project Structure
Make a tree of the project structure.

[//]: # (@TODO: Fill in the gaps here.)


## Download

Download an exectuable .jar archive [here](somerepository "exectuable")

[//]: # (@TODO: Create a repository where an executable .jar file will be placed. I have done some research that .exe file is not likely to work. byAB)

Or clone this repository

	git clone https://github.com/stymphalide/eartrainer.git


## Install

### Prerequisites
You need to have gradle installed:
[Gradle Build Tool](https://gradle.org/ "gradle build tool")

After the installation of gradle run in a command line

	cd eartrainer
	gradle build
	gradle run