## Website

This is my personal website. This is a fork from [academicpages.github.io](academicpages.github.io).

### Website Prerequisites.

To view this website, you will need [Ruby](https://www.ruby-lang.org/en/) and [Bundle](https://bundler.io). Ruby is an open-source programming language, while Bundle is a tool that takes care of all the dependencies required to run Ruby projects. Below we provide the instructions needed to install these on both Mac OS and Ubuntu.

#### Mac OS

To install Ruby and Bundle on Mac OS, you need to run the following:

```bash
$ brew update
$ brew install ruby
$ sudo gem install bundler
```

**Note**: These instructions have not been tested as I did this setup over a year ago. Please let me know if these instructions do not work.

Next, to install all the dependencies for the website, go into the `Website` folder and run:

```bash
$ bundle install
```

**Note:** For this to work on Mac OS you will need to install xcode. You can install xcode from the app store (it takes a while).

#### Ubuntu

To install Ruby and Bundle on Ubuntu you need to run the following:

```bash
$ sudo apt update
$ sudo apt install ruby-full
$ sudo gem install bundler
```

**Note:** These instructions were tested on Ubuntu 18.04

Next, to install all the dependencies for the website, go into the `Website` folder and run:

```bash
$ bundle install
```

### Viewing the Website

After you have installed everything, you can view the website by running the following in the `website` folder:
```bash
$ bundle exec jekyll serve
```

You can then view the website on:
```
http://127.0.0.1:4000/cs4501/
```