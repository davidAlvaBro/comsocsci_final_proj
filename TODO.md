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