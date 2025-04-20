# System For Video Content Moderation Using AI

This is a simple AI system for video content moderation which detects **Nudity, Kissing, Vulgar gesturing, and Profanity.** It identifies whether a given video is **SAFE** or **UNSAFE** by using Opening AI’s CLIP for visual examinations and Whisper for audio transcribing.

## Preparation Guide
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/video-content-moderator.git
   cd video-content-moderator
   ```
   Install the following:
   ```bash
   pip install git+https://github.com/openai/CLIP.git
   pip install openai-whisper moviepy opencv-python Pillow regex tqdm ffmpeg-python
   ```
   Recommended to run the script in Google Colab or prefered local with GPU.
   You will be prompted to upload your video. Do so.

### Results You Should Expect
- ***
Transcription of the Audio
- ***:
Unsafe Wards List (if detected)
- ***:
Unsafe preview frames (if flagged)
- ***:
Final decision:  SAFE /  UNSAFE

### Models Used
- OpenAI CLIP: 
Deters inappropriate visual elements such as nudity, gestures, and violence.
- OpenAI Whisper: 
Transcribes audio of the video to pick out foul and harmful language.
- Nsfw Model
  If there is any nudity, kissing scenes and violence 

### Example Prompts For CLIP
- “nudity”
- “a person showing a middle finger”
- “kissing scene”
- “graphic violence” 

### What It Flags
- Inappropriate video uttered based on CLIP confidence score. 
- Any of the abusive words from the audio transcript.
- Hand Gestures 

