# chatbot
create chatbot to scan news articles with scrapper and answer to given questions regarding the news

On this given code i created a chatbot which takes news urls , extract the html structure of the website by using beutiful soup and testing many html structures to find the one that returns the most data (since not all websites have the same html structure)
It saves then the retrieved articles info in a data frame with features (Title of the article , link of the article , summary of the article)
It creates a pre process function to pre process text 
Then i extract the complete text of the article and i run it through the pre process function 
After that i have the complete processed text of the article in my dataframe and i perform LDA to split the articles into different 
topics ,for the lda i perform hyperparameter tuning to find the optimal number of topics to split the articles by using clustering and coherence score 
Then i Creates a chatbot using TF-IDF and  LDA model's topic assignments
I use tf-idf to perform word embedding for the process text and the given question 
then by doing cosine similarity i find the nearest topic th assign the question


