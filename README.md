# Kudryavets Andrey
[LinkedIn profile](https://www.linkedin.com/in/akudryavets)

## Appeal to visitors
Greetings wanderer! 

It seems to me that you entered this site with assessment purposes. Hope that this short description of my projects will save you a little time and will help to find relevant information quickly.


### Tree Optimization Search in Python (2017)
[link to the code](https://github.com/Kudryavets/tree-optimization-search-python/)

This is the attempt to solve [optimizing search problem](https://www.hackerrank.com/contests/quora-haqathon/challenges/ontology) in python 
via trees and recursion. There is a corpus of topics represented hierarchically. Each topic has a number of questions associated with it. In the same time each topic is a generalization of it's children topics and all their questions can be considered as its own questions. The task is to find how many questions among questions of a certain topic match a pattern.

The tested solution is to build a tree of topics with questions tied to nodes. Then traverse a tree recursively to find needed topic
and recursively count matching questions from this topic and it's children. Trees are implemented in Python without using external libraries. All computations are consecutive.

Results of testing are not the best. Solution works pretty fast on 20000 topics / 20000 questions / 20000 queries. 
But 100000 topics / 100000 questions / 100000 queries make one wait for near ten seconds on my laptop. I also found out that python is not 
optimized for tail recursion functions. In several cases of very deep nested trees I have experienced 
`RecursionError: maximum recursion depth exceeded`. Most of the found advices suggest not to use recursion at all or increase recursion limit which is not working for me.


### TF-IDF implementation using Spark with Scala (2017)
[link to the code](https://github.com/Kudryavets/tf-idf-spark-scala)

This is implementation of [TF-IDF algorithm](https://en.wikipedia.org/wiki/Tf%E2%80%93idf) with only RDD API. It aims to show several basic optimizations which can be done in the first place. 

These optimizations are:
* amount of shuffles is reduced to 1
* efficient aggregation introduced for inverted index construction
* all distributed variables are created in memory saving way
* Kryo serialization is used instead of Java serialization


### Interactive heat map app in Scala (2017)
[link to the code](https://github.com/Kudryavets/interactive-heat-map-app-scala)

This application shows interactive visualization of climate data. The app allows to trace the evolution of temperatures and temperature deviations over time in all over the world. 

The project is the Coursera Functional Programming in Scala specialization capstone. This time I was very limited to application architecture designed by instructors. UI in Scala.js was also written by them. Fortunataly they did not develop the whole thing for me ;) So you can see how it actually works. (Soon)


### TSafer (TypeSafer) NLP tool in R (2016)
[link to the code](https://github.com/Kudryavets/typesafer-nlp-r)

[linc to the application](https://kudryavets.shinyapps.io/TSafer/) (Give it time to load please)

This is Natural Language Processing application which tries to predict the next word you want to enter knowing several words you have already entered. You can see a lot of similar applications while using the search or texting sms. 

This one is the Coursera Data Science specialization capstone. Please feel free to play with it. It uses relatively complex mathematical functions and produces quite amusing results from time to time.


