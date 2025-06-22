# Booking_AI_PA using Fastapi and Gemini 1.5

This project is a basic agentic AI assistant that accepts user instructions like "Book my flight, hotel, and block calendar" and responds using Google's Gemini API. The backend is built using FastAPI and exposed via ngrok for use in Google Colab.

# Features

- Accepts natural language workflow queries
- Uses Gemini 1.5 Flash (Free) API
- Built with FastAPI
- Hosted via ngrok for public access in Colab

# Requirements

Install the required packages:
pip install fastapi uvicorn google-generativeai pyngrok nest_asyncio
# How to Run (Google Colab)

1. Clone or copy the code into a Colab notebook.
2. Replace "#Add your Gemini Api key" with your Gemini API key.
3. Replace "#Add your Ngrok auth token " with your ngrok token.
4. Run the notebook to start the FastAPI server.
5. Use the generated public URL to access the `/docs` Swagger UI.

# Example Query

Use the following JSON to test the `/run-agent/` endpoint:

```json
{
  "query": "Book a flight to New York on July 10, hotel for 3 nights, and block my calendar for vacation"
}
