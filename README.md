#B669 Final Project Report
### Naveen Jetty

###Minimal - Les Miserables

#### 1. Is a window of size 15 a good window size for the characters that you think are related?
For the Les Miserables, A larger window size means gives rise to false nodes and a smaller nodes might miss out meaningful inference between characters. In my opinion, the windows size depends on the style of the author as some prefer using pronouns to that of using nouns in the sentences. Inferring a relationship between in a such case requires a larger window size. Coming to 'Les Miserables', I found that the 15 is a good size.


#### 2. What are the strengths and weaknesses of a larger window size? Give an example of a relationship that was missed because of a window size of N=15?
##### Strengths: 
When we have larger window size, the possibility of missing out nodes or character relationship inferences is minimal. Also when the book has fewer nodes, a larger window size enables us to get more nodes, which might help in finding the hidden patterns in the character inference. Also one thing that I have noticed is that some names are being cut such as Jean Valjean becomes Jean and valjean as two seperated nodes. Having a larger window improves the probability of picking the entire name in a single window.

##### Weaknesses: 
With a increase in window size, the contextual information might be incorrectly mixed up. Also it might lead to false nodes with unimportant edges. For example, the relation between Valjean and Fantine got messier as the window size is increasing because of other unimportant edges reducing the relationship weight between the two characters.

#### 3. Gephi Visualization:
![Les Miserables](https://github.com/njetty/B669-Final-Project/blob/master/les.png)

####Minimal Plus - Pride and Prejudice
#### 1. Is a window of size 15 a good window size for the characters that you think are related?
For the Pride and Prejudice, I found the size of 15 is a good fit as the character relationships were inferred correctly

#### 2. What are the strengths and weaknesses of a larger window size? Give an example of a relationship that was missed because of a window size of N=15?
The same strengths and weakness from minimal are applicable here

#### When you analysed texts of your own choosing that you're familiar with or interested in, did you glean any insights from this type of analysis that would be harder to glean from a simple read through?
Yes, when reading book you tend to be involved in the story and might miss some details that can be observed at a higher level. For example the characters in the book, Elizabeth Bennet and Jane has stronger edge in the graph than the edge between the main characters Fitzwilliam Darcy and Elizabeth Bennet.

#### Gephi Visualization:
![Pride and Prejudice](https://github.com/njetty/B669-Final-Project/blob/master/pnp.png)

#### Extra Credit Option 1:
The given project though efficient in finding the characters, has a lot of junk data due to the erroneous representation of Capitalization of incorrect words being treated as Characters, Some characters had special characters suffixed with the name making the program think that it is a different character and like wise. Also the places are treated as characters. I was not familiar with the book Les Misearbles and it took me a lot of effort to clean up the data. Also I wanted to clean up as much data as possible before giving the gml file as input to the Gephi. So I parsed the gml file based and removed the nodes that are mistakenly identified as characters.

When working on the Les Miserables, I have found the following set of incorrectly identified set of words.

`"A","Rue","Paris","God","Madame","Monsieur","Bishop","English","Jean","Emperor","Rome","Waterloo","Mother","Father","La","Guard","Did","Baron","Latin","Temple","Does","Saint","Je","Europe","Boulevard","V","Hence","Sir","Alas","Pope","Lord","Et","Le","Thou","Sister","Listen","Jesus Christ","Jesus","Death","Enlarge","Empire","Had","Old","Royal","Mon"` 

I have removed these words from the corpus and generated the gml file for Les Miserables. 
![Les Miserables](https://github.com/njetty/B669-Final-Project/blob/master/les.png)

I have also identified that some of the characters are identified as different characters when they are infact one and the same. For example "Father Fauvent" and "Fauvent" are identified as two separate characters. I have identified such nodes in the gephi and merged them before generating the graph.

When working on the Pride and Prejudice, I have found the following set of words that are incorrectly identified as characters by the program.

`"Mr.","Miss","Kitty","Colonel","Lady","How","Sir","Hertfordshire","Had","Derbyshire","Mamma","God","Esq","Lakes","March","Between","Dear","Pray","Hill","Lord","Long","Heaven","Poor","Madam","Epsom","Console","Scotch","Militia","God","Dearest","Park",'“which'`

I have also identified that some of the characters are identified as different characters when they are infact one and the same. For example "Elizabeth Bennet" and "Miss Bennet" are identified as two separate characters. I have identified such nodes in the gephi and merged them before generating the graph.

After removing these words from the corpus, I have generated the gml for the book.
![Pride and Prejudice](https://github.com/njetty/B669-Final-Project/blob/master/pnp.png)

#### Extra Credit Option 2:
As part of the Extra Credit Option 2, I have created a data capsule in the Hathi-Trust. Below are the problems that I have faced while working with a data capsule.

1. The creation of data capsule is erratic, most of the times during the initial Starting, the VM's state goes to error and stays like that. I had to delete the capsule and recreate this.
2. When trying to set up the environment for the book project, the disk space ran out crashing the system. I had to remove some of the installed modules as part of Anaconda to facilitate my environment setup.
3. When I switched to secure mode and wanted to switch back to Maintenance mode, the VM went in to error state and stayed like that, I was not able to access the VM. I had to delete the capsule and re-do the entire process.
4. Sometimes the capsule though accessible is not created properly, some of the system commands were not accessible to me occasionally. 

I am currently trying to run the project in the secure mode but due to above limitation the process is still ongoing. 

#### Links to PDF Files:
[Les Miserables](https://github.com/njetty/B669-Final-Project/blob/master/les.pdf)
[Pride and Prejudice](https://github.com/njetty/B669-Final-Project/blob/master/PNP3.pdf)

#### References:
[1] [Networkx Tutorial](https://networkx.readthedocs.io/en/stable/tutorial/index.html)

[2] [Gephi QuickStart](https://gephi.org/users/quick-start/)
