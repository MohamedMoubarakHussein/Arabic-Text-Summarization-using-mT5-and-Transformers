# Intro

Text summarization (Abstractive Summary)
We use the latest technology (state-of-the-art technique) for the Text summarization. 
This project involves building a text summarization model using the google/mt5-small model from Hugging Face’s transformers library.
We will be fine-tuning a transformer model for Summarization Task. a summary of a given article/document is generated when passed through a network.


# Dataset
<br>
we use  a small chunk of **Wikihow Dataset** ("Not cleaned dataset for Arabic lang")<br>
and we tried to clean it  .<br>
we used "300" articles for our model <br>
The link to the whole dataset<br>
https://drive.google.com/file/d/1PM7GFCy2gJL1WHqQz1dzqIDIEN6kfRoi/view<br>
we will upload our cleaned chunk of a dataset that contains **11k** articles to the dataset folder <br>
but we used only **300** because it will take a huge time to train in collab with **300** it takes 1 hour<br>


# used technique 
we used pytocrh for converting our data to a More interesting style to work with the network (First using pytorch.Dataset model to convert it<br>
to something that can the Dataloader use . dataloader used to keep a small chunk of our data in the ram not to load all data in the ram  )<br>
and we fine-tuning(mt5 model ) using  T5Tokenizer , MT5ForConditionalGeneration <br>
and we use a dashboard to keep track of our model config and log called wands.


# Very important Note

We forget to train our model and when we tried to train it yestardey it took 2 hour to just train 30 artical
so we closed the training step but we belive the code work will if there are a resources and alote of time to optimaze(we
used adam which is very slow)



