
# Audio Watermarking System

A digital audio watermarking system designed to embed and extract hidden messages in audio files for copyright protection and ownership identification. The project combines Python-based audio processing with a web-based interface built using HTML, CSS, and JavaScript.

## Features

- **Watermark Embedding:** Embeds a text message into audio using Quantization Index Modulation (QIM).
- **Blind Extraction:** Extracts the embedded message without requiring the original audio file.
- **Frequency-Based Processing:** Uses selected mid-frequency components (4–12 kHz) for watermark embedding.
- **Audio Quality Analysis:** Evaluates the quality of watermarked audio using Signal-to-Noise Ratio (SNR).
- **Robustness Testing:** Tests watermark extraction under different conditions, including:
  - Additive White Gaussian Noise (AWGN)
  - MP3 compression
  - Low-pass filtering
  - Resampling
  - Audio cropping
- **Performance Evaluation:** Uses Bit Error Rate (BER) to measure watermark extraction accuracy.
- **Interactive Web Interface:** Provides an interface for audio upload, watermark processing, extraction, and performance visualization.

## Technologies Used

- **Programming:** Python
- **Web Interface:** HTML, CSS, JavaScript
- **Audio Processing:** NumPy, SciPy
- **Visualization:** Matplotlib

## Working Principle

1. Upload an audio file through the web interface.
2. Enter the text message to be embedded.
3. The audio is divided into frames and processed in the frequency domain.
4. QIM is used to embed the message bits into selected frequency components.
5. The modified audio is reconstructed and saved as a watermarked audio file.
6. The embedded message can later be extracted without the original audio.
7. SNR and BER are used to evaluate audio quality and extraction accuracy.

## Evaluation

The system is evaluated based on:

- **Imperceptibility:** How well the original audio quality is preserved after watermark embedding.
- **Extraction Accuracy:** How accurately the embedded message is recovered.
- **Robustness:** How well the watermark survives common audio processing operations and attacks.

## Project Objective

To develop an audio watermarking system that provides reliable message embedding and extraction while maintaining audio quality and offering an easy-to-use web interface.
