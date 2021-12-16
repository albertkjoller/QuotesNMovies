<h1> Quotes'N'Movies </h1>

The Cinematic Art is one of the [most important arts in Humanity](https://notesread.com/importance-of-cinema/) and with its wide-ranging scope of artistic story telling and visual creativity, even the greatest film critic has a favourite movie. Already in 2009, the amount of tickets sold for movie theaters [was on scale with the number of living people across the planet](https://thoughteconomics.com/the-role-of-film-in-society/) - the movie industry has grown to be one of the larger industries in terms of revenue. With its wide-ranging appeal and ability to catch the viewer, movies constitute a potential arena for affecting Societal opinions and tendencies. The affective power of movies are thus important to have in mind when considering the Cinematic Art.

Have you ever had the thought that your decision to go to a movie theater and watch a movie possibly depends on recommendations from other people? Movies are constantly being covered in the media in both positive and negative ways and it is not hard to imagine that statements from movie critics or interviews with actors and actresses could potentially influence how you receive the movie. And in which way? Could it be that the old saying <font size="+2"> <b> “bad publicity is good publicity”  </b> </font> is in fact true or is it just an outdated saying? 

This data story intends to guide you through an exciting universe of Quotes'N'Movies: an intriguing visual investigation on the publicity, success and legacy of recently published movies. 
We hope to broaden your mind and get you to realize that there is possibly other factors associated with a movie's success than its quality!

If you're ready? Let's start!





<h2> <em> Cinematastic Facts </em> about recently published movies </h2>

<!-- Movies intro -->
In the periode between 2015-2020 a total of <font size="+4"> <b> 2486 </b> movies </font> premiered in movie theaters in the United States.
{% include yearly_movies.html %}

<!-- Box Office intro -->
The total revenue from Box Office sales within this period was <font size="+3"> <b> US$ 56.43 Billion </b> dollars </font> at the U.S. cinemas
{% include yearly_BoxOffice.html %}
<!-- Maybe use this instead: The total income from ticket sales within each years were heavily impacted by a small set of the movies broadcasted within that year. -->
A handfull of movies within each year were the major actors in terms of income from ticket sales. The top 10 movies within each year occupy a major part of the total Box Office sales. It is easily seen that the number of movies and the total box office sales within a year seem to follow a similar trend and are especially low. The deviation for 2020 is due to the societal impact of COVID-19.
{% include yearly_BoxOfficeByMovie.html %}

<!-- Box Office raceplot -->
The top-ranking movies in terms of income in each year heavily battled the top-ranking movies from other years in the combat for becoming the most successfull movie in the period in terms of revenue.
{% include totalBoxOffice.html %}

<!-- Quotes intro -->
In this same period a total of <font size="+4"> <b> 70.180 </b> quotes </font> related to Top 10 movies within each year were printed on online media webpages.
{% include yearly_Quotes.html %}






<h2> How did coverage of movies relate to their success when played on-screen? </h2>
<!-- RQ1 and RQ2 on a "high-level" - movie level -->

On the yearly level of total number of quotes and total income from movies it seems rather unlikely that quotes should affect the Box Office sales as the number of quotes in 2015-2016 compared to the later years do not look similar to the trend in total yearly Box Office revenue.

On the other hand, when regarding movies in general - and thus not on a yearly basis - there is (on paper) a positive relation between the amount of quotes as well as the Box Office related for movies.

<img src="./assets/images/movie.png" width="200" />

So in general, the total income of a movie can to some extend be described by the total amount of quotes portraying the movie. But couldn't it also be the case that content of quotes has a say in describing Box Office sales? One way to look at content of quotes is by analyzing the sentiment of quotes - are they exåressing a positive or negative opinion on the movie they concern? 

<img src="./assets/images/movie.png" width="200" />

So in general, there is a positive relation on paper between the total sentiment content of quotes and the total income from sold ticket for a movie. Though, we are missing the obvious here - ticket sales and quotes are not constant numbers, they are able to change over time and it is fairly reasonable to assume that the temporal aspect related to movies is important...




<h3> Quotes'N'Movies in time </h3>
<!-- RQ1 and RQ2 on a more complete level - time series -->

As it turns out, this assumption is in fact true - Box Office revenue seem to follow trends in time. For instance, the average income on weekdays is peaking on Friday and Saturday - it seems like people favor to watch cinema movies in their weekend.

###Plot the amount of box office per weekday barplot as motivation for looking into time series.
<img src="./assets/images/movie.png" width="200" />

Observing this trend, we start asking ourselves whether the relation between movies and quotes observed is also occuring when encountering temporal trends of ticket sales as well as the number of quotes and their positive/negative sentiment. Let's dive into it and start with an example!


Imagine you read the daily news papers this morning and read several people expressing their opinion on the new Star Wars VII movie. Later this week you decide to validate and end up watching the movie in the cinema. In relation to 'Star Wars VII - The Force Awankens', you were not alone - the ticket sales were affected by how the media covered Star Wars. 

{% include star_wars_quotes_box.html %}

Is this just one isolated example or is the trend of quotes causing box office revenue in the temporal setting generalizable to movies in general?

Digging into the temporal relations for quotes and sentiments to the income from ticket sales reveals that the trend observed for Star Wars VII does not generalize to movies from the combined list of top 10 movies from each year. The daily number of quotes about a movie do have an impact on the box office sales for the movie for most of the considered movies - but not for all of them:

{% include dailyNumQuotes_boxOffice.html %}

This tendency is also seen when considering the daily sentiment of quotes related to box office sales. Here the daily incomes of the majority part of the considered movies are still caused by the total daily sentiment related to the movie. Generalizing this trend however becomes harder than for the number of quotes as the relation is not valid for a larger fraction of the considered movies:

{% include dailySent_boxOffice.html %}

The tendency of quotes affecting box office sales when considering a temporal scale seem to suggest the same as when considering the totality of quotes and box office income - namely that box office sales are influenced by quotes and their sentiment. However, on the temporal level it is revealed that the trend is not general yet appears to be the case for the majority part of movies.

<!-- It is hard to generalize the temporal trend - meaning the number of days in between quote and ticket sale - on which the media coverage affected Star Wars VII. In spite of this -->



<h2> A movie's legacy - how did we respond? </h2>

###Sugestion: General introduction to IMDb ratings! Summary plots etc.
Then continue to the sentiment score --> should we include a temporal aspect here or is it stupid for the story?
###Conc: Sentiment scores do seem (from a first sight) to be comparable to the other metrics. However, it is not
	observed to be the case that the sentiment scores agree with either critics or users when investigating the selected movie series.
	We see that it resembles even more the combined user/critic score but is still not significant.
	Critics and users do not agreee either - thus the sentiment COULD be a valid approach for legacy
	that is a unique metric and reveals other information than the ratings.

<center>
<table class="center">
   <tr>
      <th> <b> Score </b> </th>
      <th> <b> Minimum </b> </th>
      <th> <b> Maximum </b> </th>
      <th> <b> Average </b> </th>
   </tr>
   <tr>
      <td> <i> Sentiment based </i> </td>
      <td> 4.6 </td>
      <td> 9.0 </td>
      <td> 6.9 </td>
   </tr>
   <tr>
      <td> <i> IMDb users </i> </td>
      <td> 5.6 </td>
      <td> 8.5 </td>
      <td> 7.2 </td>
   </tr>
   <tr>
      <td> <i> IMDb critics </i> </td>
      <td> 3.3 </td>
      <td> 9.5 </td>
      <td> 6.8 </td>
   </tr>
   <tr>
      <td> <i> IMDb mixed </i> </td>
      <td> 4.5 </td>
      <td> 8.8 </td>
      <td> 7.0 </td>
   </tr>
</table>
</center>


<h3> Are there systematic biases in the legacy? </h3>

###Sugestion: Cool bias plots on the IMDb data in general and related to sentiment and quotes etc.


<h2> Conclusion </h2>

   
###No idea yet :-)
   

   
<h2> References </h2>
   
###IMDb Dataset, Quotebank, BoxOffice, etc. -- Bob West - ADA (CREDZ!)
