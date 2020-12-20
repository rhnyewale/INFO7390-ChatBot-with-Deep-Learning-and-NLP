# INFO7390-ChatBot-with-Deep-Learning-and-NLP
Creating ChatBot using Deep Learning and NLP

medium article - 

<Img src="https://github.com/rhnyewale/INFO7390-ChatBot-with-Deep-Learning-and-NLP/blob/main/Images/Bot.jpg?raw=true">


Dataset - Cornell Movie Corpus

The data set that we are going to use is the Cornell movie corpus. It's a data set of more than 600 movies containing thousands of conversations between lots of characters. We'll build a general chatbot that can have a general conversation with us like a friend, to talk about everyday life. Thats why movies are perfect because in movies you have a lot of random conversations, general conversations between friends. Our model can be trained on other more specific dataset like calender assistant or navigation assistant. These are some other applications of the chatbot.


## Plan of Attack

<Img src="https://github.com/rhnyewale/INFO7390-ChatBot-with-Deep-Learning-and-NLP/blob/main/Images/DataFlow.jpg?raw=true">

1. **Installation, setting up an environment, and getting the Dataset**<br/>
In Windows Anaconda Prompt, create a virtual environment named 'chatbot', where we'll install python 3.5 as there are some issues while executing with TensorFlow.
conda create -n chatbot python=3.5 anaconda<br/>
Activate the virtual environment 'chatbot'<br/>
conda activate chatbot<br/>
Open Anaconda Navigator and select 'chatbot' channel. Create a new python file in Spyder.<br/>
Dataset: Cornell Movie-Dialogs Corpus<br/>
Click on Zip File to download. After extracting the file, we'll need only two files- **movie_conversation.txt** and **movie_lines.txt**

2. **Data Preprocessing**
Data processing is inevitable whenever you build an AI or whenever you build a model you have to make the data set compatible with the model you're going to build. We're going to build a neural network-based model and therefore the data will have to have a special format especially for the inputs. Besides we'll have to clean the text because the less we clean it and simplify it the more difficult it will be for a model to train itself to talk like a human. So we'll have to do a lot of data processing and do it efficiently so that we can get to the exciting parts 3 & 4.

3. **Building the Seq2Seq model**
Part 3 and Part 4 are where we get into the heart of the model and speaking of these two parts, part 3 will be building the Seq2Seq model. We will actually build a brain composed of an encoder and then a decoder and we will assemble all of them to build the final brain which will not be trained yet.

4. **Training the Seq2Seq model**
Speaking of training that leads us to part 4 where we'll train this brain that we would have just made in part 3. So we'll train it, set up a loss function get the optimizer, and then apply some stochastic gradient descent to update the weights of the neurons of the brain so that it improves its ability to talk with us.

5. **Testing the Seq2Seq model**
And finally part for the last part of this implementation we will test our Chatbot which is we will test the Seq2Seq model. Once we execute we will have an interface where we can ask some questions and then the chatbot will answer and we will just test the chatbot by observing its answers and see how it's capable of conversing with us.


