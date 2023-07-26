# Voice Cloning with Translation Project

This repository contains code for a voice cloning project that combines Whisper (for translation) and Tortoise-TTS (for voice cloning). There are two sets of codes provided:

+-----------------------+ 
| Malayalam Audio input |
+-----------------------+

1. Fast Inference (Single Voice Cloning):
   - This code allows for faster inference but is only available for a single voice output.
   - It uses Whisper for translation and ttsmms for generating dubbed voice.
   - Use this for generating audio dubbings that are longer in duration.

2. Slow Inference (Multi-Voice Cloning):
   - This code provides cleaner and clearer cloned voices that mimic the sample vocal's characteristics.
   - It uses Whisper for translation, Tortoise-TTS for voice cloning, and also includes segmentation and segment combination steps.
   - Recommended for short audio clonings with very short text (less than 15 seconds) containing one or two lines.
   - The cloned voices produced with this method may take more time to generate, very long....
   - You can add custom audio samples to generate final cloned audio output.

## Colab Notebook

You can access the Colab notebook for this project at the following link:
[Click here to open the Colab notebook](https://colab.research.google.com/drive/1aEXat-hNhNDf9lqo4fWWDZIuTfBhCeuw#scrollTo=N3MDZG8ox_eF)

## Custom Voice Samples

To add your custom voice samples, follow these steps:
1. Add at least 3 sample audio WAV files of duration about 10 seconds each.
2. Name the WAV samples like `1.wav`, `2.wav`, `3.wav`, and so on.
3. Place the custom voice samples in the folder `/content/tortoise-tts/tortoise/voices` in the Colab environment.
4. Pre-made sample are for voices 'mol','tom','emma','angie','halle','geralt','daniel','deniro','william','freeman','applejack','tim_reynolds'

## Sample Results

Some of the generated audio results are saved in the `sample` folder. It contains subfolders named after the sample audios used to clone, and it also contains the generated audio results. 

audio_imax.wav is a malayalam audio clip used to make a synthetic voice using the fast inference method and the resultant audio is synthetic_speech.wav

other folders like chirag, hiddleston, patrick_stewart and vidu contains voice sample taken to clone their voice along with the generated cloned audio clip.

## GitHub Repository

You can find the full code and resources in the GitHub repository at the following link:
[Click here to visit the GitHub repository](https://github.com/AswanthManoj/voice_clone)
