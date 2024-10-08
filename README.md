# x_fake_news_community_notes

I heard of the topic called as x (formerly twitter) fake news detection and was intrigued by it so I decided on reading it with little to no knowledge of ML.

As an ML beginner I had an idea which seemed fine at start but I thought that I could add community notes data given by X themselves and maybe improve and existing model.

So at first I decided to just collect such and metrics needed that could be added to a GNN model which as a beginner I found it as a pretty doable task as there was code given for it along with research

Data collection took a while but I will be trying out differnt ways to use the additional data given by X in their tsv files to first atleast make this model work.

Implementing a very basic train and test at the moment.


Dataset I got from x itself https://communitynotes.x.com/guide/en/under-the-hood/download-data which had tweet IDs which helped me get the rest of the dataset from.

We have used only ~1500 tweets as of now for basic implementation, this can be found in our repository.

Something new that we tried in this attempt was to not include which user spread more fake news over the course of time. 5 features were used in the graph with ~1500 nodes. The nodes were the tweetID which makes each node unique which is better for a graph model. Community notes can be added in the model in many ways but for now it has been added as agreement/ disagreement from the original tweet. GNN Model was used for implementation. Comments added by chatGPT for better understanding.

To see implementation just run the notebook file on system after installing the required libraries(as mentioned in the repository).
