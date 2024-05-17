# SNA2 - final project
Siham Hachem and Tamara Diaz K
# Introduction
Hollywood stands as the biggest place for aspiring individuals seeking fame and networking opportunities. The allure lies in the perceived interconnectedness, where once inside, everyone seems to know everyone, fostering the potential for influential connections, particularly through participation in Hollywood productions. Yet, the extent of this networking advantage remains uncertain, leaving one to wonder about the magnitude of its social web expansion.


This project delves into the intricacies of Hollywood connections to investigate whether a movie's popularity correlates with the number of connections gained by its actors. By investigating pre- and post-movie social networks of two A-list and two C-list celebrities, compared against the film's popularity, the investigation takes shape. Comparisons include participation frequency, network size, and influence, enhanced by their impact on the media.

The objective is to determine the significance of both movie popularity and actor status on social network dynamics, offering insights into the symbiotic relationship between Hollywood success and interpersonal connections via social networks.
## Hypotheses
The hypotheses is that: The more an actor have played in movies, the more he has his social network is important. 

When we think about film acotrs, we think about fame, success and mostly people well connected. For this reason, we wanted to study if the idea that playing in a lot of movies can help people increase their social network.
## Methodology
We used the film industry dataset made by IMDB, the Internet Movie Databased ( provided by the teacher in class ) 

- The dataset includes 1000 nodes.

- Accross a period of time approximativly from 1921 to 2020.

- Each node represents an actor.

- Each edge represents the actor's connections with one another.

As we can see in the Google collab work, the first figure is us charging the entire dataset, but asking the software to only show five loadings, without deleting them, just masking them so it would be easier to work on it. 

In the second figure, we did a "subset", in other words, we removed the columbs that we did't needed and asked to only show the important variables for our study meaning: The movies title and the actors. 

We were then able to start our analysis. 

In order to analyse and test our hypothesis, we decided to use Google Collab in Phython. In order to find the two actors that have played in the most movies and the two actors that have played in the least movies. When we were able to extract these informations we generated a social network graph through the use of Sigma. We set the four found actors as nodes and each movies as edges, so we would be able to see how famous and not so famous actors are connected. 

After doing so, we have to get the betweenness centrality which is the number of times a node is included in the shortests path between other nodes in a social network. Then, the degree centrality which would explain how well connected a node is in the network, by measuring the ratio of edges connected to a node to the total number of edges. We also studied the clustering coefficient which measure of the grouping of nodes in a network. 

## Data and code
Here is the link to our Google Collab: 

## Analysis and Results
With the help of the graphs we made, we are now able to have get a better understanding of the social network in the film industry. 

Firstly, we felt like it was important to decide which actors had played in the most and least movies, to then do the analysis. 

<img width="219" alt="Screenshot 2024-05-17 at 2 52 28 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/f4b4db24-9011-495f-84a2-ab9dd2783b75">

* actors that have played in the most movies. 

As we can see, Robert De Niro has played in 17 different movies, Tom Hanks in 14, Al Pacino has played in 13 movies that were listed, Clint Eastwood and Brad Pitt have played both played in 12 movies. In other words, if we follow our hypothesis, Robert De Niro should be the actor that is the most connected in Hollywood, since he has played in the most movies. 

Then, when we change the entry .orderBy("count", ascending=False) to .orderBy("count", ascending=True), we are able to have the list of the 5 actors that have least played in movies. 

<img width="228" alt="Screenshot 2024-05-17 at 3 22 10 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/ac1b592c-30c5-4b48-ab90-29ea0690d008">
* actors that have played in the least movies. 

As we can see, all of the five actors have played in only one movie each. If we follow the hypothesis, they should be the people that are the less connected to others and who has the less dense social network. 


## Actors social network

In the third graph, we can see the actor's social network. This graph includes all the actors and all the movies mention in the dataset. We need to remember that the nodes (blues dots) are the actors and the edges (black lines) are the links, illustarting the movies, in which each actor played in. If we keep in mind that, if two actors played in the same movie than other actors once, it means that their co-stars are now part of their social networks. In other words, the edges creates connection between actors, which expend their social network. 

<img width="1201" alt="Screenshot 2024-05-17 at 3 02 00 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/d8b76c42-ee54-4032-b5bf-b8a5ffbaf6f9">

* actors social network





## Conclusion
