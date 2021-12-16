<h1> Quotes'N'Movies </h1>

The Cinematic Art is one of the [most important arts in Humanity](https://notesread.com/importance-of-cinema/) and with its wide-ranging scope of artistic story telling and visual creativity, even the greatest film critic has a favourite movie. Already in 2009, the amount of tickets sold for movie theaters [was on scale with the number of living people across the planet](https://thoughteconomics.com/the-role-of-film-in-society/) - the movie industry has grown to be one of the larger industries in terms of revenue. With its wide-ranging appeal and ability to catch the viewer, movies constitute a potential arena for affecting Societal opinions and tendencies. The affective power of movies are thus important to have in mind when considering the Cinematic Art.

Have you ever had the thought that your decision to go to a movie theater and watch a movie possibly depends on recommendations from other people? Movies are constantly being covered in the media in both positive and negative ways and it is not hard to imagine that statements from movie critics or interviews with actors and actresses could potentially influence how you receive the movie. And in which way? Could it be that the old saying <font size="+4"> <b> “bad publicity is good publicity”  </b> </font> is in fact true or is it just an outdated saying? 

This data story intends to guide you through an exciting universe of Quotes'N'Movies: an intriguing visual investigation on the publicity, success and legacy of recently published movies. 
We hope to broaden your mind and get you to realize that there is possibly other factors associated with a movie's success than its quality!

<!-- We will find out how general publicity around movies "correlate/doesnt" with movie success, how public opinion on a movie "correlate/doesnt" with movie success and legacy, and finally we will try to understand where we may have biases regarding public opinion and IMDb ratings of movies. These are the three general topics we will cover but in each section we will answer subquestions and show you the wonderful visualisations that can be created with data.-->
<!-- Nice points but save them untill they're relevant: It is important, before we start, to be on the same page with a few things, that we will bring up a lot. We will be working with movies that were released to theaters in the time period 2015 to 2020. It will not be all movies since that would require us to use cloud computing, so we have chosen 56 American movies. We will use success defined by Box Office income for a given movie (money earned through theater-tickets) and the legacy of a movie is defined by the IMDb rating of that movie. The reason we separate these two terms is, that while Box Office will only be accumulated during the period of theatrical release, the IMDb rating can keep changing right until we downloaded the data this fall.-->

If you're ready? Let's start!

<h2> <em> Cinematastic Facts </em> about recently published movies </h2>

<!-- Movies intro -->
In the periode between 2015-2020 a total of <font size="+4"> <b> 2486 </b> movies </font> premiered in movie theaters in the United States.
{% include yearly_movies.html %}

<!-- Box Office intro -->
The total revenue from Box Office sales within this period was <font size="+3"> <b> US$ 56.43 Billion </b> dollars </font> at the U.S. cinemas
{% include yearly_BoxOffice.html %}
<!-- Maybe use this instead: The total income from ticket sales within each years were heavily impacted by a small set of the movies broadcasted within that year. -->
A handfull of movies within each year were the major actors in terms of income from ticket sales. The Top 10 movies within each year occupy a major part of the total Box Office sales.
{% include yearly_BoxOfficeByMovie.html %}

<!-- Box Office raceplot -->
The top-ranking movies in terms of income in each year heavily battled the top-ranking movies from other years in the combat for becoming the most successfull movie in the period in terms of revenue.
{% include totalBoxOffice.html %}

<!-- Quotes intro -->
In this same period a total of <font size="+4"> <b> 70.180 </b> quotes </font> related to Top 10 movies within each year were printed on online media webpages.
{% include yearly_Quotes.html %}




<!-- With that being said, let’s begin by asking ourselves; how does the public coverage of movies in media relate to the success of the movies concerned? -->




<h2> How did coverage of movies relate to their success when played on-screen? </h2>
<!-- Old title: Relation Between Publicity and Movie Success -->
<!-- Comment (think we should avoid talking about sections): In this section, we will focus on the success of movies. -->

###Sugestion: Tell the story from RQ1 - without encountering temporal data but just looking at sums.
Also tell it about the sentiment in the non-temporal setting

###Conc: On a movie sequence level: linear relation between revenue and number of quotes - both ways (which plots???) - high in cause high in another.
This is also the case for sentiment --> at least we can say that the total sentiment of a given movie within the period it airs on paper impacts the box office on a movie sequence level. 

![qmak](https://user-images.githubusercontent.com/57899625/146338088-08a20c40-a886-4bcd-823d-b97fe1607f9d.jpeg)


<h3> On a daily basis </h3>
<!-- <h3> Comparing Quotes and Domestic Box Office</h3> -->

Diving in to the temporal patterns of ... movie releases... gives a more complete picture of the tendencies.

###Sugestion: Start with an example? Then follow same approach as above - encountering temporal data - conclusion from Granger causality.
Also - again - tell it for the sentiment.
###Conc: On the movie basis it feels safe to say that box office sales are caused by the number of quotes for the majority of the investigated movies. This is not generalizable to every movie and we are not able to conclude whether high or low number of quotes causes a high or low box office income for the specific movies.
Same is the case for the sentiment --> Here majority of movies' box office are caused by total sentiment but the results are even less generalizable than for the number of quotes. Maybe why the positive correlation is of.



Imagine you read the news paper today and see an article about the new Star Wars movie. You decide to go to a theater and watch it, because of that news article. Are you alone, or is it something people generally do? Let's use an example.

{% include star_wars_quotes_box.html %}

The blue bars show you the daily domestic income, while the red bars show you the daily number of quotes. You can hover your mouse on the bars and get more information, if you want. There seems to be a connection between spikes in the plot. Some people see a news article and then they go watch the movie the following weekend.

This is only true for some movies.

{% include dailyNumQuotes_boxOffice.html %}

For some movies, the quotes do have a relation to the box office of the movies. Let's see if the sentiment of the quotes relate to the box office of the movies too. The sentiment means the positive or negative score of a quote:

{% include dailySent_boxOffice.html %}

Okay, fewer movies have a relation to the sentiment of the quotes.



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
