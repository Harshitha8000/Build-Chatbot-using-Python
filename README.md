# Build-Chatbot-using-Python

This is a working chatbot build by using python. This chatbot is used for interacting with basic greeting we use in daily life.


Example Conversation using Chatbot:


Chatbot: Hello, How can I help you?
User: Hi
Chatbot: Hi there!
User: What is your name?
Chatbot: I'm a chatbot!
User: Bye
Chatbot: Goodbye!



Working of Chatbot:


1. Text Preprocessing

Remove punctuation (like , . ! ?).
Convert to lowercase.
Tokenize text (split into words).
Lemmatize words (reduce “running” → “run”).
Remove stopwords (like is, the, at) – optional, commented in your code.
Clean and normalize user input before sending it to the model.

2. AI-Powered Chatbot (ML based)

CountVectorizer + Multinomial Naive Bayes (scikit-learn).
Training data → sample phrases like “hello”, “bye”, “thanks”.
Responses mapped → “Hi there!”, “Goodbye!”, “You’re welcome!”.
Pipeline created:   [Text → Vectorizer → Naive Bayes model → Predicted response]
When user types, model predicts the best response.

3. Rule-Based Chatbot (NLTK)

Uses nltk.chat.util.Chat and pattern–response pairs (pairs list).

Example:
Pattern: "hi|hello|hey"
Responses: ["Hello, how can I help you?", "Hey there!"]
Works like a regular expression matcher — if user input matches, a predefined response is returned.

4. Main Loop

Keeps asking user for input.
Preprocesses input.
If exit, stops.
Else → passes input to AI chatbot → prints response.


