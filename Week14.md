# Week 14: Open Source phase

This was the last week of the open source phase, it seems incredible to me how people from all over the world are organized in a good enough way to make these projects so interesting and free for everyone who wants to use them. It felt good to contribute to one of these projects, it makes you feel part of something big, where people are there sharing their knowledge, contributing without expecting anything in return except for the project to be successful.

## [Meilisearch-Java Issue #298](https://github.com/meilisearch/meilisearch-java/pull/299 )

The problem in this issue was a variable of type Integer in which the size of the database is saved, there are cases in which the user's database is larger than the one that can store a variable of type Integer so I had to change that variable from Integer to Long. This was the first time I had contact with unit tests, this answered some questions that I had never given myself the task of investigating. How do they work? How is a test done? And what is the purpose of unit testing?

From my point of view, unit tests are to evaluate the behavior of small blocks of code and also in a certain way serve to document what the block of code is expected to do, for example, if someone modifies the code to do something else, the test would fail so another test would have to be done specifically for the new behavior of the code, just as the code itself describes what it does, unit tests in a certain way they describe what they are testing does.

My learnings here were to become familiar with reading other people's code and to locate myself in the project, more than anything it was getting used to moving around so much code without getting overwhelmed or lost, but as time went by it became easier for me.

## [Meilisearch-Java Issue #232](https://github.com/meilisearch/meilisearch-java/pull/305)

In this case it was not to solve a problem but to add new functionality. In this project, documents are an object composed of one or more fields. Each field consists of an attribute associated to a value.

![documento](https://github.com/diegonavarroq/Journal/blob/main/images/documento.png?raw=true)

Here what had to be done was to add two new methods, the first consists of adding the documents in batches of 1000 as default or in batches of the size that the user chooses. The previous way of adding the documents was in a single operation and when the documents were too many, the computer's RAM filled up, which caused the operation to not be completed. The second method is quite similar, but it consists of updating the documents if necessary.

On a more technical level, the documents are in a String with JSON format, so what had to be done was to divide this single String into several and that each of these had either 1000 documents or the amount that the user chose.
What I learned with this issue was an object-oriented programming topic called polymorphism. In this case, I used a feature called overloading that allows you to have several methods with the same name, but the issue here is that the parameters must be different. I use it as follows:

![overloading](https://github.com/diegonavarroq/Journal/blob/main/images/overloading1.png?raw=true)
![overloading1](https://github.com/diegonavarroq/Journal/blob/main/images/overloading2.png?raw=true)

The first method that only has one parameter calls the second method passing it the document parameter and the other two are set by default, but in the event that the user wanted to set them, the second method would be called without the need to call the first.

## [Meilisearch-Java Issue #256](https://github.com/meilisearch/meilisearch-java/issues/256)

This issue, like the previous one, consists of adding functionalities and not solving a particular problem. What this issue tries to implement is to be able to add and update files and also in batches in NDJSON and CSV format in addition to the already available JSON.

The particularity of this issue was to interact directly with the http requests since some headers had to be changed to indicate the type of file that was going to be added or updated.

[INDEX](https://diegonavarroq.github.io/Journal/)
