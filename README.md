# Generative AI Meeting Assistant

A meeting assistant that transcribes audio using Whisper and uses a language model to generate a summary, key points, and action items.

## Overview

This project processes a meeting recording and extracts useful information from the conversation.

## Pipeline

```text
Meeting Audio
    ↓
Whisper
    ↓
Meeting Transcript
    ↓
Qwen LLM
    ↓
Summary + Key Points + Action Items
```

## Technologies

* Python
* OpenAI Whisper
* Hugging Face Transformers
* Qwen
* PyTorch

## Models

### Speech-to-Text

`openai-whisper`

Whisper is used to transcribe the meeting audio into text.

### Language Model

`Qwen/Qwen2.5-0.5B-Instruct`

Qwen is used to analyze the meeting transcript and generate:

* Meeting summary
* Key points
* Action items

## Dataset

The project uses an audio sample from the **AMI Meeting Corpus**.

A 3-minute segment from the meeting audio was used for the experiment.

## How to Run

1. Install the required libraries.
2. Open `generative-ai-meeting-assistant.ipynb`.
3. Run the notebook cells.
4. Load the meeting audio.
5. Transcribe the audio using Whisper.
6. Analyze the transcript using Qwen.
7. View the generated summary, key points, and action items.

## Project Structure

```text
generative-ai-meeting-assistant/
├── generative-ai-meeting-assistant.ipynb
└── README.md
```
