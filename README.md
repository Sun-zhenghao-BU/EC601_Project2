# EC601_Project2

## Zhenghao Sun 

### 1.Introduction

The aim of this project is to call Google's natural language processing API to perform sentiment analysis on text, including the overall sentiment
tendency of the text and the overall intensity of the sentiment in the text. The text used is taken from various movie clips. I will use these movie line
clips to test the API which I use.

### 2.Qucik Start
- Follow this instruction link of Google cloud to quick start and register your account
(https://cloud.google.com/natural-language)

- To run the code, you should download the all the file and in the terminal, Type：

```
python3 sentiment_analysis.py reviews/filename.txt
```
&emsp;&emsp; Replace filename.txt with the text file you want to test

### 3.MVP and User story
- ***User***:  
Consultant, Advisors, Project Manager

- ***Mission***:   
Use entity analysis to find and tag fields in documents, including emails, chat conversations, and social media posts, and then perform
sentiment analysis to understand customer perceptions to gain valuable product and user experience insights. 

- ***MVP(Minimum Valuable Product)***:  
This system can analyze the emotional tendency of each sentence in the text, and then combine the emotional intensity and emotional direction of each
sentence to determine the emotional state of the entire text creator.

- ***User stories***:  
For a legal consultant, product manager, etc. who needs to communicate with customers, when they receive emails from customers or when customers 
communicate with them, they need a sentiment analysis system to help them comprehensively understand customers' emotions and perceptions, andthrough
aggregation, they can obtain practical solutions to further enhance the user experience. This can better think from the user's point of view
and facilitate practitioners to solve problems more efficiently.

### 4.Example show
- ***Interpreting Sentiment Analysis Values***:  
The sentiment score of a document indicates the overall sentiment of the document. The magnitude of a
document's sentiment indicates how much emotional content is present in the document, and this value is usually proportional to the length of the
document.Be sure to use magnitude values to adjust your scores when comparing documents to each other, as they can help measure the amount of relevant 
emotional content.

<img width="691" alt="pic1" src="https://user-images.githubusercontent.com/103909747/196258435-5a5d657f-0371-4947-a0b0-9cefba80f071.png">

- ***Test Sample***:  
I chose the text of lines from *Bladerunner*, both ends of the movie as the detection dataset, and the lines reflect negative emotions. Test Sample will be shown below.

<img width="384" alt="pic2" src="https://user-images.githubusercontent.com/103909747/196258554-43cbe938-29db-4629-8d27-4d42e8cb9250.png">

<img width="789" alt="pic5" src="https://user-images.githubusercontent.com/103909747/196258603-828b26a9-e44a-4147-afeb-e55d9b7d57f4.png">

In the case of the negative text, we can clearly and intuitively understand the meaning of several parameters: the emotional attitude of each sentence 
ispositive or negative from the score, and after each sentence is analyzed, we can see the final sentiment value and emotional fullness of the 
paragraph.The results show that the text has a score of -0.7 and a magnitude of 3.7, which means this text is clearly negative and relatively full of 
emotion.

---------

- ***Using Result***:  
We will try to use some other .txt file to analyze the sentiment status and emotional fullness and evaluate the accuracy of this system we have implemented. Using sample will be shown below.

<img width="661" alt="pic7" src="https://user-images.githubusercontent.com/103909747/196258677-71418972-e256-4150-a7a0-77027d33e27c.png">

It is easy to find that the emotional fullness of this test is highly passionate and the tendency of this text is inclined to positive. Now, we need to prove that whether the result of this using sample is identical to what we have feeled from this text.

------

<img width="763" alt="pic6" src="https://user-images.githubusercontent.com/103909747/196258706-b899fad7-adf4-4a4a-b784-99f88ff3e676.png">

Obivously, score is 0.3 and magnitude of this text is 10, which is almost the same result as we predicted before.
