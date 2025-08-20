# Airline AI Assistant

## Overview
AI Customer Support assistant for an Airline, designed to answer customer queries with short, courteous, and accurate responses using OpenAI's GPT models. Now with multi-modal support for images and audio!

## Technologies Used
- Jupyter Notebook
- Python
- OpenAI API (gpt-4o-mini, DALL-E-3 for images, speech/audio)
- Gradio (for chat UI)
- dotenv (for environment variable management)
- PIL (Python Imaging Library for image handling)
- ffmpeg (for audio processing)

## How to Run
1. Ensure you have an OpenAI API key set in your environment as `OPENAI_API_KEY`.
2. Install required Python packages: `openai`, `gradio`, `python-dotenv`, `Pillow`.
3. For audio features, ensure `ffmpeg` is installed on your system.
4. Run the notebook to launch a local Gradio chat interface for customer interactions.

## Features

### Core Assistant
- Accurate, concise answers to airline customer support queries
- Tool integration for real-time ticket pricing (London, Paris, Tokyo, Berlin, Lisbon)
- Simple AI assistant for booking airline tickets

### Multi-modal Support
- **Image Generation**: Uses DALL-E-3 to generate vacation images for destination cities.
    - Example: The function `artist(city)` generates and displays an image for a given city.
- **Audio Responses**: Uses OpenAI's speech API to provide audio responses to text queries.
    - Example: The function `talker` converts text answers into spoken audio.

### Usage Example
- Chat interface launches at `http://127.0.0.1:7870`, allowing users to ask questions, request ticket prices, book tickets, or get images/audio for destinations.
- Example cell:
    ```python
    image = artist("New York City")
    display(image)
    ```
- For audio:
    ```python
    talker("Your ticket to Paris is booked!")
    ```

### Screenshots & Media
- See notebook cells for examples of image and audio outputs.

## Extending
- Easily add more cities, tools, or APIs for further features.
