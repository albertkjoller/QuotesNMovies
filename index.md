<h1> Quotes'N'Movies </h1>

Everyone loves a good movie. But how much does your decision to go to a movie theater to watch a movie depend on recommendations from other people? It could be people you know, movie critics in magazines or even interviews with actors and actresses. Do you ever wonder whether the old saying “bad publicity is good publicity” is in fact true or not? 

In this datastory we intend to guide you through an exciting universe of movie publicity, success and legacy. We will find out how general publicity around movies "correlate/doesnt" with movie success, how public opinion on a movie "correlate/doesnt" with movie success and legacy, and finally we will try to understand where we may have biases regarding public opinion and IMDb ratings of movies. These are the three general topics we will cover but in each section we will answer subquestions and show you the wonderful visualisations that can be created with data.

It is important, before we start, to be on the same page with a few things, that we will bring up a lot. We will be working with movies that were released to theaters in the time period 2015 to 2020. It will not be all movies since that would require us to use cloud computing, so we have chosen 56 American movies. We will use success defined by Box Office income for a given movie (money earned through theater-tickets) and the legacy of a movie is defined by the IMDb rating of that movie. The reason we separate these two terms is, that while Box Office will only be accumulated during the period of theatrical release, the IMDb rating can keep changing right until we downloaded the data this fall.

With that being said, let’s begin by asking ourselves; how does the public coverage of movies in media relate to the success of the movies concerned?


<h2> Relation Between Publicity and Movie Success</h2>
In this section, we will focus on the success of movies. This means that IMDb-ratings will not be reviewed in this section. We will use three datasets, and for good measure, they should be introduced to you here.

<ul>
   <li>QuoteBank, which is a bank of quotes. This was filtered to contain only quotes that mention movies.</li>
   <li>IMDb, which is a dataset taken from their website. It has a list of features for each movie such as IMDb-rating, total domestic Box Office (domestic meaning US-based).</li>
   <li>boxOffice is the last dataset. It contains time-series data for movie attributes such as domestic Box Office.</li>
</ul>

<h2> Comparing Quotes and Domestic Box Office</h2>

We wanted to find out whether there was a correlation between a movie's total publicity, eg. number of quotes, and total income, eg. Box Office. We started by fitting a linear regression to two variables. X was going to be the total domestic box office for a given movie and Y was going to be the total number of quotes about that movie. It looked a little something like this:

##ADD PLOT OF LINREG##

The blue dots are all of our values with an X and Y value, while the blue line is the linear regression. As you can see, the line doesn't fit the data perfectly, but it is actually statistically significant anyway. That means that we can in fact conclude that there is a positive correlation between the two variables. Or in other words; when a movie has a higher box office, there tend to be more publicity around that movie. 

Well, let's see what the opinion in the coverage of movies has to say. Is bad publicity still good publicity? For this task, we #ALBERT WHAT DO WE DOOOO?#

Okay, that was total quotes and total box office for movies. But imagine you read the news paper today and see an article about the new Star Wars movie. You decide to go to a theater and watch it, because of that news article. Are you alone, or is it something people generally do? Let's use an example.

{% include star_wars_quotes_box.html %}

This is the latest movie in the Star Wars saga. The blue bars show you the daily domestic income, while the red bars show you the daily number of quotes. You can hover your mouse on the bars and get more information, if you want. One might speculate that if our hypothesis above, that everyone watches movies based on publicity of the movies, is true the red and blue bars should follow each other. If only a few quotes were in the news on a given day, the box office for the same day or the next day should also be pretty low compared to days with high media coverage.

Does the bar plot follow this hypothesis? Not really, no. This means that although there might generally be more total quotes for blockbusters, there is not really a daily correlation between quotes and movie success.


<ul>
   <li> Which one was most incoming movie, etc. </li>
   <li> (Some of RQ1) </li>
   <li> (Some of RQ3 - maybe?) </li>
</ul>

<h3> Media coverage </h3>

In terms of number of quotation:
{% include dailyNumQuotes_boxOffice.html %}


In terms of sentiment of quotations:
{% include dailySent_boxOffice.html %}


```markdown
```
<h2> How did we respond to the movies? </h2>

<h3> Rating of movies (IMDb) </h3>
(Some of RQ2)

<table>
   <caption> Ratings of movies </caption>
   <tr>
      <th> <b> Score </b> </th>
      <th> <b> Minimum </b> </th>
      <th> <b> Maximum </b> </th>
      <th> <b> Average </b> </th>
   </tr>
   <tr>
      <th> Sentiment based </th>
      <th> 4.6 </th>
      <th> 9.0 </th>
      <th> 6.9 </th>
   </tr>
   <tr>
      <th> IMDb users </th>
      <th> 5.6 </th>
      <th> 8.5 </th>
      <th> 7.2 </th>
   </tr>
   <tr>
      <th> IMDb critics </th>
      <th> 3.3 </th>
      <th> 9.5 </th>
      <th> 6.8 </th>
   </tr>
   <tr>
      <th> IMDb critics </th>
      <th> 4.5 </th>
      <th> 8.8 </th>
      <th> 7.0 </th>
   </tr>
</table>


<ul>
   <li> How are these in general? Main points of investigation of IMDb data </li>
   <li> Is the sentiment of quotes over all time somewhat represented in the IMDb rating? </li>
   <ul>
      <li> Overall </li>
      <li> Voters </li>
      <li> Critics </li>
   </ul>
</ul>




<h3> Do we need to be aware of biases in the legacy? </h3>
Bias in ratings
(RQ4)



```markdown
plotly example 1
```


<h2> Conclusion </h2>
