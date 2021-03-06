---
date: "2019-05-05T00:00:00+01:00"
draft: false
linktitle: ""
menu:
  workshop:
    parent: BasicBasic
    weight: 3
title: BasicBasic 2
toc: true
type: docs
weight: 1
---

# Installing and loading packages

For the second lesson in [Basic Basics](https://rladiessydney.org/courses/workshop/01-basicbasics-0/) we're going to talk about *packages*. You likely won't get very far in R without packages. Sure, you could write all the functions you need for your analysis yourself if you wanted, but the great thing about the [#rstats](https://twitter.com/hashtag/rstats?src=hash) community is that people write code, bundle it into packages, and then give them away FOR FREE because they are so terribly nice. Once you are an #rstats expert, you can create your own packages and give back, but for now let's learn what packages are and how to use them. 

## Lesson Outcomes

By the end of the lesson, you should:

* 2.1 Understand what a package is
* 2.2 Understand how to install packages from the console (quadrant 2).
* 2.3 Be able to use the `library` function to load packages at the top of your script (and understand why it is best to do it there and not in the console!)
* 2.4 Know how to find useful information about how to use a particular package when you are trying something new. 

## 2.1 What is a package?

A package is a bundle of code that a generous person has written, tested, and then given away. Most of the time packages are designed to solve a specific problem, so they to pull together functions related to a particular data science problem (e.g., data wrangling, visualisation, inference). Anyone can write a package, and you can get packages from lots of different places, but for beginners the best thing to do is get packages from CRAN, the *Comprehensive R Archive Network*. It's easier than any of the alternatives, and people tend to wait until their package is stable before submitting it to CRAN, so you're less likely to run into problems. You can find a list of all the packages on CRAN [here](https://cran.r-project.org/). 

Some packages are bundles of packages. For example, the [tidyverse](https://www.tidyverse.org/packages/) is an umbrella package that pulls together lots of individual data wrangling and visualisation packages, so that when you install `tidyverse` you get 8 packages for price of 1 (actually they are free, but you get what I mean). The packages in the tidyverse include: 

  * ggplot2
  * dplyr
  * tidyr
  * readr
  * purrr
  * tibble
  * stringr
  * forcats

## 2.2 How do I install and load packages?

In this screencast, we'll cover:

  * How to install packages
  * How to use the `library` function to load packages when you want to use them 

<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/v6VygIgvoZU?rel=0&modestbranding=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Watch the video and then carry out the following steps:

1. Install the `tidyverse` and `here` packages
2. Add a section label to your script and `library()` calls to the top of your script to load the `tidyverse` and `here` packages. You'll be using these packages to read in data in Basic Basics Lesson 3!  
3. Browse the list of packages on CRAN, find one that looks interesting and install it (just because now you know how!) **Hint** - we will probably use the `janitor` and `skimr` packages soon, so have a go at installing those. 

## 2.3 I've installed a package... now what? 

Installing and loading packages is all well and good - but knowing what they do is pretty important when you want to use them! CRAN requires that package authors write documentation that goes with their package and these documents are designed to give you an idea of what functions are included and what the package can be used for. 

When you are looking for information about a package there are a few places to look. Lets use the `janitor` package as an example...

### Step 1: Look on CRAN 

![](/img/CRAN_janitor.png)

The README file is most often pretty useful. [janitor README](https://cran.r-project.org/web/packages/janitor/readme/README.html)

### Step 2: See if the author wrote a package vignette

A vignette is a long form guide to using the package. For the `janitor` package, there is a link to the vignette in the README file. [janitor vignette](http://sfirke.github.io/janitor/articles/janitor.html)

### Step 3: Google it 

You can see when we google "how to use the janitor package R" the first things that come up are CRAN documentation but under that there are links to documentation and blog posts by other R users who have found the package helpful and written about it. 

![](/img/google_janitor.png)


### Step 4: Have a look on Twitter

Searching twitter is also a great way of locating people who might have written a blog post about how to use a package. Search [#rstats janitor] to find people who have liked the package enough to bother tweeting about it. 

![](/img/twitter_janitor.png)


Now that you have the `tidyverse` and `here` (and a few other potentially useful packages) installed, let's read in some data. 


Now onto [Lesson 3!](/courses/workshop/01-BasicBasics-3/)





