# Description: 
To extract user problems of the app. Basically reasons behind negative feedback of the app.

# DataSet: 
https://drive.google.com/file/d/1_IoMrZYQCm0OymtViK-Xh04Sp6uxYDxw/view?usp=sharing

# Set up: 
$ pip install numpy

$ pip install pandas

$ pip install matplotlib

$ pip install seaborn

$ pip install --user -U nltk

$ pip install -U scikit-learn


# Technique Used, Data Cleaning and Further Analysis:

Used *WordCloud* technique in python library [*a data visualization technique used for representing text data* *in which the size of each word indicates its frequency or importance*] to extract most frequent words/feedback given by users.   

1. Primarily cleaned the data.

    - Feedback contains lot of emoticons, null values, stopwords, links, etc.
    
2. Divided the data into training[90%] and testing[10%] .

3. Further categorised the **training data** according to NPS score, screen type and view type.

         I. Promoters, NPS score 9,10.  

         II. Passives, NPS score 7,8.        

         III. Detractors, NPS score ≤6.     

4. Further dividing the detractors data meaning less NPS score feedback into 4 parts to deeply    
[To analyse the most frequent negative feedbacks** given by users.] 
Those 4 parts are:-

NPS score ≤4, NPS score ≤3, NPS score ≤2 & NPS score =1

    I. Promoters and Detractors for different screen type i.e. submit_assignment / end_lecture / finish_test / add_lecture.
    
    II. View Type i.e. student/teacher. 
    
5. For each 5 categories trained the data. Thereafter, Plotted WordCloud and fetched frequent words in each category.

6. Lastly listed down the frequent feedbacks received by users for respective screen type and over all."



*NPS is mostly collected through the Lecture feedback screen. Since maximum engagement is through the lecture, this is intuitive.*

### Feedback given mostly when the screen is end_lecture
Bad network, connection breaking, shows waiting on the screen(network issue)
camera issue,

### Feedback given mostly when the screen is submit_assignment
lag and upload issue, slow, uploading issue.

### For all screens and view_type
many glitches,

### Suggestions
Fix message and chat issue and improve heavy data consumption.
