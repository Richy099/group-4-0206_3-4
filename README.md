# Computing Vision: A New Frontier in Movies
Deloitte AI Academy Capstone Presentation - Cohort 4B, Team 4

![hollywood](https://ca-times.brightspotcdn.com/dims4/default/f057258/2147483647/strip/true/crop/2048x1232+0+0/resize/1200x722!/quality/80/?url=https%3A%2F%2Fcalifornia-times-brightspot.s3.amazonaws.com%2F89%2Fa0%2Fe58e0b431e8ba9ea8444dee8cac8%2Fla-ed-hollywood-sign-wiped-off-the-map-2014112-001)

## Project Overview / Business Problem

We have been tasked with consulting new movie studio, Computing Vision, to explore which types of films are currently doing best at the box office. This includes actionable insights theat the head of Computing Vision's new movie studio can use in selecting which films to create first.

### Business Understanding

- Stakeholder and Key Biz Questions


### Data Understanding and Analysis

- Source of data
- Description of data
- Three visualizations


In the folder `Data/original_data` are movie datasets from the following movie websites:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

Because this data was collected from various locations, the first step will be combining the different files into a single SQLite DB.

The resulting DB will form a schema that looks like this:

![movie data db_schema](https://github.com/Richy099/group-4-0206_3-4/tree/master/Images/DB_schema.jpg)

Your Jupyter Notebook will walk you through the exact steps of creating this merged database and accessing the data needed for analysis.

The list of files available in the Data folder are as follows:

* `original_im.db`
  * Tables from IMDB (denoted in light grey on above schema)
* `bom.movie_gross.csv`
  * Helpful for analyzing gross revenue of movies, per 'Box Office Mojo' (denoted in blue)
* `rt_movie_info.csv`
  * Basic movie info from Rotten Tomatoes  (denoted in dark grey)
* `rt_reviews.csv`
  * Critic and audience reviews from Rotten Tomatoes (denoted in dark grey)
* `tmdb.movies.csv
  * Used for movie genres and other pertinent movie info from The Movie Database (denoted in magenta)
* `tn.movie_budgets.csv`
  * Contains important financial information across thousands of major movie titles (denoted in gold). 
* `tn.movie_budgets_updated.csv` 
  * An updated, reformatted version of the above.




### Statistical Communication
- Results of statistical inference 
- Interpretation of these results in the context of the problem

### Conclusion
- Summary of conclusions including three relevant findings 






### Jupyter Notebook

The Jupyter Notebook is a notebook that uses Python and Markdown to present your analysis to a data science audience.

* ***Python and Markdown*** means that you need to construct an integrated `.ipynb` file with Markdown (headings, paragraphs, links, lists, etc.) and Python code to create a well-organized, skim-able document.
  * The notebook kernel should be restarted and all cells run before submission, to ensure that all code is runnable in order.
  * Markdown should be used to frame the project with a clear introduction and conclusion, as well as introducing each of the required elements.
* ***Data science audience*** means that you can assume basic data science proficiency in the person reading your notebook. This differs from the non-technical presentation.

Along with the presentation, the notebook also describes the project ***goals, data, methods, and results***. It must include at least ***three visualizations*** which correspond to ***three business recommendations***.




## Summary

This project will give you a valuable opportunity to develop your data science skills using real-world data. The capstone projects are a critical part of the program because they give you a chance to bring together all the skills you've learned, apply them to realistic projects for a business stakeholder, practice communication skills, and get feedback to help you improve. You've got this!
