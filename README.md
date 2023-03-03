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


### Data Analysis and Statistical Inference
After cloning this repo, navigate to the `group-4-0206_3-4` directory in your terminal. Launch your local Jupyter notebook by typing `jupyter noteook` and navigate to the file `final_group4_notebook`within the Notebooks folder.

Here you will find the steps to connect to the SQLite database and begin manipulating the data necessary for analysis

Now to the analysis and results...

### Business Question #1: How much, on average, should Computing Vision invest into producing movies?

![movie_revenue](/Images/bizRec1.png)

* Recommendation #1: Follow the Leaders. With tudios making billions of dollars in profit, Computing Vision should invest on average between $440 and $680 million to maximize their ROI
    * The top 10 studios have raked in on average about 1.4 billion dollars in Revenue
    * The top studios have generated about 1.2 billion dollars in Profit on average
    * Studios invested on an average budget/cost of about 440 million dollars. 
    * The top 25 and top 50 of the top 10 Studios have on average spent 440 millions and 680 million dollars





### Business Question #2: Which movies should Computing Vision focus on based on total realized profits and profit?

![genre](/Images/top10profitByGenre.jpg)

* Recommendation #2: Pick the right genre. With all kinds of movie genres in the movie, Computing Vision should invest in making action, adventure, and comedy.
    * The top 3 movie genres raked in more than $1 billion each in profit 
    * Action genres are the most successful with about $6.5 billion in total profit
    * Adventure and comedy respectively totaled roughly $2.8 billion and $1.5 billion




### Business Question #3: When should Computing Vision release its movies?

![seasonRev](/Images/revenueBySeason.jpg)
![seasonProfit](/Images/highestProfitMonth.jpg)

* Recommendation #3: Pick the right season. The best time to release a movie is in the summer, specifically in the month of June.
    * Summer brought in the most ROI with about $4.5 billion
    * The month of June is the best time to release a movie in the summer
    * August is the least profitable month in summer to release a movie


### Conclusion
In addition to our team's recommendations of:
  * Follow the leaders
  * Pick the right genre
  * Pick the right season

We would strongly recommend bolstering today's insights with the following informationL
  * Include latest performance data (post-2017)
  * Additional research (qualitative analysis; surveys)
  * Consider performance across other distributions, such as:
      * Streaming
      * On-demand


## Thank You!
