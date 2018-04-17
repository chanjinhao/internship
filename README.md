Internship Project
---

# Overview

We wish to compare different secure programming languages for evaluation. The motivation for doing this is to help us choose an appropriate language for us to adopt to build our programs

There are three 3 phases to this:

0. Setting up the environment
Setup your programming environemnt to allow you to conduct the experiemnt

1. Choosing the languages
We pick a few popular languages that are inherently secure for consideration of this experiment

2. Constructing the artifacts
We will build an FTP using different languages, and use the multiple FTP implementations for comparison.

3. Comparing the artifacts (Bonus Credits)
After building the FTPs in different languages, we compare them to find similarities or differences, and pros and cons

Each of the phases will be explained in detail below

## 0. Setting up the environment
This is set as 0 because it's not really related to the experiement.

We would prefer you to use Linux for development, and some form of version control for your code to be stored. Github is one form of version control, which you are recommended to use. Don't dwell too much time on this part. Get it up and running and get your hands dirty!

## 1. Choosing Languages

Your first phase will be to pick at least 3 languages for comparison. If you can find more, then its perfect, as long as they meet the constrains set below.

The language choice must be actively maintained, and "popular". "Popular" isnt concretely defined, and a metric now is how many stars it has on github/gitlab. See [Rust](https://github.com/rust-lang/rust) for an example of an "popular" program.

It also has to be actively maintained because we want a language that survives, as the language chosen will be used in the long run.

Languages that you should not pick:
1. C (we're already using C, so omit this in your language choice)
2. Java (No)

A few ideas for languages are:
1. Rust
2. nim

## 2. Constructing the Artifacts

After choosing your languages, its time to build your program.

We have chosen to build an FTP server due to its high complexity and programmatic entropy, yet straight forward to implement. We need this entropy to allow variance in the comparison later

If you can think of more complicated programs to implement, feel free to suggest it to us! (SSH server? Or the AES algorithm if you're crazy enough)

When building the various FTP servers in different languages, ensure that they all have the same functionalites for a fair comparison

Suggested functions are:
1. User Authentication
2. File Upload
3. File Download
4. Permission Checking

Do add in additional features you see fit. Remember, the features must be common across all the FTP servers (i.e. don't implement something that can only be done in one language, but not the rest)

### 2.1 Easter egg planting!

While you are constructing your program, we would like you guys to plant some easter eggs into them! Hidden functions that will be called under very abnormal and obscure circumstances (e.g. failing authentication 42 times will throw log you in automatically)

This sets up work for the next intern, who will be doing malware analysis and reverse engineering to find the easter eggs.

## 3. Comparing the Artifacts (Bonus Credits)

If you've made it this far, congratulations! Its no easy feat for the tasks above in such a short period of time.

Now that we have the programs built up, we need to start comparing them.

We'll compare the programs using Static Analysis. An exmaple program to do this is `bindiff` which finds out similarities between the programs.

This area of work touches a the tip of the iceberg of reverse engineering, which you are welcome to read into!
