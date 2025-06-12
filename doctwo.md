# What is R?

> This page will provide new R programmers with an overview of R programming and how to transform their R code into a [Shiny App](glossary.md#glossary). 

### RStudio 

[RStudio](glossary.md#glossary) is the integrated development environment (IDE) that runs R. It contains the console to run the code, and a text editor to edit the code. RStudio is very similar to a word processor, such as Google Docs or Microsoft Word,  where you write and print the document. In R, you write your code and instead of printing you run the code. 

### R 

R is a programming language primarily used for data analysis, statistics and data visualization. The language is designed to be simple to read and learn. The language has a variety of different tools used for analysis such as graphing and calculating functions. Additional packages containing [libraries](glossary.md#glossary) can be loaded into the code and provide an even bigger tool box. R code can be published into websites called Shiny Apps.

### Shiny Apps 
#### Set Up 

Shiny is a [package](glossary.md#glossary) that can be loaded into R to build apps. To install the package, run: 

        install.packages("shiny")

This will take some time, but will install shiny on your device and you will not need to run this [command](glossary.md#glossary) again. To use the shiny features you will need to include: 
  
        library(shiny)

This will need to be at the beginning of your R code to access the different libraries. The word “shiny” can be replaced in this code to access any library.

#### Components 
[Shiny Apps](glossary.md#glossary) create three components, a user interface (UI) object, a server function, and an app function. You will not need to create these items, but you should understand how they work. 


##### UI Components 
The UI Component is responsible for creating the page setup. This document essentially contains all of the components of the app. Creates the tabs, titles and headings, and calls the content on each page as functions. 

##### Server
The server hosts the App. The content in the server provides the input and output to each page.

##### App Component 
The app component is very simple. This file provides the sources for each page, referring the file paths and provides the shiny app with the ui and server. An example of this could look like: 

        #List source files to provide functions 
        source("compare_bands.R")
        
        #Load UI and server variables 
        shinyApp(ui = ui, server = server)

