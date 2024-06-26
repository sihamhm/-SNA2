# SNA2 - final project

## Importance of a movie’s popularity and its impact on the social network connections of the participant actors. 
Siham Hachem and Tamara Diaz K

# Introduction
Hollywood stands as the biggest place for aspiring individuals seeking fame and networking opportunities. The allure lies in the perceived interconnectedness, where once inside, everyone seems to know everyone, fostering the potential for influential connections, particularly through participation in Hollywood productions. Yet, the extent of this networking advantage remains uncertain, leaving one to wonder about the magnitude of its social web expansion.

This project delves into the intricacies of Hollywood connections to investigate whether a movie's popularity correlates with the number of connections gained by its actors. By investigating pre- and post-movie social networks of two A-list and two C-list celebrities, compared against the film's popularity, the investigation takes shape. Comparisons include participation frequency, network size, and influence, enhanced by their impact on the media.

The objective is to determine the significance of both movie popularity and actor status on social network dynamics, offering insights into the symbiotic relationship between Hollywood success and interpersonal connections via social networks.

## Hypothesis
The hypothesis is that: The more an actor has played in movies, the greater the size of their social network will be. However, for information to flow seamlessly the network needs actors who have played in less movies and who have less connections.

When thinking about film actors, fame, success and mostly well connected people come to mind. For this reason, we wanted to study the idea that playing in a lot of movies can help people increase the size and range of their social network.

## Methodology
We used the film industry dataset made by IMDB, the Internet Movie Databased ( provided by the teacher in class ) 

- The dataset includes 1000 nodes.

- Accross a period of time approximativly from 1921 to 2020.

- Each node represents an actor.

- Each edge represents the actor's connections with one another.

As we can see in the Google collab work, the first figure is us charging the entire dataset, but asking the software to only show five loadings, without deleting them, just masking them so it would be easier to work on it. 

In the second figure, we did a "subset", in other words, we removed the columns that were not needed and asked to only show the important variables for our study, those being the movie titles and the actors.

Then we are able to start our analysis.

To help us analyze and test our hypothesis, we decided to use Python for coding in Google Collab in order to find the two actors that have played in the most movies and the two actors that have played in the least movies. When we were able to extract this information we generated a social network graph. We set the four found actors as nodes and each movie as edges, so we would be able to see how famous and less famous actors are connected.

After doing so, we will have to find the diameter of the social network and then we have to get the betweenness centrality, which is the number of times a node is included in the shortests path between other nodes in a social network and the degree centrality which would explain how well connected a node is in the network. 

## Data and code
Here is the link to our Google Collab: https://colab.research.google.com/drive/1luYxRaw4dY_D-QhyaMWHdkGXo7Vkz8eM#scrollTo=XJ0cVikGmuTI

## Analysis 
With the help of the graphs we made, we are now able to have get a better understanding of the way in which social networks in the film industry work. 

Firstly, we felt like it was important to decide which actors had played in the most and least movies, to then do the analysis. 

<img width="219" alt="Screenshot 2024-05-17 at 2 52 28 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/f4b4db24-9011-495f-84a2-ab9dd2783b75">

* actors that have played in the most movies. 

As we can see, Robert De Niro has played in 17 different movies, Tom Hanks in 14, Al Pacino has played in 13 movies that were listed, Clint Eastwood and Brad Pitt have both played in 12 movies. In other words, if we follow our hypothesis, Robert De Niro should be the actor that is the most well connected in Hollywood, since he has played in the most movies. 

Then, when we change the entry .orderBy("count", ascending=False) to .orderBy("count", ascending=True), we are able to have the list of the 5 actors that have least played in the least amount of movies. 

<img width="228" alt="Screenshot 2024-05-17 at 3 22 10 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/ac1b592c-30c5-4b48-ab90-29ea0690d008">

* actors that have played in the least movies. 

As we can see, all of the five actors have played in only one movie each. If we follow the hypothesis, they should be the people that are the less connected to others and who has the least dense social network. However, their importance in the network should not be understated, since removing them from the network may have consequences, or make a really big impact on the current social networks. 

