# Kudryavets Andrey

## Appeal to visitors
Greetings wanderer! 

It seems to me that you entered this site with assessment purposes. Hope that this short description of my projects will save you a little time and will help to find relevant information quickly.


### TF-IDF implementation using Spark with Scala 
[link to code](https://github.com/Kudryavets/tf-idf-spark-scala)

This is implementation of [TF-IDF algorithm](https://en.wikipedia.org/wiki/Tf%E2%80%93idf) with only RDD API. It aims to show several basic optimizations which can be done in the first place. 

These optimizations are:
* amount of shuffles is reduced to 1
* efficient aggregation introduced for inverted index construction
* all distributed variables are created in memory saving way
* Kryo serialization is used instead of Java serialization


### Interactive heat map app in Scala
[link to code](https://github.com/Kudryavets/interactive-heat-map-app-scala)

This application shows interactive visualization of climate data. The app allows to trace the evolution of temperatures and temperature deviations over time in all over the world. 

The project is Coursera Functional Programming in Scala Capstone. Thus I was limited to application architecture designed by instructors. UI in Scala.js was also written by them. Fortunataly they did not write the whole thing for me;)

Here you can see how it actually works. (Soon)


###
