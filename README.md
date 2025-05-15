# DiAna - Dialog Analyzer

## Overview
DiAna (Dialog Analyzer) is a comprehensive tool for analyzing conversations from YouTube videos. The project uses advanced speech recognition, speaker diarization, and sentiment analysis to provide detailed insights into dialogues.

## Team Members
[Mind Digger](https://github.com/Minddigger07)
George Joyal Vincent
Gouri S Govind
[St.Destiny](https://github.com/StDensity)

## Summarization Model
We developed a fine-tuned version of the DialogLED model, [StDestiny/DialogLED-base-16384-dialogsum-finetuned-10epochs](https://huggingface.co/StDestiny/DialogLED-base-16384-dialogsum-finetuned-10epochs), to deliver concise conversation summaries. Built on the Longformer-Encoder-Decoder (LED) framework, it leverages the base model ([MingZhong/DialogLED-base-16384](https://huggingface.co/MingZhong/DialogLED-base-16384)) with a 16,384-token input capacity from pre-training—perfect for tackling long dialogues. We fine-tuned this powerhouse on the DialogSum dataset for 10 epochs, sharpening its skills for our summarization needs.

## Features
- **YouTube Video Processing**: Download and extract audio from YouTube videos
- **Speech Recognition**: Transcribe audio to text using WhisperX
- **Speaker Diarization**: Identify and separate different speakers in the conversation
- **Sentiment Analysis**: Analyze emotions throughout the dialogue
- **Interactive Visualization**: View results through an intuitive Streamlit interface
- **Summary Generation**: Create concise summaries of lengthy conversations

## Technology Stack
- **WhisperX**: For high-quality speech recognition and alignment
- **Hugging Face Transformers**: For sentiment analysis and summarization
- **PyTube**: For YouTube video downloading
- **Streamlit**: For interactive web interface
- **Plotly**: For data visualization

## How It Works
1. The system downloads audio from a YouTube video
2. Audio is transcribed using WhisperX
3. Speaker diarization identifies different speakers
4. Sentiment analysis is performed on the transcript
5. Results are visualized through various charts and graphs
6. A summary of the conversation is generated

## Visualizations
- **Spoke When**: Shows who was speaking at different points in the video
- **Emotion Distribution**: Displays emotion scores throughout the video
- **Speaker-Level Analysis**: Provides emotion analysis for each speaker separately

## Use Cases
- **Content Analysis**: Understand the emotional tone of interviews or debates
- **Media Research**: Analyze speaking patterns in conversations
- **Accessibility**: Generate transcripts and summaries of video content
- **Educational**: Study conversation dynamics and emotional patterns

## Installation and Usage
The project is packaged as a Jupyter notebook that can be run in any environment supporting Python and the required libraries. The Streamlit interface makes it easy to interact with the analysis results.

## Future Improvements
- Support for more languages
- Real-time analysis capabilities
- Enhanced visualization options
- Integration with more video platforms

---

*This project was developed as a final project for our BTech degree program.*