# task-5
# Sentiment analysis on Social Media Posts
    from textblob import TextBlob

    def fetch_tweets(query, count=10):
        print("Fetching tweets...")
        mock_tweets = [
            f"This is the positive tweet about {query}!",
            f"I don't like {query}.",
            f"{query} is okay, I guess.",
            f"I absolutely love {query}!",
            f"{query} makes me so angry!"
        ]
        return mock_tweets[:count]

    def analyze_sentiment(text):
        analysis = TextBlob(text)
        if analysis.sentiment.polarity > 0:
           return 'Positive'
        elif analysis.sentiment.polarity < 0:
           return 'Negative'
        else:
           return 'Neutral'

    def sentiment_analysis_pipeline(query):
        tweets = fetch_tweets(query)

        if not tweets:
           print("No tweets found or error occurred.")
           return

        print(f"\nAnalyzing sentiments for '{query}'...\n")
        for tweet in tweets:
            sentiment = analyze_sentiment(tweet)
            print(f"Tweet: {tweet}\nSentiment: {sentiment}\n")

# Execute the pipeline by directly calling the function
    topic = input("Enter a topic (or) hashtag to search tweets: ")
    sentiment_analysis_pipeline(topic)
