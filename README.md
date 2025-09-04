# Customer_support_analyzer

## Transcription
Obtaining a transcription for sample_customer_call.wav file using SpeechRecognition class from google, with its record function 

## Audio Stats
Obtained audio stats of the sample_customer_call.wav file using pydub with its AudioSegment class with its from_file function

## Sentiment Analysis
The classify_sentiment function uses SentimentIntensityAnalyzer class from Natural Language Toolkit to perform sentiment analysis on transcriptions from the customer_call_transcriptions.csv with a threshhold ranging from 0.05 and -0.05

## Frequent Entities
Obtained the most frequent entity and saved it as most_freq_ent by leveraging spaCy while using the small English model ('en_core_web_sm') to extract named entities from each text in the dataframe.
Got the entity counts for each entity after using Counter class from collections package and saved the entity with the highest entity count in the variable most_freq_ent

## Similarity
Obtained the most similar call from the dataframe to the query, 'wrong package delivery'.
Used spaCy's small English model with its similarity_score method to provide similarity scores to each text in the dataframe
Obtained the text of the transcription with the highest similarity score
