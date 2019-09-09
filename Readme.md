[![Build Status](https://travis-ci.org/Shenaida/eventweek-solitair-student.svg?branch=group_version)](https://travis-ci.org/Shenaida/eventweek-solitair-student)

# Solitaire / Patience
##### Software Engineering Event Week With Quintor

--- 

Welcome to the Event Week! In this project you will program your own game of Solitaire / Patience. If you are unfamiliar 
with the rules of the game, you can take a look at one of these sites:
 - [patiencespel.nl](http://www.patiencespel.nl/patiencespelregels.php) (Dutch)
 - [digsolitaire.com](http://digsolitaire.com/solitaire-rules.php) (English)

It really helps to play a few games of Solitaire / Patience so that you are really comfortable with the rules. Although 
the game is
easy to understand, you will find that programming the game logic can be quite challenging if you don't have a really 
thorough understanding of the rules. There are a lot of Solitaire / Patience games that you can use to 
get up to speed, both online and offline.

##### The assignment
This week will introduce a lot of new concepts to you. You will develop as a team, perhaps for the first time. 
You will report to a Product Owner. Your software has to be of high quality, but you're under pressure to deliver as 
many features as possible as well. These are just a few of the programming concepts you will encounter:

 - [Lists](https://docs.oracle.com/javase/8/docs/api/java/util/List.html), 
   [Maps](https://docs.oracle.com/javase/8/docs/api/java/util/Map.html) and other Java 
   [Collections](https://docs.oracle.com/javase/8/docs/api/java/util/Collection.html), which are really helpful in 
   managing groups of things, like cards :)
 - You will encounter [enums](https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html), 
   [classes](https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html) and 
   [objects](https://docs.oracle.com/javase/tutorial/java/javaOO/objects.html) (you don't have to design them)
 - You will implement [Interfaces](https://docs.oracle.com/javase/tutorial/java/concepts/interface.html), 
   which are a kind of blueprints for classes (which is why you don't have to design them).

If all of this is new for you, don't worry. We've left you examples, documentation so you know what everything does / 
is supposed to do. And we are there to help you of course.

As a team, you will try and implement a game of Solitaire. While it is a relatively simple game, quite a lot of different 
features can be identified. A [backlog](backlog.md) of such features has been created for you. It is split into two categories. 
The first category consists of "MVP"-features. MVP means Minimal Viable Product, and this set of features is what you 
have to implement at minimum to launch your software (to "go live"). **You have to implement the MVP at minimum to pass the 
project.**

The second set of features consists of optional features. You get **bonus points for implementing optional features**,
but you don't have to. However, the **best version of the game will win a prize**. You might try and rush as many
features as possible into your implementation, but keep an eye on the quality of your work: **bugs & stacktraces will count
against you**.

All features have been assigned a number of points. **These points indicate our estimation of the relative difficulty 
and/or time commitment of implementing that feature.** You, as a team including your Product Owner, will decide what 
features you are going to pursue. We hope you will really enjoy yourself and get a test of what real software engineering
is all about, as you push hard towards your 1.0 release!!!

---  

##### What do you need to get going?
You can work in both Windows and Linux. MacOS will most likely work just fine as well, but hasn't been tested.

 - Git: included in most Linux distributions, downloadable for Windows [here](https://git-scm.com/download/win).
 - Maven: inluded in NetBeans, Eclipse and IntelliJ IDEA or downloadable [here](https://maven.apache.org/download.cgi).
 - Java 8 (or higher) SDK: OpenJDK included in most Linux distributions, Oracle Java downloadable for Windows 
   [here](http://www.oracle.com/technetwork/java/javase/downloads/jdk9-downloads-3848520.html).

##### Clone & open the project
You can either:
 - Clone the project from Git and open it in your favorite IDE (assuming git(.exe) is on your PATH):
 
   ```
   git clone GIT_URL
   ```
 - Import the project in your favorite IDE from Git directly.

##### Building & running
To build & run the project, you need to use the Maven tool. Maven is a Java build tool that can 
do Many Important Things. What it does for you is build this software with all required dependencies, so 
that you can focus on your code.

This is something you probably heard before, and then you spent hours scouring obscure corners of the 
internet to get the stupid tool to work, while salty tears start to shortcircuit your keyboard and 
existential questions about your life choices pop up into your head.

Not this time! Most IDE's (including NetBeans, IntelliJ IDEA and Eclipse) include Maven out of the box. 
All you need to do is import or open this project (as a Maven project) and everything will be taken care
of. You can simply run nl.quintor.solitaire.Main from the IDE to start the application.

If you are feeling adventurous and/or self-loathing and don't want to use an IDE, you can install Maven 
yourself from the download link above. You can then build and run the application using:
```
mvn compile exec:java -DskipTests=true
``` 
from the project root folder (assuming mvn(.exe) is on your PATH).

##### Documentation

The project is documented using JavaDoc in the source code itself. You may be familiar
with it from the Java [API](https://docs.oracle.com/javase/8/docs/api/). JavaDoc is a special comment format. Because 
reading comments in code is at best inconvenient and at worst really awful, JavaDocs can be magically transformed into 
readable, clickable websites. In order to become a good Java programmer, it is really important that you learn to find 
your way around such documentation. That's why you can generate these JavaDocs using:
```
mvn javadoc:javadoc
```
from the project root folder (assuming mvn(.exe) is on your PATH). The docs will be generated in the folder "apidocs" 
in the project root, you can view them by opening apidocs/index.html in any browser.

##### Tests

The project contains methods you need to implement. You can run the tests from your IDE or with Maven:
```
mvn clean:test
```
You can find all the tests in the "src/test/java" directory.
After checking out the project most of the tests will fail. Start writing implementations for the test methods with 
the name ending in "DoesNotThrowNotImplementedException".
