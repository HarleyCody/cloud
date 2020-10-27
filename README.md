Food Truck Finder(FTF)
======================

This file covers  **install dependencies**, **build FTF** and **run FTF**.

install dependecies
---------------------

As FTF is mainly written in Java 12, in order to run it successfully, please install Java12. 

Install from sratch:
```
brew tap AdoptOpenJDK/openjdk
```
Then 
```
brew cask install adoptopenjdk12
```
For making sure the Java12 is installed use command line
```
java --version
```
to see if openjdk 12.0.2 is printed in the terminal

build FTF
---------------------
After Java12 is all set, compile steps kicks in.

Before compiling, please make sure the terminal is at .../FoodTruck/src. Then FTF can be compiled by running:
```
javac FoodTruckFinder.java
```
This steps should not take 10 seconds to finish

run FTF
---------------------
In the final step, FTF can be invoked by command
```
java FoodTruckFinder
```

The welcome message will show up, in the first step, you will be ask to share the time or not. Simply tap "accept" or "refuse" to go to next step. (Case insensitive)

Then if the result is larger than 10, you will be asked to enter "next" to see the next page or "update" to start serach from beginning with current time.

"update" is used when you leave FTF open for so long, and want to get new results. update will reset the date and time for query with current date and time.

If there is no more results, App will exit.
