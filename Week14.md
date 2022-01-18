# Week 13: Open Source phase

This was the last week of the open source phase, it seems incredible to me how people from all over the world are organized in a good enough way to make these projects so interesting and free for everyone who wants to use them. It felt good to contribute to one of these projects, it makes you feel part of something big, where people are there sharing their knowledge, contributing without expecting anything in return except for the project to be successful.

## [Meilisearch-Java Issue #298](https://github.com/meilisearch/meilisearch-java/pull/299 )

The problem in this issue was a variable of type Integer in which the size of the database is saved, there are cases in which the user's database is larger than the one that can store a variable of type Integer so I had to change that variable from Integer to Long. This was the first time I had contact with unit tests, this answered some questions that I had never given myself the task of investigating. How do they work? How is a test done? And what is the purpose of unit testing?

From my point of view, unit tests are to evaluate the behavior of small blocks of code and also in a certain way serve to document what the block of code is expected to do, for example, if someone modifies the code to do something else, the test would fail so another test would have to be done specifically for the new behavior of the code, just as the code itself describes what it does, unit tests in a certain way they describe what they are testing does.

[INDEX](https://diegonavarroq.github.io/Journal/)
