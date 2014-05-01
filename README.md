First Exercise (Callacks & EventEmitter Patterns)
=================================================

Please complete the following steps:
 
1. Create a TCP server which accepts input lines, and processes a sentiment score for each line. You will have to split line data to **letters only words**, and the score will be the sum of all words rates, based on AFINN lexicone. The calculated score should be returned to the client - do the processing inside the **"data"** event handler.
2. Create a function named **"sentiment"**, which receives the data from the **"data"** event handler, and calculates the sentiment score.
3. Make your **"sentiment"** function acts as if it is asynchronous (**HINT: use a callback**)
4. Create a **"Sentimentor"** object, which inherits the Node base EventEmitter, and implements a **"process"** method for calculating the sentiment. This object should emit a **"sentiment"** event with the calculated score
5. Now make your server return a score only for the first input line


#####Use the AFINN.json in this repository for the score calculations
#####*You can also use the boilerplate index.js as a staring point for your server code*

