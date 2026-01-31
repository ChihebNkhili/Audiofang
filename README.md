# AudioFang - Advanced Audio Mixer

AudioFang is a professional audio mixing application with voice-activated auto-ducking, YouTube audio downloading, and real-time audio processing capabilities. Perfect for streamers, podcasters, and content creators.

## Features

- **Smart Auto-Ducking**: Voice-activated music ducking (music volume drops to 0.5% when speaking)
- **YouTube Integration**: Download audio directly from YouTube videos
- **Virtual Audio Cable Support**: Route audio to applications like Discord, OBS, etc.
- **Multi-Channel Output**: Select specific output channels
- **Hotkey Support**: F1-F12 to control sounds
- **Real-time Monitoring**: Hear your mix while streaming
- **Auto-Updating**: yt-dlp automatically updates to bypass YouTube changes

## python install commands:
pip install -r requirements.txt

## Build the executable: 
pip install nuitka
nuitka --standalone --onefile --windows-console-mode=disable --enable-plugin=tk-inter --windows-icon-from-ico=Audiofang_icon.ico --include-data-file=Audiofang_icon.ico=Audiofang_icon.ico --output-filename=AudioFang.exe audiofang_youtube.py