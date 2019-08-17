
--- 
knit: "bookdown::render_book"
title: "R 4 Criminology"
author: ["Jacob Kaplan"]
bibliography: [packages.bib]
biblio-style: apalike
link-citations: yes
colorlinks: yes
description: "Notes for learning R for Criminology."
url: "https://r4crim.com"
fontsize: 12pt
github-repo: jacobkap/r4crim
site: bookdown::bookdown_site
documentclass: book
---



# Welcome {-}

These notes introduce the programming language R and are meant for undergrads or graduate students studying criminology. R is a programming language that is well-suited to the type of work frequently done in criminology - taking messy data and turning it into useful information such as cleaning the data, graphing it, or running statistical tests on the data. While R is a useful tool for many fields of study, this book focuses on the skills criminologists should know and uses crime data for the example data sets. 

This book is based off of the lessons I took as a Master's student in criminology at Penn from [Dr. Greg Ridgeway](https://crim.sas.upenn.edu/people/greg-ridgeway). This book covers much of the same material as well as a focus basic philosophy of teaching by example and a focus on the fundamentals of R (and programming in general) as Dr. Ridgeway's lessons. For his lessons, please see [here](https://github.com/gregridgeway/R4crim) .

For this book you should have the latest version of [R](https://cloud.r-project.org/) installed and be running it through [RStudio Desktop (The free version)](https://www.rstudio.com/products/rstudio/download/) . We'll get into what R and RStudio are soon but please have them installed to be able to follow along with each chapter. I highly recommend following along with the code for each lesson and trying to use the lessons learned on a data set you are interested in. To download the data used in this book please see [here](https://github.com/jacobkap/r4crimz/tree/master/data).

## What you will learn {-}

For many of the lessons we will be working through real research questions and working from start to finish as you would on your own project. This involves thinking about what you want to accomplish from the data you have and what steps you need to take to reach that goal. This involves more than just knowing what code to write - it includes figuring out what your data has, whether it can answer the question you're asking, and planning out (without writing any code yet) what you need to do when you start coding. 

### Skills {-}

There is a large range of skills in criminological research - far too large to cover in a single book. Here we will attempt to teach fundamental skills to build a solid foundation for future work. We'll be focusing on the following skills and trying to reinforce our skills with each lesson. 

  * Subsetting - Taking only certain rows or columns from a data set
  * Graphing
  * Regular expressions - Essentially R's "Find and Replace" function for text
  * Getting data from websites (webscraping)
  * Getting data from PDFs
  * Mapping
  * Writing documents through R

### Data {-}

Criminology has a large - and growing - number of data sets publicly available for us to use. In this book we will focus on a few prominent ones including the following:

  * Uniform Crime Report (UCR) - A FBI data set with agency-level crime data for nearly every agency in the United States
  * National Incident-Based Reporting System (NIBRS) - Similar to the UCR, NIBRS is published by the FBI and has agency-level crime data. This data is far more detailed than the UCR which we'll see greatly increases difficulty of use and the rewards from the data
  * Census - The Census surveys people in the United States on a wide variety of variables including demographic, economic, and geographic information. 
  
We'll also cover a number of other data sets such a local police data and government data on alcohol consumption in the United States.

## What you won't learn {-}

This book is not a statistics book so we will not be covering any statistical techniques. Though some data sets we handle are fairly large, this book does not discuss how to deal with Big Data. While the lessons you learn in this book can apply to larger data sets, Big Data (which I tend to define loosely as too large for my computer to handle) requires special skills that are outside the realm of this book. If you do intend to deal with huge data sets I recommend you look at the R package [data.table](https://github.com/Rdatatable/data.table/wiki) which is an excellent resource for it. While we briefly cover mapping, this book will not cover working with geographic data in detail. 

## Simple vs Easy {-}

In the course of this book we will cover things that are very simple. For example, we'll take a data set (think of an Excel file) with crime for nearly every agency in the United States and keep only data from Colorado for a small number of years. We'll then find out how many murders happened in Colorado each year. This is a fairly simple task - it can be expressed in two sentences. You'll find that most of what you do is simple like this - it is quick to talk about what you are doing and the concepts are not complicated. What it isn't is easy. To actually write the R code to do this takes knowing a number of interrelated concepts in R and several lines of code to implement each step. 

While this distinction may seem minor, I think it is important for newer programmers to understand that what they are doing may be simple to talk about but hard to implement. It is easy to feel like a bad programmer because something that can be articulated in 10 seconds may take hours to do. So during times when you are working with R try to keep in mind that even though a project may be simple to articulate, it may be hard to code and that there is often very little correlation between the two.

## How to Contribute {-}

If you have any questions, suggestions, or find any issues please email me at jacob@crimedatatool.com. If this book has helped you, also email me so I can try to measure the book's impact and who is using it. 