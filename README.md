# ST311 Group 11: Project Improving sentiment analysis through use of image and audio data

### Contributors
  - 51126 
  - 38134
  - 42159
  - 44766

## Abstract
Traditional sentiment analysis typically relies on text alone, an approach which has limitations. In this paper, we explore multimodal sentiment analysis, integrating text, audio, and image data to enhance emotion detection accuracy. Our proposed model uses RoBERTa for textual sentiment analysis, a custom CNN for facial emotion recognition from images, and a fine-tuned Wav2Vec2 model for vocal emotion cues from audio. We use a late fusion strategy to combine predictions from all all three models based on the length of the input clip. Despite challenges in dataset availability and model integration, our experiments demonstrate that multimodal analysis outperforms single-modal approaches in sentiment classification, encouraging further use of multimodal approaches to sentiment analysis.

# 🎭 Multimodal Sentiment Analysis

This repository contains all code and notebooks for our project on improving sentiment analysis using **text**, **audio**, and **image** data. We combine models from each modality to better detect human emotions.

---

## 📓 Notebooks

The project is structured across the following Jupyter notebooks:

1. `Notebook1_CNN.ipynb`  
   - Trains a **Convolutional Neural Network (CNN)** to detect facial emotions from grayscale images (FER-2013 dataset).

2. `Notebook2_SpeechEmotion.ipynb`
   - Fine-tunes **Wav2Vec2** to classify emotions based on vocal tone and speech features.
   - Uses **RoBERTa**, a transformer model, to classify sentiment from transcribed speech.

3. `Notebook3_WhisperTuning.ipynb`  
   - Fine-tunes **Whisper Tiny**, an audio transcription model, on short emotional speech clips to improve text input quality for sentiment analysis.

4. `Notebook4_Combination.ipynb`  
   - Combines the outputs of all three models using a **late fusion strategy**.  
   - Evaluates the final model on **unseen audio/image/text clips** from real media.
