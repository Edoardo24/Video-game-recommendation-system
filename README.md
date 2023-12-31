# Video-game-recommendation-system
The project consists of a recommendation system for video games in which the Steam catalog was examined. The dataset contained more than 70000 games developed and released on steam from 1997. Therefore, the goal of the project was to create a recommendation systema that based on the content of the game or based on the history of the user on the Steam platform. To sum up the results, the output of the results of the system is of high relevance. In addition to the main recomendation system, we wadeted to detect a path between the increase of the development of video games genres based on specific cluster. Thanks to the results of the project would be possible to suggest to the customer (video gamer) the most appropiate game based on their prefernces and at the same time to suggest to each company wich game are more viral based on their user target.

The first phase was to detect the paths of the different time periods. To be able to visualize the dataset was necessary to use three different dimensionality reduction (PCA, T-SNE and UMAP). Based on the Elbow and the Silhouette methods was possible to identify the number of clusters that could be identified. Therefore, the three periods (1997-2007, 2007-2017, 2017-2015) were displayed and clustered separately so that they could be compared to draw conclusions. ![UMAP_git](https://github.com/Edoardo24/Video-game-recommendation-system/assets/46709461/ccbeae38-8b2f-42a7-8d93-24b9c68f02d1) The result of the analysis is very interesting both in terms of the methods used and the differences in the increase in the numbers of games produced for a specific genre within a cluster examined. For example, in a cluster in the period 2007-2017 and 2017-2015 the genre which has increased the most was completelly different from the one of another cluster.

![image](https://github.com/Edoardo24/Video-game-recommendation-system/assets/46709461/f77c52ed-81e8-4f71-bb3a-9f4079440c8c)


## The recommendation system
The recommendation system was based on the content of the game. All the relevant information, like tags, description, genre... were counter factorized to create a matrix with only 0 and 1 on which different ML methods can be applied. With a matrix full of number was possible to calculate the distance between two point (two games) and therefore, to create a list with the 10 games that are most similar. The ranking of the simar games can be influenced based of other factors like price, ads program, date of release and so on. 
If the user history would be provided would be possible to detect the user space in which the user can be inserted. In this case the user history was not provided and therefore, it was created manually. 

Another alternative for creating a group of similar games is to use the Convex Hull method, which creates a convex shape that contains certain games that have similar characteristics to those required as a whole.![Convex_Hull](https://github.com/Edoardo24/Video-game-recommendation-system/assets/46709461/95a84612-91b8-4aa4-9fb3-3525034cb254)


## Authors
- Edoardo Berardi Vittur
- Ali Yassine
- Ethan Greene
