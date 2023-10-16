# WordCount for Named Entities
In this part, you will compute the word frequency for named entities in a large file. You are free to use any NLP library that works with Scala/PySpark. Some examples are:


### The steps of the assignment would be as follows:
1. Find a large text file from the Gutenberg project: https://www.gutenberg.org and upload it to your Databricks cluster.
2. Use a NLP library to extract only the named entities from the text.
3. Write code for a mapreduce program that performs wordcount on the extracted named entities.
4. The output from the map task should be in the form of (key, Value) where key is the named entity, and value is its count (i.e. once every time it occurs)
5. The output from the reducer should be sorted in descending order of count. That is, the named entity that is most frequent should appear at the top.


# Using NLTK Library
https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1909261951439895/2617178664973054/4943942562258491/latest.html

# Using Spacy Library
https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1909261951439895/2617178664973023/4943942562258491/latest.html
