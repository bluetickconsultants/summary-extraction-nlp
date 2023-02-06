<h1> Summary Extraction of News Articles </h1>
<hr>

<img src="/Summary Extraction/Images/s1.png" width="700" height="400">

<hr>

For Summary extraction from the News Articles we are usin a Library called nwewspaper3k . Where we can collect the urls of the article and collect the text 

<hr> 

<h2> Implementation </h2> 

Using newspaper3k collected the articles url and and using the same library colleted entire text of the article . From the text for collecting the summary used a library called spacy . 

with the help of spacy the collected text and the individual words where given some importance based on there embedding vectors results and findiing the performance of each word  compare to the entire length . By doing this technique we can collect the probability percentage of text as a summary .

<hr> 

<h2> REGEX </h2>

<img src="/Summary Extraction/Images/s2.jpg" width="700" height="400">
<hr> 

Using regex I just clean the data .using meta characters and spatial sequential for cleaning purpose 

<h3> Meta characters </h3> 

                          1 . [] -> returns a match if contains patterns / character specified in []
                          2 . ^ -> string starts with given patterns 
                          3 . $ -> ends with 
                          4 . . -> any character except new line 
                          5 . * -> Zero or more occurences 
                          6 . + -> one or more occurences 
                          7 . {} -> specified number of occurences 

                          

<h3> special sequences </h3> 

                            1 . \d -> if a given string has digits (0-9)
                            2 . \D -> if the given string does not have strings
                            3 . \w -> if a given string has word characters(a-z,A-Z,0-9)
                            4 . \W -> if a given string does not have word characters
                            5 . \s -> if given string has spaces
                            6 . \S -> if given string has no spaces

                         

<p> Techniques used for cleaning </P> 


                         1 . Removing unwanted Punctuation for the text
                         2 . Removing URLS from the text 
                         3 . Removing hashtags 
                         4 . Removing Extra white spaces 
                         5 . Lowering the text 
                         6 . removing the own mentions 
                      

                         
<h2> Deployment using Flask </h2> 

link = https://spacy-data-extraction.herokuapp.com/
