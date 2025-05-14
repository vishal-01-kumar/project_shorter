📘 Project Overview
This project is a YouTube video processing pipeline that automates the conversion of video content into summarized, translated, and speech-enabled outputs. Designed for educational or informational videos, the system extracts the transcript, summarizes the key points, analyzes sentiment, and generates multilingual audio versions — making video content more accessible and efficient to consume.

🔧 Features
YouTube Transcript Extraction
Uses youtube_transcript_api to fetch the transcript directly from a YouTube video link.

Text Summarization
Applies Hugging Face’s transformers summarization pipeline to condense lengthy transcripts into key insights.

Translation
Translates the summarized text into a target language (e.g., Hindi) using the googletrans API.

Text-to-Speech (TTS)
Converts translated summaries into speech using Google Text-to-Speech (gTTS), producing audio files for playback or download.

Sentiment Analysis
Uses both VADER and Transformer-based models to evaluate the sentiment of the summarized content, categorizing it into positive, negative, and neutral segments.

Audio Outputs for Sentiment Segments
Each sentiment category can be converted into separate audio files, making it easier to understand tone and emotion.

Performance Evaluation
Includes optional BERTScore evaluation to compare the quality of generated summaries against reference summaries.

🚀 Use Cases
Create quick, summarized audio versions of long YouTube educational videos.

Make video content accessible in different languages.

Analyze sentiment from thought leadership or review-based content.

Generate audio content for users with visual impairments.

📦 Requirements
This project uses the following Python libraries:

transformers

torch

gtts

googletrans==4.0.0-rc1

youtube_transcript_api

pytube

vaderSentiment

nltk

bert_score

📝 How It Works
Input: Provide a YouTube video link.

Transcript: Extract text from the video.

Summarize: Use NLP models to condense the transcript.

Translate (optional): Convert summary into another language.

Sentiment Analysis (optional): Detect sentiment in text.

TTS: Convert any text (original, translated, or sentiment-filtered) into speech.

Output: Play or download audio summaries.
