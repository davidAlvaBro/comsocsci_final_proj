# TODO list for content 
## Idea 
- Find social trends in which books people read
- Social vs NLP analysis

## Data 
- Where do we get the data from
    - Like the slides: Goodreads and random guy 
    - Specs (All the sizes)
    - Biases?! 

## Preprocessing 
- Collect datasets into one 
    - Match titles of books 
    - Clean dataset from duplicates and the likes 

## Preprocessing II - Generate networks 
- Shelves network 
    - Choice of weighting of edges
    - Chose threshhold 
    - Use NetworkX to create network
- TL-IDF 
    - Generate TL-IDF scores for each book
    - And for each Genre 
    - Chose top genre for each book with TF-IDF 
    - Make edges with TF-IDF inner products (normalized)
    - Generate network to have as many edges as the shelves one 

## Network Analysis 
- Communities 
    - Louvain to create networks
    - Check modularity to know if we form communities
    - Compare communities from the networks, and the genres
        - Create confusion matrices (do they find the same?)

- Assortativity 
    - Assortativity between genres 
    - Assortativity for degree? 

## NLP Analysis 
- Create word clouds for communities 

## Conclusion 
- Shelves better decides genre in communities 















# TODO tomorrow 
- Look at conclusions together. 
    - Confusion matrices 
    - Assortativity 
    - Views of network 
    - Word Clouds 

- Use one genre at a time to see if the confusion matrices look better? 
- Use assortativity with all genres of each book together - How? do we need to write our own assortativity function? 

- Should we really have the degree assortativity included? 
    - If yes choose which one we put in the code 

- Why are the communities pickle files? 

- two todoes in mixing matrix 
    - Seb write some comments 






# BODY
Look at section Create Graph under Shelf Graph - Body messing around with comments. 

- Calculate assortativity
    - Genre
    - Degrees
- Get largest sub network
- Create communities
    - Color according to genre