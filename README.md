# Project Description

You've made it all the way through the first phase of being a Data Scientist - take a minute to celebrate your awesomeness!

![awesome](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-1-project-v2-4/master/awesome.gif)

Now you will put your new skills to use with a large end-of-Phase project!

In this project description, we will cover:

* [***Project Overview:***](#project-overview) the project goal, audience, and dataset
* [***Deliverables:***](#deliverables) the specific items you are required to produce for this project
* [***Grading:***](#grading) how your project will be scored

## Project Overview

For this project, you will use exploratory data analysis to generate insights for a business stakeholder.

### Business Problem

Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.

### The Data

In the folder `zippedData` are movie datasets from:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

Because it was collected from various locations, the different files have different formats. Some are compressed CSV (comma-separated values) or TSV (tab-separated values) files that can be opened using spreadsheet software or `pd.read_csv`, while the data from IMDB is located in a SQLite database.

![movie data erd](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-1-project-v2-4/master/movie_data_erd.jpeg)

Note that the above diagram shows ONLY the IMDB data. You will need to look carefully at the features to figure out how the IMDB data relates to the other provided data files.

It is up to you to decide what data from this to use and how to use it. If you want to make this more challenging, you can scrape websites or make API calls to get additional data. If you are feeling overwhelmed or behind, we recommend you use only the following data files:

* `im.db.zip`
  * Zipped SQLite database (you will need to unzip then query using SQLite)
  * `movie_basics` and `movie_ratings` tables are most relevant
* `bom.movie_gross.csv.gz`
  * Compressed CSV file (you can open without expanding the file using `pd.read_csv`)

### Key Points

* **Your analysis should yield three concrete business recommendations.** The ultimate purpose of exploratory analysis is not just to learn about the data, but to help an organization perform better. Explicitly relate your findings to business needs by recommending actions that you think the business (Microsoft) should take.

* **Communicating about your work well is extremely important.** Your ability to provide value to an organization - or to land a job there - is directly reliant on your ability to communicate with them about what you have done and why it is valuable. Create a storyline your audience (the head of Microsoft's new movie studio) can follow by walking them through the steps of your process, highlighting the most important points and skipping over the rest.

* **Use plenty of visualizations.** Visualizations are invaluable for exploring your data and making your findings accessible to a non-technical audience. Spotlight visuals in your presentation, but only ones that relate directly to your recommendations. Simple visuals are usually best (e.g. bar charts and line graphs), and don't forget to format them well (e.g. labels, titles).

## Deliverables

There is only one deliverable for this project:

* A **Jupyter Notebook**

### Jupyter Notebook

The Jupyter Notebook is a notebook that uses Python and Markdown to present your analysis to a data science audience.

* ***Python and Markdown*** means that you need to construct an integrated `.ipynb` file with Markdown (headings, paragraphs, links, lists, etc.) and Python code to create a well-organized, skim-able document.
  * The notebook kernel should be restarted and all cells run before submission, to ensure that all code is runnable in order.
  * Markdown should be used to frame the project with a clear introduction and conclusion, as well as introducing each of the required elements.
* ***Data science audience*** means that you can assume basic data science proficiency in the person reading your notebook. This differs from the non-technical presentation.

Along with the presentation, the notebook also describes the project ***goals, data, methods, and results***. It must include at least ***three visualizations*** which correspond to ***three business recommendations***.

You will submit the notebook in PDF format.

The graded elements for the Jupyter Notebook are:

* Business Understanding
* Data Understanding
* Data Preparation
* Data Analysis
* Visualization

## Grading

The project rubric objectives are:

1. Attention to Detail
2. Data Communication
3. Authoring Jupyter Notebooks
4. Data Manipulation and Analysis with `pandas`

### Attention to Detail

If you have searched for a job, you have probably seen "attention to detail" appear on a job description. In a [survey of hiring managers](https://www.payscale.com/data-packages/job-skills), fully 56% of them said they felt that recent college grads lacked this skill. So, what does "attention to detail" mean?

Attention to detail means that you accomplish tasks thoroughly and accurately. You need to understand what is being asked of you, and double-check that your work fulfills all of the requirements. This will help make you a "no-brainer hire" because it helps employers feel confident that they will not have to double-check your work. For further reading, check out [this article](https://www.indeed.com/career-advice/career-development/attention-to-detail) from Indeed.


### Data Communication

Communication is another key "soft skill". In [the same survey mentioned above](https://www.payscale.com/data-packages/job-skills), 46% of hiring managers said that recent college grads were missing this skill.

Because "communication" can encompass such a wide range of contexts and skills, we will specifically focus our Phase 1 objective on Data Communication. We define Data Communication as:

> Communicating basic data analysis results to diverse audiences via writing and live presentation

To further define some of these terms:

* By "basic data analysis" we mean that you are filtering, sorting, grouping, and/or aggregating the data in order to answer business questions. This project does not involve inferential statistics or machine learning, although descriptive statistics such as measures of central tendency are encouraged.
* By "results" we mean your ***three visualizations and recommendations***.
* By "diverse audiences" we mean that your presentation and notebook are appropriately addressing a business and data science audience, respectively.

### Authoring Jupyter Notebooks

According to [Kaggle's 2020 State of Data Science and Machine Learning Survey](https://www.kaggle.com/kaggle-survey-2020), 74.1% of data scientists use a Jupyter development environment, which is more than twice the percentage of the next-most-popular IDE, Visual Studio Code. Jupyter Notebooks allow for reproducible, skim-able code documents for a data science audience. Comfort and skill with authoring Jupyter Notebooks will prepare you for job interviews, take-home challenges, and on-the-job tasks as a data scientist.

The key feature that distinguishes *authoring Jupyter Notebooks* from simply *writing Python code* is the fact that Markdown cells are integrated into the notebook along with the Python cells in a notebook. You have seen examples of this throughout the sessions we have been having, but now it's time for you to practice this yourself!

> Headers in Markdown are delineated with one or more `#`s at the start of the line. You should have a mixture of headers and plaintext (text where the line does not start with `#`)


### Data Manipulation and Analysis with `pandas`

`pandas` is a very popular data manipulation library, with over 2 million downloads on Anaconda (`conda install pandas`) and over 19 million downloads on PyPI (`pip install pandas`) at the time of this writing. In our own internal data, we see that the overwhelming majority of Flatiron School DS grads use `pandas` on the job in some capacity.

Unlike in base Python, where the Zen of Python says "There should be one-- and preferably only one --obvious way to do it", there is often more than one valid way to do something in `pandas`. However there are still more efficient and less efficient ways to use it. Specifically, the best `pandas` code is *performant* and *idiomatic*.

Performant `pandas` code utilizes methods and broadcasting rather than user-defined functions or `for` loops. For example, if you need to strip whitespace from a column containing string data, the best approach would be to use the [`pandas.Series.str.strip` method](https://pandas.pydata.org/docs/reference/api/pandas.Series.str.strip.html) rather than writing your own function or writing a loop. Or if you want to multiply everything in a column by 100, the best approach would be to use broadcasting (e.g. `df["column_name"] * 100`) instead of a function or loop. You can still write your own functions if needed, but only after checking that there isn't a built-in way to do it.

Idiomatic `pandas` code has variable names that are meaningful words or abbreviations in English, that are related to the purpose of the variables. You can still use `df` as the name of your DataFrame if there is only one main DataFrame you are working with, but as soon as you are merging multiple DataFrames or taking a subset of a DataFrame, you should use meaningful names. For example, `df2` would not be an idiomatic name, but `movies_and_reviews` could be.

We also recommend that you rename all DataFrame columns so that their meanings are more understandable, although it is fine to have acronyms. For example, `"col1"` would not be an idiomatic name, but `"USD"` could be.


## Summary

This project will give you a valuable opportunity to develop your data science skills using real-world data. The end-of-phase projects are a critical part of the program because they give you a chance to bring together all the skills you've learned, apply them to realistic projects for a business stakeholder, practice communication skills, and get feedback to help you improve. You've got this!
