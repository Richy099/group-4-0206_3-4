# Computing Vision: A New Frontier in Movies
Deloitte AI Academy Capstone Presentation - Cohort 4B, Team 4

![hollywood](https://ca-times.brightspotcdn.com/dims4/default/f057258/2147483647/strip/true/crop/2048x1232+0+0/resize/1200x722!/quality/80/?url=https%3A%2F%2Fcalifornia-times-brightspot.s3.amazonaws.com%2F89%2Fa0%2Fe58e0b431e8ba9ea8444dee8cac8%2Fla-ed-hollywood-sign-wiped-off-the-map-2014112-001)

## Project Overview / Business Problem

We have been tasked with consulting new movie studio, Computing Vision, to explore which types of films are currently doing best at the box office. This includes actionable insights theat the head of Computing Vision's new movie studio can use in selecting which films to create first.

### Business Understanding

Our team targeted two financial metrics for measuring the success of a movie's box office release:
* Total Gross Revenue
* Movie Profitability -- the return on investment (ROI) of a film

There are several other attributes that can be used to measure movie success - such as popularity, review scores, critically acclaimed, etc. - however, we determined the financial success to be a universally agreeable measure of success, and more importantly -- why Computing Vision is interested in entering the space in the first place.

With gross revenue and profitability as our central focus -- next was to identify our three key business questions we determined were most important for Computing Vision to have answered:

* How much, on average, should Computing Vision invest into producing movies?
* What genres of movies should Computing Vision focus on based on total realized profits and profit?
* Which season is best for Computing Vision to release movies?

By completing the thorough data analysis steps seen below -- we are to produce our recommendations for Computng Vision.

### Data Understanding

In the folder `Data/original_data` are movie datasets from the following movie websites:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

Because this data was collected from various locations, the first step will be combining the different files into a single SQLite DB.

The resulting DB will form a schema that looks like this:

![movie_data_db_schema](/Images/DB_schema.jpg)

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
* `tmdb.movies.csv`
  * Used for movie genres and other pertinent movie info from The Movie Database (denoted in magenta)
* `tn.movie_budgets.csv`
  * Contains important financial information across thousands of major movie titles (denoted in gold). 
* `tn.movie_budgets_updated.csv` 
  * An updated, reformatted version of the above.


### Data Analysis
After cloning this repo, navigate to the `group-4-0206_3-4` directory in your terminal. Launch your local Jupyter notebook by typing `jupyter noteook` and navigate to the file `final_group4_notebook`within the Notebooks folder.

Here you will find the steps to connect to the SQLite database and begin manipulating the data necessary for analysis


### Statistical Communication
- Results of statistical inference 
- Interpretation of these results in the context of the problem


### Conclusion
- Summary of conclusions including three relevant findings 

