# QBS 101.5: Data Wrangling

Data processing of any kind (statistical analysis, machine learning, visualizations, ...) requires neatly and consistently structured data. In published dataset, much work has usually been done to make sure that all data points adhere to a common format and structure so that whatever processing we plan on doing can start right away.

Often, however, and especially when we collect our own data, the datapoints can be a bit of a mess: Maybe we tapped different sources, which delivered data in different formats. Maybe some of our data points are incomplete. Maybe we have to convert some of our data to be able to process it. In a word: our data is dirty!

In this session, we will look at some selected techniques to deal with Dirty Data in a systematic and effective way.

<img style="float: right; margin:5px 0px 0px 10px" src="Images/IMG-lego-logo.svg" alt="Lego-Logo" height="128" width="128">

The example data we will be handling are various facts and figures about Lego sets. It was collected by scraping the public product descriptions of www.lego.com. If you are interested in how you can collect data in this way, look out for our workshop on "Scraping and using web APIs with Python"!

In the course of this notebook, we will consolidate the data from two very different files, analyze its structure and format, clean up incomplete entries, and store the clean dataset for later use. This process is often called **Data Wrangling** or **Data Munging**.

### What you will learn in this session
- Importing data from inconsistent sources
- Cleaning up inconsistent or inconveniently formatted entries
- Dealing with missing values

We will use the Python data analysis and manipulation package [pandas](https://pandas.pydata.org/), but the presented strategies can be applied in any programming language and framework.