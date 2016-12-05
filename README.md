#B669 Final Project Report
### Naveen Jetty

###Minimal - Les Miserables

#### 1. Is a window of size 15 a good window size for the characters that you think are related?
For the Les Miserables, A larger window size means gives rise to false nodes and a smaller nodes might miss out meaningful inferrence between characters. In my opinion, the windows size depends on the style of the author as some prefer using pronouns to that of using nouns in the sentences. Inferring a relationship between in a such case requires a larger window size. Coming to 'Les Miserables', I found that the 15 is a good size.


#### 2. What are the strengths and weaknesses of a larger window size? Give an example of a relationship that was missed because of a window size of N=15?
##### Strengths: 
When we have larger window size, the possibility of missing out nodes or character relationship inferrences is minimal. Also when the book has fewer nodes, a larger window size enables us to get more nodes, which might help in finding the hidden patterns in the character inference. Also one thing that I have noticed is that some names are being cut such as Jean Valjean becomes Jean and valjean as two seperated nodes. Having a larger window improves the probability of picking the entire name in a single window.

##### Weaknesses: 
With a increase in window size, the contextual information might be incorrectly mixed up. Also it might lead to false nodes with unimportant edges. For example, the relation between Valjean and Fantine got messier as the window size is increasing because of other unimportant edges reducing the relationship weight between the two characters.

#### 3. Gephi Visualization:
![Les Miserables](https://github.com/njetty/B669-Final-Project/blob/master/les.png)

####Minimal Plus - Pride and Prejudice
#### 1. Is a window of size 15 a good window size for the characters that you think are related?
For the Pride and Prejudice, I found the size of 15 is a good fit as the character relationships were inferred correctly

#### 2. What are the strengths and weaknesses of a larger window size? Give an example of a relationship that was missed because of a window size of N=15?
The same strengths and weakness from minimal are applicable here

#### When you analyzed texts of your own choosing that you're familiar with or interested in, did you glean any insights from this type of analysis that would be harder to glean from a simple readthrough?
Yes, when reading book you tend to be involved in the story and might miss some details that can be observed at a higher level. For example the characters in the book, Elizabeth Bennet and Jane has stronger edge in the graph than the edge between the main characters Fitzwilliam Darcy and Elizabeth Bennet.

#### Gephi Visualization:
![Pride and Prejudice](https://github.com/njetty/B669-Final-Project/blob/master/pnp.png)




