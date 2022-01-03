# Week 12 phase: Open Source

### Welcome to my third phase of open source.

After the third open source week, I was able to contribute my second pull request to the meilisearch project, it was accepted and it was joined to the rest of the project code. I am currently working on an issue that includes several pull requests, this consists of adding new methods so that it is possible to add documents not only from json files, but also from csv and ndjson files (newline delimited json). This issue includes implementing the solution that I contributed in the last issue which is to batch upload documents from a json file but now apply that with csv and ndjson files.

## Bors

I noticed the existence of Bors until I made my second pull request to this repository, Bors is a GitHub tool, when making a pull request apart from the code being reviewed by the project maintainers it also has to pass the tests, so what does bors do it is a merge with the main code in a waiting area where you can run the tests before actually merging main, after all the tests have passed and the maintainers have given it the go-ahead now if it is possible to do the merge.

## Linters

Linter is a tool that analyzes the code without having to execute it, in order to improve or correct it as the case may be within these four categories: programming errors, bugs and performance improvements, code standardization and security. In the case of this project, linter is used to follow a certain code format, I was struggling because the IntelliJ IDE that I am using has a tool that is used to optimize imports which accommodated them in a certain way in the code that was not approved by linter which when making the pull request and the bors running the tests did not allow it to be joined with the main code. To solve the problem I only had to deactivate the IntelliJ tool, the problem was quite simple, but it did take me some time to know what was happening.

## Http

This new issue I am working on consists of submitting new file types, which leads me to directly modify some of the http methods. I already knew some http methods from having used them in the previous phase such as POST and GET. This issue led me to investigate the rest of the methods, to know what they are and what each one of them does. Those used in this project are the following:

- GET: This method sends the information in the URL itself, the information is always visible so you should never send sensitive information through this method.
- POST: This sends data through the body and nothing through the URL, the request body type is defined in the Content-Type header.
- PUT: It is similar to the POST method, but in this case insert if it does not exist and if it already exists it replaces, if we execute PUT several times it would be like having executed it only one.
- DELETE: This method is to eliminate a specific resource, it can be executed n times and will have the same result as in the case of the PUT.

## Newline Delimited JSON or ndjson

It consists of a text-based format in which each individual line is a valid JSON-type text.

### JSON file example:
![JSON](https://github.com/diegonavarroq/Journal/blob/main/images/JSON.png?raw=true)

### NDJSON file example:
![NDJSON](https://github.com/diegonavarroq/Journal/blob/main/images/NDJSON.png?raw=true)

### Also a CSV file example:
![CSV](https://github.com/diegonavarroq/Journal/blob/main/images/CSV2.png?raw=true)


[INDEX](https://diegonavarroq.github.io/Journal/)
