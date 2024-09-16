## AI-Powered Negotiation Chatbot: Dynamic Pricing and Sentiment-Driven Interactions Using LangChain and Hugging Face ##

Integration Documentation: Sentiment Analysis Model in Negotiation Chatbot

### 1. Model Selection ###

The sentiment analysis model used in this integration is the distilbert-base-uncased-finetuned-sst-2-english model from the Hugging Face Transformers library. This model is a fine-tuned version of the DistilBERT model, which is a smaller and more efficient version of the BERT model. The model is trained on the SST-2 dataset, which is a popular dataset for sentiment analysis tasks.


### 2. Model Integration ###

#### 1. **Model Loading** : 
The model is loaded using the pipeline function from the Transformers library, which provides a simple way to load and use pre-trained models.

#### 2. **Model Configuration**: 
The model is configured to use the sentiment-analysis task, which is the default task for the distilbert-base-uncased-finetuned-sst-2-english model.

#### 3. **Model Input**: 
The user's input is passed to the model as a string, which is then analyzed by the model to determine the sentiment.

#### 4. **Model Output**: 
The model output is a dictionary containing the sentiment label and score. The sentiment label is used to determine the chatbot's response.
Chatbot Logic

#### The chatbot logic is implemented using a combination of conditional statements and functions. The chatbot's response is determined based on the user's input and the sentiment analysis output. The chatbot's logic is as follows:

**Positive Sentiment**: If the user's sentiment is positive, the chatbot offers a discount and adjusts the price accordingly.

**Neutral Sentiment**: If the user's sentiment is neutral, the chatbot continues with the normal negotiation process.

**Negative Sentiment**: If the user's sentiment is negative, the chatbot responds defensively and raises the price.


### 3. Conclusion: ###

The integration of the sentiment analysis model in the negotiation chatbot enables the chatbot to respond to users in a more human-like way, taking into account the user's sentiment and tone. The model is used to analyze the user's input and adjust the chatbot's response accordingly, providing a more personalized and engaging experience for the user.
