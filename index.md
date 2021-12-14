<h1> Quotes'N'Movies </h1>

Everyone loves a good movie. But how much does your decision to go to a movie theater to watch a movie depend on recommendations from other people? Movies are constantly being covered in the media in both positive and negative ways and it is not hard to imagine that statements from movie critics or interviews with actors and actresses could potentially influence how you receive the movie. And in which way? Have you ever wondered whether the old saying “bad publicity is good publicity” is in fact true or not in relation to movies? 

###COMMENT: Facts about movies - how many tickets a year or something - kind of intro to the industry without using our data but facts from a good article instead maybe?

This data story intends to guide you through an exciting universe of Quotes'N'Movies: an intriguing visual investigation on the publicity, success and legacy of recently published movies. 
We hope to broaden your mind and get you to realize that there is possibly other factors associated with a movie's success than its quality!

<!-- We will find out how general publicity around movies "correlate/doesnt" with movie success, how public opinion on a movie "correlate/doesnt" with movie success and legacy, and finally we will try to understand where we may have biases regarding public opinion and IMDb ratings of movies. These are the three general topics we will cover but in each section we will answer subquestions and show you the wonderful visualisations that can be created with data.-->

<!-- Nice points but save them untill they're relevant: It is important, before we start, to be on the same page with a few things, that we will bring up a lot. We will be working with movies that were released to theaters in the time period 2015 to 2020. It will not be all movies since that would require us to use cloud computing, so we have chosen 56 American movies. We will use success defined by Box Office income for a given movie (money earned through theater-tickets) and the legacy of a movie is defined by the IMDb rating of that movie. The reason we separate these two terms is, that while Box Office will only be accumulated during the period of theatrical release, the IMDb rating can keep changing right until we downloaded the data this fall.-->

If you're ready? Let's start!

<h2> ###Maybe a title - at least something to mark the difference </h2>

Between 2015-2020 ... movies were on-screen... in movie theaters...

###Specific plots that we do not necessarily use in the RQ's but are useful for the story telling.


<!-- With that being said, let’s begin by asking ourselves; how does the public coverage of movies in media relate to the success of the movies concerned? -->


<h2> How does the coverage of movies relate to their success when airing? </h2>
<!-- Old title: Relation Between Publicity and Movie Success -->

<!-- Comment (think we should avoid talking about sections): In this section, we will focus on the success of movies. -->

{% include totalBoxOffice.html %}

<h3> Comparing Quotes and Domestic Box Office</h3>
Imagine you read the news paper today and see an article about the new Star Wars movie. You decide to go to a theater and watch it, because of that news article. Are you alone, or is it something people generally do? Let's use an example.

{% include star_wars_quotes_box.html %}

The blue bars show you the daily domestic income, while the red bars show you the daily number of quotes. You can hover your mouse on the bars and get more information, if you want. There seems to be a connection between spikes in the plot. Some people see a news article and then they go watch the movie the following weekend.

This is only true for some movies.

{% include dailyNumQuotes_boxOffice.html %}

For some movies, the quotes do have a relation to the box office of the movies. Let's see if the sentiment of the quotes relate to the box office of the movies too. The sentiment means the positive or negative score of a quote:

{% include dailySent_boxOffice.html %}

Okay, fewer movies have a relation to the sentiment of the quotes.


<h2> How did we respond to the movies? </h2>

<h3> Rating of movies (IMDb) </h3>

### RQ2 conclusion?

<table class="center">
   <tr>
      <th> <b> Score </b> </th>
      <th> <b> Minimum </b> </th>
      <th> <b> Maximum </b> </th>
      <th> <b> Average </b> </th>
   </tr>
   <tr>
      <td> Sentiment based </th>
      <td> 4.6 </th>
      <td> 9.0 </th>
      <td> 6.9 </th>
   </tr>
   <tr>
      <td> IMDb users </th>
      <td> 5.6 </th>
      <td> 8.5 </th>
      <td> 7.2 </th>
   </tr>
   <tr>
      <td> IMDb critics </th>
      <td> 3.3 </th>
      <td> 9.5 </th>
      <td> 6.8 </th>
   </tr>
   <tr>
      <td> IMDb critics </th>
      <td> 4.5 </th>
      <td> 8.8 </th>
      <td> 7.0 </th>
   </tr>
   <caption> Different ratings of movies </caption>
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
