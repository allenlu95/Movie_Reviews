# Movie_Reviews
Compares movie reviews from Fandango, Metacritic, and IMDB
A further description of this dataset can be found here
https://github.com/fivethirtyeight/data/tree/master/fandango

#How to trust Movie reviews
  These days a quick Google search allows us to know whether or not a movie is worth watching. Movie reviews from sites such as Rotten 
Tomatoes, IMDB, and Metacritic have been known to make or break movies. Among these review sites, some are known to be more trust worthy than others. In the following analysis we explore how popular movie review sites like the three mentioned above differ from sites that directly sell tickets to consumers such as Fandango.
#Initial Observation
To get a general overview of our data we plot out a bar graph of all four reviews.

![alt tag](https://github.com/allenlu95/Movie_Reviews/blob/master/download.png)




Clearly Fandango’s scores are skewed right with no movie falling below 3 stars. A look at each graph’s mean confirms our observation, Fandango has the highest average at 4.08 while all other sites have averages from 2.97 to 3.38 almost 1 entire star below Fandango’s (an astounding 20% on a 5 point scale!). Besides having a high average, Fandango has an even higher median; this means there are more movies over 4 stars than under it according to Fandango! 
#Inflated or Just different?
Now that we know Fandango ratings are generally higher, an interesting question arises: Can we just take a Fandango rating subtract it by 1 and get a rating comparable to the other 3 sites? To answer this, we plot every site against each other and observe. To read the following graphs we simply match the far left label for the graph’s y-axis and the far bottom label for the graph’s x-axis. 
![alt tag](https://github.com/allenlu95/Movie_Reviews/blob/master/download%20(1).png)


Certain graphs seem to have linear relations, while others have no distinct pattern. Upon closer inspection the only graphs with no linear pattern happen to be the ones plotted against Fandango. For a more quantitative comparison we look at each movie’s Pearson values (covariance over standard deviation of both). With  -1 representing complete negative correlation and +1 representing perfectly linear correlation we find Fandango has Pearson scores of 0.18, 0.30, 0.57 with Metacritic, Rotten Tomatoes, and IMDB respectively. This is greatly contrasted by Pearson scores of over .69 when we compare Metacrtic, Rotten Tomatoes, and IMDB among themselves. The answer to our question above is a conclusive no. Not only are Fandango ratings on average higher but also Fandango critics’ tastes in movies are different. Just what kind of people are Fandango critics?
#A different taste for movies
We take the absolute difference between Fandango’s ratings and ratings from the other three sites to find the movies with the greatest contrast in opinion. By taking the first 10 movies with the largest difference we find three movies that consistently appear: “Do You Believe?”, ”Little Boy”, and “Annie”. These movies tend to get low scores from Metacritic, IMDB, and Rotten Tomatoes, but perform well with Fandango critics. After carefully watching the trailers of all three movies, it seems to me there is a theme of family and miracles among all three. Perhaps Fandango critics just have a soft spot for family tearjerkers or perhaps getting entire families to the theatres allow for more ticket sales.  
