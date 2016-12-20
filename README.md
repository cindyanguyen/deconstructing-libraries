# Deconstrucing Libraries
## Using Machine Learning Techniques to Analyze the United States Library of Congress Vietnamese Materials Collections
by Jordan Shedlock (University of California Berkeley, School of Information) 
jshedlock@ischool.berkeley.edu 

Cindy A. Nguyen (University of California Berkeley, History Department)
cindynguyen35@berkeley.edu

*Final project for 'Deconstrucing Data Science' course taught by Professor David Bamman at the UC Berkeley School of Information, Spring 2016.*

##Introduction
This project focuses on a complex non-English language historical data source--bibliographies of the United States Library of Congress collections of Vietnamese language materials from 1979-1985. We employ a dual approach to this project: a contextualized historical reading and machine learning methods to understand the language, political leanings, and content of the collections and how they change over time.

##Hypotheses
Focusing on a small slice of the research questions, we examine the relationship between the titles and their city of publication within the Library of Congress collections of Vietnamese language materials retrospectively collected up to 1979 and 1979-1985. We hypothesize that different publication locations will have different distribution of topics. 

To operationalize our hypothesis into a probabilistic problem, we ask the following question: ***What are the words in a title most characteristic of a publication city?***

Our hypotheses rest upon the important underlying assumption that a publication title can reveal important information about a work’s content, potential audience, and literary style. Although not a substitute for reading the entirety of the work, a work’s title reveals negotiated information between the author, the perceived audience, the publisher, and in this case, the library collection.

##Methods
We employed three methods of analysis:

1. Frequency Counts comparing works by publication city (Saigon, Hanoi), and Library of Congress Classification
2. Naive Bayes probability of word in title conditioned on city to understand the words in a title most characteristic of a publication city
3. Naive Bayes to predict an unknown city based on the words of a title
4. Permutation test to observe the most significant differences in words
5. MALLET Topic Models to learn patterns that suggest types of books from a publication city

##Data Cleanup
**Help us continue to clean up our data! For our project, we used Optical Character Recognition, Regular Expressions, Google Refine, and vnTokenizer to clean up our data set as much as possible to run our analysis. However, our data is far from perfect. To improve our analysis, results, and facilitate future projects with this important data set, help us improve the accuracy of the text data set.** 

*Example Mistakes in Need of Your Help*
* Vietnamese diacritics and misspellings from OCR output
* Incorect tokenization of Vietnamese words
* Incorrect categorization of values (Title, Author, Publication City, Library of Congress Classification label)

##Further Reading
* For the complete project report and conclusions, read the file "Shedlock_Nguyen_Final_Report-Updated-12-2016.pdf" and see slides "slides-updated-12-2016.pdf". 
* Blog Post description ["A Humanist does Data Science: Introduction to the 'Deconstructing Libraries' Project"](https://cindyanguyen.com/2016/12/02/a-humanist-does-data-science-deconstructing-libraries-project/#more-783)
* Deconstructing Data Science Course by Professor David Bamman [Website](http://courses.ischool.berkeley.edu/i290-dds/s16/) 