- We would like to mention the fact that we were not able to find the diameter of this social network, the software kept posting "error". 


## Actors' social network

In the third graph, we can see the actor's social network. This graph includes all the actors and all the movies mentioned in the dataset. We need to remember that the nodes (blues dots) are the actors and the edges (black lines) are the links, illustarting the movies in which each actor played in. If we keep in mind that, if two actors played in the same movie as other actors once, it means that their co-stars are now part of their social networks. In other words, the edges create connections between actors, which expands their social network.

<img width="1216" alt="Screenshot 2024-05-17 at 4 04 53 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/0c9c4192-54a7-4f55-91da-bc1ba47d2f36">

* actors' social network

The graph that we obtained shows an overload of edges and nodes in the social network, so we are not able to clearly see the connections. However, this tells us important things regarding this social network, since actors are really connected to one another. These connections are made on movie sets, by working with different actors and directors, the celebrities are able to expand their social network and be better connected to everyone. In addition, even if an actor only played in one movie, it has opened for them the opportunity to be connected to others and start building up their own network.

## Betweenness Centrality 

<img width="1239" alt="Screenshot 2024-05-17 at 4 07 23 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/e1436994-770e-42f1-b297-1ec66fdc8f2e">

* actors' betweenness centrality

Betweenness centrality is used in network analysis to determine the importance of a node within a network. Let’s take the example of a city map with various intersections (nodes) and roads (edges) connecting them. Betweenness centrality identifies the intersections that most frequently serve as shortcuts or bridges for the shortest paths between other intersections. These intersections are crucial because they connect different parts of the city efficiently.

Contrary to degree centrality, which identifies the most connected nods in a networks, betweenness centrality helps to identify which nods (or actors in our case) are the most important to facilitate a seamless transfer of information among the different nodes.

Here we can see that Dave Patel (0.066) despite being among the actors who played in the least number of movies and therefore ranking low in degree centrality he ranks the highest in betweenness centrality. This means that if Dave Patel were to be removed from our network, the flow of information would be less efficient, since some nodes would then be completly isolated from the rest of the network.

## Degree Centrality

<img width="1299" alt="Screenshot 2024-05-17 at 4 07 32 AM" src="https://github.com/sihamhm/-SNA2/assets/167986363/2beed44e-522c-4e3a-87a1-52b126c1091b">

* actors' degree centrality

The theory of degree centrality posits that the total number of direct connections to a node, which can be separated into entering and exiting connections, can allow us to identify the most influential persons in a social network. 

In this context, the degree centrality of an actor in our social network is highly correlated to the total number of movies they have appeared in. For instance, Robert De Niro (0.0165), who has played in the highest number of movies, also has the most connections in our social network. He is followed by Tom Hanks (0.014), who comes second in terms of the number of movies he has played in. Brad Pitt (0.013) and Al Pacino (0.012) follow, with almost the same number of connections, ranking third and fourth, respectively. 

This result makes sense, as it can be argued that the higher the number of movies an actor appears in, the more likely they are to be exposed to more people and make connections than actors who have appeared in fewer movies. This increased exposure allows them to expand their centrality within the social network.

## Conclusion

When looking at the graphs, it can be argued that there is a high correlation between the number of movies an actor played in and their degree centrality; they are the nodes with the most connections in the network. However, degree centrality is also impacted by the betweenness centrality of the networks since betweenness centrality helps identify how efficiently information moves within the networks. Betweenness centrality is not related to the number of movies an actor played in, but rather it focuses on their connections and own social network links. The example of Dave Patel perfectly illustrates this scenario, since Dave Patel is not among the actors who have the highest degree centrality since he is one of the actors analyzed who at the time of research had been part of the actors to have a role in the least amount of movies. However, his high level of betweenness centrality shows that without him other nodes would be isolated from the rest of the network. Therefore, making the flow of information less efficient, and proving that the size of an actor's social network is not always about having a part in many big movies, but rather be in the right movie and knowing the right people.




