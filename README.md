# ST311 Group 11: Project Improving sentiment analysis through use of image and audio data

### Contributors
  - 51126 
  - 38134
  - 42159
  - 44766

## Abstract
Traditional sentiment analysis typically relies on text alone, an approach which has limitations. In this paper, we explore multimodal sentiment analysis, inte- grating text, audio, and image data to enhance emotion detection accuracy. Our proposed model uses RoBERTa for textual sentiment analysis, a custom CNN for facial emotion recognition from images, and a fine-tuned Wav2Vec2 model for vo- cal emotion cues from audio. We use a late fusion strategy to combine predictions from all all three models based on the length of the input clip. Despite challenges in dataset availability and model integration, our experiments demonstrate that multimodal analysis outperforms single-modal approaches in sentiment classifi- cation, encouraging further use of multimodal approaches to sentiment analysis.

