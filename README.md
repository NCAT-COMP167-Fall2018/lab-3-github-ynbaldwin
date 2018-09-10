# Introduction to GitHub

Today, we will use git and GitHub to make improvements to an existing application. These improvements will improve code readability and program performance. Each improvement will be made on a separate branch and sumitted via a pull request.

## Clone and Open the Project

For this lab, a project already exists. This simulates working on a project at your job, where the code base will likely already exist. Clone this repository and open the NetBeans project called PersonalTwitterFeed. This project is a local, self-hosted, command line Twitter feed. Since so many people get upset when seeing opinions different from their own on Twitter, and so many people actively use Twitter to leverage hate and anger against users generally minding their own business, we are developing a Twitter experience fit for today's social culture. In our instance, users see a timeline of _only_ their own tweets, no disagreements and no one for trolls to target!

## Feature 1 - Timestamped Tweets - 2 points

Now that you have downloaded the project, its time to start making upgrades! The first assignment you've received is to add a feature that will timestamp each tweet as it is entered. 

* _First_, we must make a branch for us to work on. Because this code already exists, it would be very poor practice to simply add code on top of the **master** branch unilaterally. Lets create a branch called **feature-1** that will hold all of our code for this feature.
  * On the command line, enter `git checkout -b feature-1` to create this branch.
  * Make sure you are within the GitHub-Lab-2 repository to run this command.

* To implement this, should should write a method called `getCurrentTimeStamp()` that returns a `String` representation of the current time.

* Add the current timestamp to the end of each Tweet as it is created.

* Check out [this tutorial](http://tutorials.jenkov.com/java-internationalization/simpledateformat.html) to get an introduction to Java's `SimpleDateFormat`, which will be useful for this feature.

* Once you have completed this feature, make sure you run the following commands to commit and push this code:
  ```
  git add .
  git commit -m "Your commit message here"
  git push
  ```

* Then, look at your repository on GitHub's website. Click on the "Pull Requests" tab and then "New pull request".

* Your **base** branch is the branch that will _receive_ data, the **compare** branch should be the _new_ code to be added.

* Make sure to add all of your TA's as a reviewer to receive credit!

## Feature 2 - Make a `newTweet()` method - 2 points

Our main method is large, and can be difficult to follow. We are going to break up some operations into separate methods to make it easier to read.

* First, we _must_ create our new branch to work on feature 2! This work is going to _build on_ our work done in feature 1, so we should have **feature-1** as our active branch when we create **feature-2**. Remember the command from above to create a new feature branch.

* Now, create a new method called `newTweet()` that will handle accepting input from the user and adding a new tweet to the array called `tweets`. This means you will have to pass the array `tweets` as an argument to `newTweet()`.

* Remove the code from the `main()` method that handles creating a new tweet, and replace it with a call to `newTweet()`.

* Commit, push, and open a new pull request for this feature.

## Feature 3 - 
