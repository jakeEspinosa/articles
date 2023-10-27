If you’ve been programming for more than a few months, you’ve likely heard of git. Git is a distributed version control system that lets you manage your code and easily collaborate with others. Git is relatively simple to learn, but the workflow used in enterprise environments may be foreign to aspiring developers. In this article, I will explain the basic enterprise workflow and some standard best practices to go along with it.

## Basic Workflow
When you get to your first job, the team will likely have an existent code base. This article will not cover initial setup and cloning repos, but go here if you need a refresher. After you get all of the repos cloned to your machine, you will likely be following this general workflow:

1. Create and checkout a branch to isolate your commits
2. Submit a merge/pull request to the remote branch (NOT main) to save your work 
3. Write your code and commit your changes
4. Review your commits with a linting tool, security tool, your eyes, etc
5. Request a code review before merging your branch into main

### Branching
You should _always_ create a new branch for any bug fixes/features you implement. Doing so will isolate your changes and make reviewing (and hopefully accepting!) easier. _Don’t_ be the person who tries to push their changes to directly to main.

### Submit A Merge/Pull Request _Before_ You Write Any Code
This is a best practice for keeping your commits if your hard drive crashes, your computer dies, etc. It also allows others to review your code as you go along. Even though you submit a merge/pull request, you can still make commits and push to your remote branch until it is approved or rejected. Again, push your code to your _branch_, not to main.

### Commit Code
This is the most crucial step. Make time to review your company’s style guide and implement it. If your company doesn’t have a style guide, read existing code and match the style (and perhaps create a style guide). Your code should be as concise and readable as possible. Remember, we write code for other programmers first and the machine second.

Commit messages, like code, should be concise and descriptive. I recommend [this article](https://initialcommit.com/blog/git-commit-messages-best-practices) for some best practices for crafting commit messages.

### Review Your Code
Your company should have a style guide and linter that enforces the style guide. Make sure to learn how to use it and do so before asking another developer for review. Your company also should have a security scanning solution (I shudder at the thought of all the companies who don’t…). Make a habit of running these scans before requesting review. 

### Final Code Review Before Merging into Main
Many developers loathe code reviews. They may take criticism personally, become defensive, or completely ignore what their fellow developer has to say. However, it doesn’t have to be this way.

Everyone has experiences, skills, and knowledge that form who they are as a person. Therefore, everyone will view things differently and see things in a way you never thought possible. Without getting too philosophical, you should look forward to code reviews to learn from your reviewer and develop your critical eye. Take note of their suggestions, evaluate them, and implement them if it makes sense (or if you are required to for approval).

Lastly, but most importantly, remember that you are not your code. Any criticism or suggestions to improve your code should be taken as alternative analyses of what you wrote instead of as personal attacks on your skills or you as a person. Remember, the company owns the code and hires us to write it in the best way possible.

## Summary
The enterprise git workflow may be jarring to junior developers, but it is critical to effective collaboration and engineering. The basic workflow is creating and checking out your branch, submitting a pull/merge request, writing and committing changes, reviewing your code for quality on your own, and then reviewing your code with a peer before merging to main. Not every company will follow this exactly, but this basic process will form the foundation of what you will be expected to do on the job.
