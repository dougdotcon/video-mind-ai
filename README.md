# VideoMind AI

<div align="center">
  <img src="logo.png" alt="VideoMind AI Logo" width="200"/>
</div>

An advanced automation solution for creating YouTube Shorts video content using Artificial Intelligence.

## About the Project

VideoMind AI is an automation tool developed in Node.js that revolutionizes the content creation process for YouTube Shorts. Through the integration of cutting-edge AI technologies, the system automates the entire production pipeline, from script generation to video publishing.

Detailed article about the project: [Automating Content Generation on YouTube with Artificial Intelligence and Programming](https://medium.com/@thiagobergamig/automatizando-a-gera%C3%A7%C3%A3o-de-conte%C3%BAdo-no-youtube-com-intelig%C3%AAncia-artificial-e-programa%C3%A7%C3%A3o-f50f095d0e70)

## Key Features

### 1. Automated Script Generation
- Utilization of ChatGPT-4 for creating optimized scripts
- Contextual analysis to ensure content relevance
- Automatic adaptation for the Shorts format

### 2. Advanced Voice Synthesis
- Integration with Google Cloud Text-to-Speech
- Support for multiple languages and accents
- Control over intonation and speech rate
- High-quality audio processing

### 3. Professional Video Processing
- Automated editing using FFmpeg
- Robust scene composition system
- Support for multiple input formats
- Optimization for vertical format (9:16)
- Precise control over quality and compression

### 4. Captioning System
- Automatic caption generation via CapCut
- Precise synchronization with audio
- Customizable caption styles
- Support for multiple languages

### 5. SEO Optimization
- Intelligent description generation with ChatGPT-4
- Trend analysis for keywords
- Optimization of titles and tags
- Compliance with YouTube best practices

## System Requirements

### Software
- Node.js 16.x or higher
- FFmpeg 4.x or higher
- CapCut (latest version)
- Active Google Cloud Platform account
- Access to the ChatGPT-4 API

### Recommended Hardware
- Processor: Intel i5/AMD Ryzen 5 or higher
- RAM Memory: 8GB minimum (16GB recommended)
- Storage: SSD with 256GB of free space
- Internet Connection: 10Mbps or higher

## Project Structure


src/
├── audio/
│   └── audio.js         # Audio processing
├── chatGPT/
│   ├── chatGPT.js      # ChatGPT integration
│   └── longText.js      # Long text processing
├── video/
│   ├── cropVideo.js     # Video cropping
│   ├── editVideo.js     # Main editing
│   └── joinVideo.js     # Final composition
└── index.js             # Entry point


## Installation

1. Clone the repository:
bash
git clone https://github.com/seu-usuario/videomind-ai.git
cd videomind-ai


2. Install dependencies:
bash
npm install


3. Configure environment variables:
bash
cp .env.example .env
# Edit the .env file with your credentials
