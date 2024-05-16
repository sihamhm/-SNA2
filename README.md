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

In order to analyse and test our hypothesis, we decided to use Google Collab in Phython. In order to find the two actors that have played in the most movies and the two actors that have played in the least movies. When we were able to extract these informations we generated a social network graph through the use of Sigma. We set the four found actors as nodes and each movies as edges, so we would be able to see how famous and not so famous actors are connected. 

After doing so, we have to get the betweenness centrality which is the number of times a node is included in the shortests path between other nodes in a social network. Then, the degree centrality which would explain how well connected a node is in the network, by measuring the ratio of edgesconnected to a node to the total number of edges. We also studied the clustering coefficient which measure of the grouping of nodes in a network. 

## Data and code
Here is the link to our Google Collab: 

## Analysis and Results
With the help of the graph we made, we are now able to have a better understanding of the social network in the film industry. 

## Conclusion
