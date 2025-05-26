# YouTube Downloader - Video & Audio Chrome Extension with Python Backend

A simple and user-friendly Chrome extension that allows users to download YouTube videos or audio directly to their desktop. The extension communicates with a Python Flask backend that uses `yt-dlp` to process the download requests.

## Features
- **Download YouTube videos** in MP4 format.
- **Download YouTube audio** as MP3 files.
- User can **enter a custom filename** for the downloaded file.
- Simple and clean user interface.
- Communicates with a local Python Flask backend via REST API.
- Saves files directly to the user’s desktop.
- CORS enabled backend for easy extension communication.

## How It Works
1. The user enters a YouTube video URL into the extension.
2. The user selects whether to download video or audio.
3. The user specifies a file name or uses the default.
4. The extension sends a request to the Python Flask backend.
5. The backend uses `yt-dlp` to download the requested content.
6. The downloaded file is saved on the user’s desktop.
7. The extension displays the download status.

## Prerequisites
- Python 3.x
- Flask (`pip install flask flask-cors yt-dlp`)
- Chrome browser
- [FFmpeg](https://ffmpeg.org/) installed and added to system PATH (required for audio extraction)

## Installation & Usage

### Backend Setup
1. Clone this repository.
2. Navigate to the backend folder or project root.
3. Run the Python backend:
   ```bash
   python app.py
