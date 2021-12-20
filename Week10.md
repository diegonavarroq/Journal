# Week 10 - Phase: Open Source

This week we started with the third phase of the apprentice which consists of contributing to an open source project, and I chose one called meilisearch which consists of a fairly fast search engine. It is a library that is supported for several languages, but I started contributing in java. I solved an issue that was quite easy to solve, I made the pull request and it was accepted to merge with the base code. This next week I will try to solve a bigger issue and maybe even make a pull request before Christmas.

Starting to read other people's code is a very important skill since when entering a new team the first thing you have to do is understand the code that is already written to start writing yours. And I suppose that this skill is the one that you want to develop with this phase, which would suit me very well because I don't have much experience reading other people's code.

## Cypress

But this week it was not only about the open source phase, I also saw with my mentor a framework called Cypress, this works to do functional testing of the frontend by automating actions in the browser that will interact with a web application. I found the structure of the tests in the code and the reserved words used to be quite intuitive.

## Gradle

The open source project uses a tool called Gradle that helps with the automation process in compiling the code. It also manages the dependencies within the project, which caused me some problems when I was setting up the environment because it didn't want to download some dependencies, which wouldn't let me run the project. And since at first I did not understand how Gradle works, I thought it was gradle, but working with my mentor we came to the result that it was the antivirus on my computer and not gradle itself.

## Sdkman

Another tool I use is Sdkman this works to install and manage various versions of SDK such as Java and Gradle. This helped me to verify that the error I described above was not due to incompatibility of the Gradle and Java versions that I was handling. It is also much easier and more practical to download, install and select which version of the SDK you want to use.

## Testing

After making the change to the code, a series of tests must be carried out to see that everything works well and then the Pull Request can be accepted. What I did was change a variable type from Integer to Long, the code did not pass the test because its input had to be Integer, so I also had to modify the test to read the test values correctly.
