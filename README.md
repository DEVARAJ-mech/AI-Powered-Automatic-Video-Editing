# AI-Powered Automatic Video Editing

## Overview
This project is an AI-powered automatic video editing system that enhances videos by adding subtitles, related images, and graphics. The system extracts speech text, generates AI-enhanced visuals, overlays graphics, applies smooth transitions, and produces a final processed video.

## Features
- **Speech-to-Text Conversion**: Extracts audio from video and generates subtitles.
- **AI-Generated Images**: Uses AI to generate relevant images based on speech content.
- **Graphics Overlay**: Adds text, icons, and other visual elements to enhance the video.
- **Smooth Transitions**: Applies AI-driven motion effects for seamless scene changes.
- **Final Processing**: Merges all components and exports the final edited video.

## Architecture
1. **Extract Speech Text**
    - Convert speech to text using AI models (Whisper, DeepSpeech, Google Speech-to-Text)
    - Generate and sync subtitles (SRT/VTT format)

2. **AI Enhancements**
    - NLP-based text enhancement (GPT-4, BERT)
    - AI-generated images using Stable Diffusion

3. **Overlay & Graphics**
    - Merge AI-generated images with video
    - Add dynamic graphics and text overlays

4. **AI Transitions**
    - Detect scene changes using OpenCV
    - Apply smooth motion effects

5. **Final Processing**
    - Merge video, subtitles, and graphics
    - Export the final processed video

## Tech Stack
- **Programming Languages**: Python
- **Video Processing**: FFmpeg, MoviePy, OpenCV
- **Speech-to-Text**: OpenAI Whisper, DeepSpeech
- **AI Image Generation**: Stable Diffusion, DALL·E
- **Natural Language Processing**: GPT-4, BERT
- **Machine Learning Frameworks**: PyTorch, TensorFlow

## Installation
### Prerequisites
Ensure you have the following installed:
- Python (>=3.8)
- FFmpeg (`sudo apt install ffmpeg`)
- Required Python libraries:
  ```sh
  pip install torch torchvision torchaudio whisper openai moviepy opencv-python transformers
  ```

### Running the Project
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/video-ai-editor.git
   cd video-ai-editor
   ```
2. Place your input video in the `input/` directory.
3. Run the main script:
   ```sh
   python main.py --input input/video.mp4 --output output/edited_video.mp4
   ```

## Future Enhancements
- Web-based UI for manual adjustments
- Real-time processing improvements
- Support for multi-language subtitles
- AI-based sentiment-driven video editing

## Contributing
Feel free to submit pull requests or open issues for improvements. Contributions are welcome!

