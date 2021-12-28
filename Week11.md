# Week 11 - Open Source 27/12/2021

### Welcome to my second phase of open source.

The second week of the open source phase was a bit more complicated than the first, due to some unusual situations, firstly, it was Christmas Eve and Christmas this week and even if you want to continue working sometimes you can't, because with the whole family here in the house there are too many distractions, secondly, the interview that in theory should not be very complicated, but since it is my first interview it is almost impossible to stop thinking about it when you are trying to do the other assignments of the phase, they were between internal blockers and non-blockers this week.

This week I dedicated myself to solving another issue of Meilisearch definitely more complex than the previous one, this consisted of adding two new functionalities, “addDocumentsInBatches” and “updateDocumentsInBatches”, they consist of having the option to add and update documents in the Meilisearch database , in batches of the size that the user decides. Before there was only the option of uploading all the documents in a single operation, when they were sets of very large documents it filled all the RAM memory of the computer and the process could not be completed.

What took me the most time was to fully understand the requirements of the new functionality, since I got confused with a previous PR that another person had made that was rejected, but it was not very clear why and that's when I started to interpret what it is what they really wanted. I learned how to read someone else's code and how to follow the guidelines established in this project.

The guidelines of this project say that before each PR a unit test must be done for the code block that you just added or modified, unlike the last issue that I only had to modify an existing test, in this one I had to create one since I added a new method to the code.
