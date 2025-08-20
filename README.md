# Airline AI Assistant

## Overview
AI Customer Support assistant for an Airline, designed to answer customer queries with short, courteous, and accurate responses using OpenAI's GPT models.

## Technologies Used
- Jupyter Notebook
- Python
- OpenAI API (gpt-4o-mini)
- Gradio (for chat UI)
- dotenv (for environment variable management)

## How to Run
1. Ensure you have an OpenAI API key set in your environment as `OPENAI_API_KEY`.
2. Install required Python packages: `openai`, `gradio`, `python-dotenv`.
3. Run the notebook to launch a local Gradio chat interface for customer interactions.

## Ticket Price Tool
- The assistant uses a custom function to provide ticket prices for destinations like London, Paris, Tokyo, Berlin, and Lisbon.
- When a user asks for a ticket price, the tool is invoked to fetch the correct price.

## Example
- Chat interface launches at `http://127.0.0.1:7870`, allowing users to ask questions such as "How much is a ticket to Paris?"
- Screenshot examples are included in the notebook to demonstrate usage.

## Features
- Accurate, concise responses
- Tool integration for real-time ticket pricing
- Easy extension for more tools or APIs

---