# Week 13: Open Source phase

This week I managed to complete the third pull request, although this pull request only solves half of the issue that consists of two parts, the first is to add the necessary methods to add documents that come in CSV and NDJSON formats that documents can be added in one operation or in batches. The pull request has not yet been reviewed, but in my opinion it looks good for the unit tests and the bors tests that are applied automatically when making a pull request.

The problem here was to send the correct headers depending on the type of file that was being sent, if it is CSV the following Content-Type has to be sent: text / csv, NDJSON, Content-Type: application / x-ndjson and if it is JSON, Content-Type: application / json. Here what took me the most time was to find where the headers set was made, since in some methods empty maps were sent where they gave you to understand that the set could be made there, but in reality they were hardcoded where they were towards the request.

Once that was changed, it was now possible to make new methods from where each one would send its header depending on the type of file to be uploaded.

### Enum

It is a special class that represents a group of constants, in this case those constants were the http verbs that were used in the different methods of the project. To avoid committing a typo, they called this class with the verbs inside.




[Index](https://diegonavarroq.github.io/Journal)
