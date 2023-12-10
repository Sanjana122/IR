# IR
Drug and Medicine related search
PROJECT NAME : Drug and Medicine related search

project description:
	Users will have some queries realted to drugs and medicine. 
   When we give query we will get some description and url to know more info about it.

Group members:
	1.THATIKONDA SANJANA  --> S20210010228
	2.SHYAM BHASKAR       --> S20210010035
	
Dataset Link:

https://github.com/Sanjana122/IR
    
How to run:
  1.unzip the file
  2.go to the current folder IR_PROJECT
  3.type on console : python app.py
  
Dirve link contains:
  codes [app.py]
  index.html

Components:

1. Indexing:
   We take the all documents and create a dictionary ,keys are the all unique words and posting list is document ID and frequency of that word in that document.
2. Searching:
   We calculate the tf and idf values and assign the weights to the each document by creating vector.Similarly find vector to query,now find the similarity between query and each document by using cosine similarity ,based on that we rank the document and return the top 10 document.Here we used the trie data structure for faster retrieval.
3. Refining searches based on specific filters:
   a. Search based on drugs
      We search the documents based on the durgs of each document ,if user enter something realted to drug we return the top 10 documents based on the entered query and similarity of that document
   b. Search based on medicine 
      We search the documents based on something related to medicine,if user enter any query we return the documents related to that particular query.
4. Capturing Feedback:
   By taking the relevance feedback from user,we find the new query 
   after geting new query we find cosine similarity between the new query and each document and return the top 10 documents
5. Assessment Components:
   We calculate the Precison , Recall and avgP and plot graph of Precison and Recall

Contribution:
	
     1.THATIKONDA SANJANA  -->  Web crawling for Data collection
                                Data Cleaning and extracting only needed information
                                Inverted Index construction
                                Ranking
                                User interface

     2.SHYAM BHASKAR       --> Inverted index in tries for faster retrieval 
                               Spell correction using Levenshtein Distance 
                               Relevance Feedback and Re-Ranking
                               Evaluation

Note: 
The time taken to search a query depends on posting list size. If it is small sized query then it retrieves in less time.
Else it takes the intersection of posting lists so takes little more time.
One word -> less than 20sec 
3 or more words -> around a min - 2 mins

